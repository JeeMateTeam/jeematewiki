---
title: Présentation
description: 
published: true
date: 2022-03-31T20:08:28.178Z
tags: 
editor: markdown
dateCreated: 2022-03-13T19:25:38.144Z
---

# JeeMate

JeeMate est une application mobile compatible avec Jeedom.  
Contrôlez facilement votre maison intelligente grâce à son interface intuitive et customisable

JeeMate est une application mobile compatible avec Jeedom disponible sur Android, IOS, Windows, MacOS, et très bientôt sur AndroidTV OS ainsi que Linux.  
Contrôlez facilement votre maison intelligente grâce à son interface intuitive et customisable.

Sentez-vous toujours proche de chez vous !  
Depuis n’importe où, vous pourrez :

-   Interagir avec votre maison intelligente
-   Monitorer et contrôler vos équipements
-   Recevoir et répondre aux notifications PUSH, textes, images et/ou vocales.
-   Gérer la présence et automatiser des actions en fonction de votre localisation
-   Visualiser vos caméras, ou streams externes en Live
-   Visualiser l’historique de vos équipements si préalablement activé dans Jeedom
-   Envoyer des commandes vocales à votre serveur Jeedom, sans passer par les serveurs Cloud, avec écoute en continue ou non, et hotword custom
-   Utiliser l’application en mode tablette de contrôle à la maison, et utiliser des fonctions d’intelligence artificielle de la caméra
-   Envoyer et recevoir des sms
-   etc.

## Customisation

Grâce à son interface customisable, vous pourrez aussi :

L’application mobile et son plugin ont été développés avec comme objectifs principaux :

-   Définir des équipements et scènes favoris
-   Réorganiser l’ordre d’affichage
-   Customiser vos widgets
-   Customiser l’affichage global ou par pièces
-   Customiser certaines parties de l’interface
-   Changer complètement l’interface, grâce aux différents thèmes ainsi que leurs variantes Jour/Nuit aka « Light/dark »
-   Sécuriser l’accès à chaque équipement! Grâce à un digicode ou la reconnaissance biométrique (faciale ou empreinte digitale)
-   Afficher vos designs Jeedom et autres pages favorites, comme des pages persos Grafana ou autres
-   Ou encore créer des scénarios grâce à son éditeur.
-   etc.
-   « mobile-first » afin de réduire la dépendance à un autre périphérique tel qu’un ordinateur que ce soit pour le rendu dans l’application mobile et d’autres tâches quotidiennes
-   contrôler votre maison intelligente le plus simplement possible, avec le moins d’étapes tout en ayant de nombreuses possibilités de customisation
-   réduire le nombre de plugins utilisés et les ressources de votre serveur Jeedom
-   réduire le nombre d’applications mobiles utilisées et les ressources de votre équipement

JeeMate gère aussi les droits utilisateurs et mots de passe Jeedom sur les commandes, préalablement définis dans votre Jeedom.

L’utilisation continue du GPS en tâche de fond peut réduire la durée de vie de la batterie. JeeMate contient des paramètres afin d’optimiser ceci.

## Exemples d'interface


