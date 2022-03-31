---
title: Appairage
description: 
published: true
date: 2022-03-31T19:16:36.508Z
tags: 
editor: markdown
dateCreated: 2022-03-13T19:07:38.093Z
---

## Appairage du plugin JeeMate avec votre appareil

Après téléchargement du plugin, vous devez commencer par l’activer.

Ensuite, vous devez **créer un équipement**. Pour cela :

  
1\. Accéder à la page « Plugins > Communication > JeeMate »

![](https://dev.jeemate.fr/wp-content/uploads/2021/07/jeemate_select_plugin.webp)

2\. Cliquer sur « Ajouter » pour créer votre premier appareil.

![](https://jeemate.fr/wp-content/uploads/2021/10/Appairage01-1024x334.png)

1.  Saisir/sélectionner les informations concernant votre nouvel appareil: nom, objet Jeedom, utilisateur Jeedom que vous souhaitez rattacher, les droits JeeMate.

-   Utilisateur : permet de définir quel utilisateur Jeedom se connecte à l’application. Les droits utilisateurs configurés dans Jeedom sont pris en compte par JeeMate.
-   Droit de renommer : autorise l’utilisateur à renommer l’équipement depuis l’application mobile. Il s’agit d’un nom d’équipement alternatif, il n’écrase pas le nom que vous avez défini dans Jeedom.
-   Droit de changer la visibilité : permet de choisir depuis l’application mobile les équipements visibles ou non

![](https://dev.jeemate.fr/wp-content/uploads/2021/07/jeemate_add_device_2-1024x428.webp)

1.  Choisir le mode d’appairage:

-   via QrCode
-   via l’appairage automatique (réseau local uniquement)

1.  Premier lancement de l’app JeeMate

-   Si ce n’est pas déjà fait, installer l’application depuis le store ou en la téléchargeant sur le site
-   Puis suivez les étapes proposées dans l’assistant si elles n’ont pas déjà été faites précédemment
-   Scanner le QR code présent ou effectuer l’appairage auto sur l’équipement créé sur Jeedom.
-   Valider la procédure.

**Pour qu’un équipement apparaisse dans JeeMate, l’équipement doit:**

-   **être visible, rafraichir la page si ce n’est pas le cas.**
-   **avec des types génériques configurés sur ses commandes info et action. Sauf si le plugin est compatible avec gestion avancée (voir section fonctionnalités la liste des plugins).**

Pour chaque équipement créé, une liste de commandes est disponible ainsi qu’un onglet « Backups » permettant de gérer les sauvegardes de la configuration de l’application mobile par utilisateur.

Depuis le plugin, sont disponibles :

-   **Configuration** et administration de l’appairage
-   **Vos appareils** : liste les appareils utilisé avec jeemate et l’équipement auquel ils sont rattaché.
-   **Configuration Jeemate**: permet de définir depuis le plugin quels équipements, scénarios ou designs importer (peut aussi être géré depuis l’application mobile) ainsi que leurs types génériques.
-   **Géo repérage** : permet de définir les zones de géolocalisation. (plus d’infos, section géolocalisation)
-   **Notifications** : permet de configurer des modèles de notifications. (plus d’infos, section notifications)
-   **Débug fonction** : permet de nous fournir des informations concernant votre import pour le support

**Si certains de vos équipements ne sont pas importés dans l’application, vérifiez que :**

-   vos équipements sont actifs dans Jeedom
-   qu’ils fonctionnent correctement sur le dashboard Jeedom
-   qu’ils sont cochés/sélectionnés pour l’import dans le plugin JeeMate/Configuration JeeMate