---
title: Configuration
description: 
published: true
date: 2022-03-31T19:25:31.727Z
tags: 
editor: markdown
dateCreated: 2022-03-13T19:10:49.031Z
---

# Configuration

Le menu « Configuration » permet de paramétrer :

-   les notifications avec TTS ou non
-   la géolocalisation (Activer, définir des zones, affiner les réglages pour le geofencing et la durée de la batterie)
-   le lien JeeMate<->Jeedom. Ici rien à configurer. Mais ce menu permet de synchroniser JeeMate avec votre serveur Jeedom et de mettre à jour de nouveaux équipements. Il permet sinon, de ré-appairer votre téléphone, ou bien de remettre à zéro l’interface graphique
-   Activer la détection d’objet de la caméra de votre appareil et plus tard envoyer la vidéo vers Jeedom
-   Activer le service SMS pour recevoir ou envoyer des SMS, avec gestion d’une liste blanche des contacts
-   Active le service SIP. Pour l’instant testé uniquement avec Asterisk. Sert à communiquer en audio+vidéo avec par exemple des portiers vidéos, softphones etc
-   Sécurité (Activer ou non les biométriques, digicode etc). Afin d’empêcher que quelqu’un d’autre n’utilise JeeMate.
-   Thèmes&Langues. Entre autres, afficher une image, ou des dégradés de couleurs, en fond d’écran, activer le thème jour/nuit, choisir les fonds d’écran pour chaque mode etc
-   Sauver/Importer App. Permet de sauvegarder la configuration, les favoris, pièces etc de JeeMate dans votre serveur Jeedom. Importer permet donc de réimporter une sauvegarde.

![jeemate_configuration.webp](/img/doc/jeemate_configuration.webp)

# Géoloc

# Connecteur Jeedom

-   Activer/Désactiver la connexion avec votre serveur Jeedom
-   Paramètres de connexion à votre serveur Jeedom (adresse interne, externe etc) récupérés lors du scan de qrcode
-   Local Wifi : vous pouvez soit cliquer sur le bouton, soit saisir votre Nom de Wifi local.
-   Scanner le QR Code : permet de rescanner le QR Code de votre équipement dans le plugin JeeMate et ainsi mettre à jour la configuration ci-dessus
-   Re-générer l’interface : importe vos équipements Jeedom dans JeeMate
-   Effacer les favoris : permet de réinitialiser l’affichage des favoris dans l’onglet Maison
-   Effacer l’interface : permet de réinitialiser complètement l’interface
-   Tester la connexion : permet de tester la connexion entre l’application mobile et votre serveur Jeedom

![jeemate_configuration.webp](/img/doc/jeemate_jeedom_settings.webp)
# Caméra

*Temporairement désactivé*

-   Streaming (pas encore disponible)
-   Activer la reconnaissance d’objets (exemple : détection humain)
-   La précision de la reconnaissance (score mini)

![jeemate_configuration.webp](/img/doc/jeemate_intcam_settings-300x266.webp)
# Reconnaissance vocale

JeeMate permet de contrôler votre Jeedom, en mode offline. C’est-à-dire que la reconnaissance du hotword ainsi que la transcription de la voix en texte est faite sur votre appareil, et ne passe pas par le Cloud.

-   Interactions : si l’option est activée, la commande vocale est envoyée aux Interactions Jeedom
-   Rhasspy plugin : si l’option est activée, la commande vocale est envoyée à Rhasspy
-   Toujours active : si l’option est activée, l’appareil reste en permanence sur écoute, en attente d’une commande. Dans ce mode, la configuration d’un hotword est obligatoire
-   Hotword : la phrase clé que vous souhaitez pour valider une commande. Exemple : « Jasper », « Dis Toto » etc

![jeemate_configuration.webp](/img/doc/jeemate_recovocal_settings-300x282.webp)

# Service SMS

*Version Hors Stores (Android)*

Il est possible d’utiliser un ancien mobile comme passerelle entre Jeedom et les SMS.

-   Autoriser ou non l’envoi de SMS depuis Jeedom
-   Autoriser ou non la réception de SMS
-   Interactions : si l’option est activée, le contenu du SMS est envoyé aux Interactions Jeedom
-   Rhasspy plugin : si l’option est activée, le contenu du SMS est envoyé au plugin Rhasspy
-   Liste blanche permet d’ajouter/supprimer des contacts autorisés. Tout SMS, envoyé par un contact non présent dans cette liste blanche, ne sera pas transmis à Jeedom

![jeemate_configuration.webp](/img/doc/jeemate_sms_settings-268x300.webp)
# Service SIP