![Exemple Interface 5](https://jeemate.fr/wp-content/uploads/2021/07/diapo5-1024x711.webp)

![](https://jeemate.fr/wp-content/uploads/2021/10/Thermostat-0.9.7-1024x576.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/10/Console-0.9.7-1024x640.jpg)

![Exemple Interface 1](https://jeemate.fr/wp-content/uploads/2021/07/diapo1-1024x640.webp)

![Exemple Interface 2](https://jeemate.fr/wp-content/uploads/2021/07/diapo2-1024x640.webp)

![Exemple Interface 3](https://jeemate.fr/wp-content/uploads/2021/07/diapo3-1024x640.webp)

![Exemple Interface 4](https://jeemate.fr/wp-content/uploads/2021/07/diapo4-1024x640.webp)

![Exemple Interface 5](https://jeemate.fr/wp-content/uploads/2021/07/diapo5-1024x711.webp)

![](https://jeemate.fr/wp-content/uploads/2021/10/Thermostat-0.9.7-1024x576.jpg)

![](https://dev.jeemate.fr/wp-content/uploads/2021/07/Photo1-1.webp)

-   **Onglet Pièces**  
    Affichez et contrôlez vos différents équipements par pièce

![](https://dev.jeemate.fr/wp-content/uploads/2021/07/Photo2.webp)

-   **Widgets**  
    Personnalisez votre widget en fonction de son état

![](https://dev.jeemate.fr/wp-content/uploads/2021/07/Photo3.webp)

-   **Widgets**  
    Personnalisez vos widgets

![](https://dev.jeemate.fr/wp-content/uploads/2021/07/Photo4-492x1024.webp)

-   **Tuiles**  
    Personnalisez vos tuiles

# Changelog Jeemate

## **V1.0.0** (BETA)

-   ***Breaking Change : Une nouvelle version de l’application va sortir le 16/01/2022, cette version BETA ne contiendra pas encore le system de migration. Nous vous conseillons de faire un backup le temps que le system soit intégré***
-   Fix : Correction de la carte qui ne s’affichait plus en 4.2
-   Fix : Mise à jour de system du génération du QR Code pour rentré dans les règles de sécurité de la 4.2
-   Fix : Correction de plusieurs erreurs PHP
-   Amélioration : Mise en service de la nouvelle API Compatible avec la version 1.0.0 de l’application. (Reste grandement compatible avec la version 0.9)
-   Amélioration : Ajout d’options pour les notifications ainsi que changement du system pour améliorer la fiabilité
-   Ajout : Intégration des plugins ZigbeeLinker et deCONZ dans la page santé Zigbee
-   Ajout : Mise en place des API pour la gestion de la santé de Jeedom ainsi que de la mise à jour des plugins
-   Ajout : Mise en place des API pour la gestion du multi Jeedom  
     

## V0.9.10

-   Correction d’un bug avec les virtuels
-   Preparation a la prochaine version de JeeMate
-   Ajout de la fonction de … chut ^^

## V0.9.9

-   Correction d’un bug avec les virtuel
-   Correction des notifications
-   Ajout d’une option pour cacher les doubles notifications
-   Multiple corrections de bug, Merci Sagitaz

## V0.9.8

-   Correction Json Notification
-   Correction Icon Notification
-   Correction de petits bugs dans le plugin
-   Ajout de la commande pour les SMS

## V0.9.7

-   Mise à jour des interfaces du plugin
-   Ajout des nouvelles API pour la prochaine version de l’app
-   Ajout de nouvelles commandes (pas toutes fonctionnelles)
-   Refonte du système de notification
-   Refonte du système de géolocalisation
-   Refonte du système d’event
-   Prise en charge de Windows
-   Prise en charge de MacOS
-   Compatibilité Jeedom 4.2
-   Multiples corrections de bug
-   Ajout des fonctions de stockage d’images pour les applications
-   Breaking Change : Cette version met en place plein de nouveaux systèmes, les commandes seront déplacées dans l’onglet OLD pour pouvoir transférer les commandes sur les nouvelles
-   (22h30) Correction TTS
-   (22h30) Correction Notifications
-   (22h30) Correction des sessions User

## V0.9.3 (29/07/2021)

-   Mise à jour des liens de changelog et de documentation
-   Adaptation pour la 0.9.3 de l’application
-   Ajout d’une option pour supprimer les téléphones en double ou triple
-   Ajout de l’application sur l’Amazon Store. (Encore en validation)
-   Correction des Geofence et GeoLoc

## V0.9.2+2 (24/06/2021)

-   Correction de plusieurs bugs
-   Ajout d’options pour debugger le plugin
-   Attention il y a actuellement des bugs de GeoLoc, c’est en attente de debug que je retrouve une connexion internet pour faire des tests. (Peut-être milieu de semaine prochaine)

## V0.9.2 (19/06/2021 à 19h30)

-   Ajout d’un assistant pour la création d’un nouvel équipement
-   Ajout de la gestion automatique des identifiants Market
-   Ajout de paramètres pour la précision des Geofences
-   Auto-configuration des génériques des équipements JeeMate
-   ***Breaking Change*** : Nouvel équipement. Attention : vos anciens équipements en 0.8 ne sont plus compatibles.
-   ***Breaking Change :*** Nouveau système de backup. Attention : vos anciennes sauvegardes en 0.8 ne sont plus compatibles.
-   Prise en charge de nouveaux OS : Android, IOS, Windows, Linux, Android TV, Web
-   Prise en charge des versions store
-   Update des Interfaces
-   Update des API pour correspondre à l’application en 0.9.2
-   Update du backend de gestion
-   Update des fonctions API sur la gestion des notifications

## V0.9.1 (30/04/2021 à 23h59)

-   Nouveau système d’appairage de l’app avec le plugin, sans QR code
-   Nouveau système de tuiles, nouvelles interactions, redimensionnables (ce point est encore en cours d’amélioration), multi widgets, …
-   Customisation des widgets, résumés. : images/icônes et couleurs, titres et sous-titres, …
-   Slider discret intégré dans la tuile quand l’équipement le permet
-   Volet, lumières, peuvent par exemple être pilotés sans ouvrir la page dédiée
-   Possibilité de créer/cacher/supprimer/réorganiser des onglets Favoris, auparavant vous étiez limité à un seul
-   On peut par exemple mettre des caméras dans les onglets Favoris, ce n’est plus limité à l’onglet Caméra.
-   Notifications avec grandes icônes, emojis, boutons actions dans le centre notifs en cours d’ajout (nous attendions une version stable de la lib pour iOS avant de l’ajouter)

## V0.8.3 (22/02/2021 à 00h10)

-   Update lien APK
-   Update des event sans action
-   Update du system de GeoLoc
-   Add System de notification personnalisée : [_Issue_](https://github.com/JeeMateTeam/JeeMate-Project/issues/72)

## V0.8.2 (15/02/2021 à 20h00)

-   Correction pour les equipment du plugin KNX

## V0.8.1 (14/02/2021)

-   Mise en stable pour la compatibilité du plugin avec L’app au lancement de du bêta

## V0.8 (02/02/2021)

-   Ajout de la timeline

# Changelog Plugin

## **V1.0.0 23/01/2022** (BETA)

-   Clics sur le nom dans la session dans la barre de menu du 1er onglet: Clic simple: menu changement rapide session Clic long: page de gestion des sessions
-   Ajout/correction dans la page Config Geoloc de l’app, d’une option pour définir le jeedom qui recoit les events de geoloc
-   Correction scénarios provenant d’une pièce vide
-   Correction iOS scroll en bas de page
-   Correction icone Garage
-   Correction de l’interface dans la page détails Météo
-   Correction Raccourcis systèmes (veuillez reconfigurer vos raccourcis, 4 raccourcis max)
-   Correction volume media. Note1: pour les medias, le plugin jeemate a actuellement quelques soucis d’envoi events/refresh vers l’app, corrigés prochainement Note2: corrections playlist et radio en cours pour certains plugins (sonos..), probablement dispo dans prochaine maj
-   Correction lastCommunication page détails
-   Correction lien github dans page About

## **V1.0.0 21/01/2022** (BETA)

-   Ajout possibilité de configurer les raccourcis systèmes pour chaque session
-   Correction delete raccourci système
-   Correction icone vert/rouge dans Page détails Santé
-   Correction dans Pièce, éditer, utiliser image de la synthese : ne fonctionnait qu’en thème glass/dégradé global
-   Correction on ne pouvait pas renommer les onglets par défaut (maison etc)
-   Correction changement du nom de la session active n’était refresh dans onglet accueil que lors du reboot
-   Correction la popup design n’était pas filtrée en multijeedom
-   Correction page Plugin tenir compte de ne pas mettre à jour dans jeedom
-   Correction quand la configuration est sécurisée, verrouiller boutons mise à jour plugin
-   Correction de certains libellés FR/EN
-   Corrections dans l’import en cours

## **V1.0.0 20/01/2022** (BETA)

-   Passage de la page About en pleine page
-   Correction icone jeedom Mode dans la tuile
-   Correction couleur libellé bouton Mise à jour plugins
-   Correction Tuile Media Play/Pause, Slider Volume, et libellés
-   Réactivation de la fonction « Appliquer la personnalisation à des widgets compatibles » A betastester
-   Corrections dans l’import en cours

## **V1.0.0 19/01/2022** (BETA)

-   Ajout et correction des types génériques Volet BSO Slider, Véhicule dans App et plugin (widget véhicule en cours)
-   Ajout réorganisation des sessions
-   Ajout possibilité de lancer une session depuis les raccourcis systèmes
-   Correction personnalisation icone alarme ON qui écrasait le icone OFF
-   Correction pairing connection externe dans le step by step
-   Correction de certains plugins dans l’import piscine, sonos, googlecast, spotifyconnect, alexa amazon,deezer
-   Corrections dans l’import en cours

## **V1.0.0 18/01/2022** (BETA)

-   Correction import

## **V1.0.0** (BETA)

-   ***Breaking Change : Cette version BETA ne contiendra pas encore le system de migration. Nous vous conseillons de faire un backup le temps que le system soit intégré***

## **V0.9.**10+97

-   Correction de la validation premium (Windows)
-   Ajout de la connexion via câble internet (Android)

## **V0.9.**10+96

-   Correction de la validation premium (Android)

## **V0.9.**10+95

Version ajoutant des fonctions dans le module Télécommande et fixant quelques soucis de la version précédente **(En cours de validation sur les stores)**

**Rappel:** [_https://jeemate.fr/changelog-application/changelog-details/_](https://jeemate.fr/changelog-application/changelog-details/)

-   Télécommande: option pour afficher ou non un libellé dans le bouton, ou sous le slider
-   Télécommande: option pour afficher ou non l’icône dans le bouton
-   Télécommande: option pour choisir les icônes
-   Télécommande: option pour afficher des icônes conditionnelles dans le widget lcd
-   Télécommande: option pour sélection des couleurs slider
-   Correction: Netatmo: modules additionnels
-   Correction: Bloc vide est delete lorsqu’on ajoute un widget
-   Correction: Correction affichage page Thermostat Paysage depuis dernière maj bottombar
-   Correction: Correction Notifs personnalisées breaking change dans dépendance + harmonisation API
-   Correction: Plugin Alarme et Mode: sécurité
-   Correction: Notification

## **V0.9.**9+90

[_https://jeemate.fr/changelog-application/changelog-details/_](https://jeemate.fr/changelog-application/changelog-details/)

-   Création widget Télécommande
-   Image de fond tuile avec conditions
-   Option pour Afficher/Cacher la barre de résumés dans les onglets favoris
-   Option pour Ajouter un bloc vide/transparent dans les onglets favoris
-   Possibilité de cacher l’icône en sélectionnant la couleur « transparent » dans le sélecteur de couleur
-   Sécurité menu configuration bloque à présent la config caméra
-   Création et édition d’onglet utilisent la même page (auparavant la création était dans une popup)
-   Réactivation de la fonction pour appliquer une configuration d’un widget aux autres de même type
-   Correction: dégradés jour/nuit
-   Correction: import
-   Correction: SMS (bug suite à changement API dans le plugin) / Contacts
-   Correction: quand on passait en mode DNS Jeedom, il fallait reboot l’app
-   Correction: bug alignement barre de boutons en bas de page Thermostat
-   Windows: Ajout d’un bouton « Retour » lorsque la caméra est en plein écran

## **V0.9.**8

-   Correction Tuile Blanche
-   Widget Thermostat : Ajout mode manuel
-   Widget Thermostat : Ajout humidité
-   Widget Thermostat : Correction du bug de refresh
-   Work in Progress : Widget + Page Véhicule
-   Correction Popup config Scrollable
-   Ajout de logs lors de la vérification du Premium pour debug
-   Correction tuile volet
-   Correction fond d’écran volet
-   Correction bulle batterie Mini
-   Notification : Correction Icônes
-   Notification : Breaking Change, changement du paramètre « groupName » à « groupKey »

## **V0.9.7**

-   Android, iOS, Windows et MacOS (Très bientôt)
-   Création/Editeur de widgets (avec ou sans types génériques)
-   Nouveau sélecteur d’images/icônes et centralisation des images sur votre Jeedom
-   Raccourcis Android et iOS
-   Console de logs temps réel dans l’app
-   Intégration de plugins :
    -   Freetelec
    -   Android TV
    -   Telco (En Cours)
-   API Actions
-   Nouveau widget lumière avec option pour que le slider se cache automatiquement
-   Nouveau widget thermostat tout en un
-   Widget Tuile Map
-   Amélioration du design de certaines pages
-   Deeplinking en cours de finalisation
-   Import config des zones GeoLoc créées dans Jeedom
-   Widgets sur conditions
-   Fond d’écran onglets sur conditions
-   Page détail widget sur conditions
-   Indicateur lumineux de tuile sur conditions
-   Possibilité de cacher l’heure sur le widget Météo
-   Si on sécurise la configuration, cela cache les parties configuration widgets etc
-   Passage de tout le projet en null-safety
-   Comme d’habitude, dernière version de Flutter (le framework utilisé pour dev JeeMate) avec à chaque maj de belles améliorations des performances
-   Version **hors store** pour le mode **Android launcher** et la **gestion des sms** avec liste blanche de contacts autorisés
-   Optimisations
-   Corrections
-   Tous les autres points que l’on a oubliés

## **V0.9.5**

-   Correction: doublon biometric dans certains cas
-   Correction: les icônes Pièces nécessitaient de regen 2x
-   Correction: alignement des scénarios
-   Correction: accordéon lors d’une recherche d’icône
-   Correction: widget plugin AirQuality
-   Correction: sauvegarde personnalisation tuile dans un panel
-   Correction: ASK + titre notif dans la page Notifications + customIcon et iconColor
-   Correction: Configuration Sécurité: digicode et biometric une seule checkbox à la fois
-   Correction: Caméra mode paysage : ajout d’un bouton pour revenir en Portrait
-   La page détails Équipements pour les capteurs s’affiche sur clic ou double clic. L’ancienne popup historique a été supprimée.

## **V0.9.4**

-   Menu latéral : Switch Réorganiser est devenu Editer
-   Le mode active la réorganisation, ainsi que la possibilité d’activer le resize avec double clic au lieu d’ouvrir le menu
-   Dans menu contextuel, on peut maintenant switcher entre taille mini et normale
-   Correction de bugs

## **V0.9.3**

-   Actions groupées sur panels
-   Affichage tous les résumés lorsque l’on est en mode tablette dans la barre de menu
-   Ajout d’icônes de personnalisation
-   Ajout d’une icône de refresh dans la barre de menu
-   Ajout d’animations sur tuile météo: orage, lune, nuit étoilée
-   Aggrégation des types batterie/charging/online/sabotage+indicateur d’état
-   Caméra ajout d’un paramètre dans l’app config de la caméra pour forcer le mode snapshot lorsque Live est actif mais que la caméra n’est pas fullscreen (n’affecte pas le mode en fullscreen)
-   Couleurs dégradés dans les graphiques tuiles sont celles de la personnalisation
-   Changement barre de menu principale + barre de menu latérale droite
-   Dans ajout de widget, on peut créer des widgets raccourcis (et bientôt aussi les widgets équipements)
-   Intégration plugin AirQuality
-   Intégration plugin MyBin
-   Long press sur tuile pour afficher le menu contextuel
-   Nombreuses corrections
-   Suppression de la barre fixe de raccourcis
-   Optimisations
-   Personnalisation tuiles et widgets
-   Page détails équipement WIP (sur type capteur pour l’instant)
-   Pour réorganiser, activer l’option dans le menu droite. En mode réorganiser, on ne peut pas long press pour le menu contextuel, il faut désactiver