Il est possible de connecter JeeMate à un serveur compatible Asterisk, et d’effectuer ou recevoir des appels audios/vidéos SIP (softphones, portier vidéo etc)

Exemple d’un appel softphone Windows (PC sans webcam) vers JeeMate

![jeemate_configuration.webp](/img/doc/sip_call-287x300.webp)

# Sécurité

-   Activer biométriques : permet d’activer la reconnaissance sur empreinte digitale, ou faciale
-   Activer digicode : permet d’activer l’utilisation d’un digicode
-   Digicode : saisir le code souhaité
-   Sécuriser lancement JeeMate : permet de sécuriser le lancement de l’app avec une des options ci-dessus
-   Sécuriser menu Configuration : permet de sécuriser l’accès au menu Configuration de JeeMate, cela bloque également toutes les configuration accessible sur les pages, tuiles, onglets.

**Si vous configurez un mot de passe sur vos commandes dans Jeedom (dans les paramètres des commandes), alors ce sera dernier qui sera utilisé en priorité. Le digicode sera d’ailleurs affiché même si le digicode n’est pas activé.**

![jeemate_configuration.webp](/img/doc/jeemate_security_settings.webp)
# Interface

-   Choix de la langue. Pour l’instant les langues disponibles sont Français, Anglais, et Espagnol. D’autres seront ajoutées. La langue est automatiquement sélectionnée en fonction de celle qui est configurée dans votre appareil mobile.
-   Activer/désactiver Image de fond pour l’onglet Favoris Maison
-   Choix de l’image de fond pour l’onglet Favoris Maison
-   Activer/Désactiver le changement automatique de thème Jour/Nuit
-   Choix du Dégradé pour le thème Jour
-   Choix du Dégradé pour le thème Nuit
-   Thème : Morphic ou Glass
-   Mode : Jour ou Nuit

![jeemate_configuration.webp](/img/doc/jeemate_theme_settings1.webp)

-   Transparence/opacité et couleurs des tuiles: uniquement disponible en thème Glass
-   Transparence par défaut utilisée lorsque la tuile est à l’état ON
-   Transparence par défaut utilisée lorsque la tuile est à l’état OFF
-   Couleurs des différentes zones dans les tuiles et l’application

**Si vous ne souhaitez pas avoir de différence de transparence lorsque la tuile est ON/OFF, alors il suffit de mettre les 2 sliders sur la même valeur.**

![jeemate_configuration.webp](/img/doc/jeemate_theme_settings2.webp)

# Sauver/Importer App

-   Sauvegarder : permet d’enregistrer toute la configuration de votre application mobile, paramètres et interface, dans votre serveur Jeedom. Vous devez saisir un nom pour votre sauvegarde.
-   Sauvegardes disponibles : permet de récupérer dans votre serveur Jeedom la sauvegarde de votre application mobile. La Liste des sauvegardes disponibles est automatiquement rafraîchie ou en cliquant sur « Sauvegardes disponibles. »
-   Dans le plugin JeeMate, vous pouvez ensuite aller sur votre équipement et définir si votre sauvegarde est globale ou non. Si elle est globale, alors elle sera disponible pour vos autres équipements afin de la partager.

![jeemate_configuration.webp](/img/doc/jeemate_backup-599x1024.webp)


## Capteurs disponibles sur votre appareil JeeMate

|     |     |     |
| --- | --- | --- |
| **Nom** | **Sous-type** | **Description** |
| State Lux Sensor | Info | Luminosité (en Lux) détectée par votre appareil JeeMate |
| State Battery | Info | Niveau de batterie de votre appareil JeeMate |
| State Signal | Info | Qualité de réception (en dB) de votre appareil JeeMate |
| IP JeeMate | Info | Addresse IP de votre appareil JeeMate |
| Charging State | Info | Statut de charge de l’appareil |
| Geoloc Position | Info | Position GPS de votre appareil |
| (geoloc) geofence | Info | Une info binaire par zone |
| (geoloc) Distance de geofence | Info | Distance en mètres depuis votre position à la bordure de la zone |

## Send SMS

Send SMS est une commande de type message que vous pouvez utiliser depuis votre serveur Jeedom, par exemple dans les scénarios, afin d’envoyer un SMS depuis l’application mobile JeeMate.

|     |     |
| --- | --- |
| **Paramètre** | **Valeur** |
| Titre | N° téléphone destinataire |
| Message | Le message à envoyer |

## TTS Speak

TTS Speak est une commande de type message que vous pouvez utiliser depuis votre serveur Jeedom, par exemple dans les scénarios, afin de faire parler l’application mobile JeeMate.

|     |     |
| --- | --- |
| **Paramètre** | **Valeur** |
| Message | Le message à envoyer |