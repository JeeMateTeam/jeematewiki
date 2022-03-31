---
title: Geolocalisation
description: 
published: true
date: 2022-03-31T20:02:54.493Z
tags: 
editor: markdown
dateCreated: 2022-03-13T13:38:57.870Z
---

# Géolocalisation

Le module suit la localisation de votre appareil de manière optimisée afin de limiter la consommation de la batterie.  
Pour cette raison, la notion de détection de mouvement de l’appareil est très importante (mobile vs stationnaire). Le module lance le service uniquement lorsqu’il détecte du mouvement. Quand l’appareil reste stationnaire, les services de localisation sont stoppés.

![Geoloc-1-300x115.jpg.webp](/img/doc/Geoloc-1-300x115.jpg.webp)

Pour que les services de géolocalisations et la géofence fonctionne vous devez activer la fonction ici.

## Etats : Mobile & Stationnaire

Le module Géolocalisation peut prendre deux états : mobile et stationnaire, et passe d’un état à l’autre en monitorant le service Activité natif de votre appareil (immobile, à pieds, courir, à vélo et en véhicule).  
  
Vous avez la possibilité de configurer certains paramètres selon votre usage.  
  
**Lorsque vous êtes déconnecté du réseau Wifi/4G, alors les évènements détectés par le module (géoloc et zones) sont stockés sur l’appareil en attendant que la connexion soit rétablie, puis le module envoie l’historique à Jeedom.**  
  
**Pour un bon fonctionnement, vous devez avoir les autorisations correctement configurées, ainsi que les optimisations batterie désactivées pour JeeMate dans les paramètres Android de votre appareil\*\*** [**_https://dontkillmyapp.com/_**](https://dontkillmyapp.com/)

## Configuration

![Geoloc-4-289x300.jpg.webp](/img/doc/Geoloc-4-289x300.jpg.webp)

**_Domicile et zones_** : Voir Géofence  
  
**_Activer/Désactiver_** la géolocalisation  
  
**_Elasticité_** : permet d’activer ou non l’auto-adaptation de Distance Détection.  
  
**_Forcer la géolocalisation_** : désactive la reconnaissance d’activité et force la géolocalisation. Cette option peut être utilisée lors d’un entrainement ou d’un « Jogging » mais forcément va consommer un peu plus de batterie puisque la géoloc est forcée.  
  
**_Retour sonore_** : permet d’activer ou non un retour sonore sur les évènements de géoloc.

![Geoloc-3-300x235.jpg.webp](/img/doc/Geoloc-3-300x235.jpg.webp)

|     |     |     |
| --- | --- | --- |
| **Précision** | **Mode** | **Précision vs Autonomie** |
| NAVIGATION | (iOS seulement) GPS + Wifi + Cellular | Consommation batterie élevée; Meilleure précision |
| HIGH | GPS + Wifi + Cellular | Consommation batterie plus élevée; Meilleure précision |
| MEDIUM | Wifi + Cellular | Consommation batterie moyenne; Précision moyenne |
| LOW | Wifi (basse conso) + Cellular | Consommation basse; Pas de GPS |
| VERY LOW | Cellular seulement | Consommation très basse ; Précision faible |
| LOWEST | (iOS seulement) | Consommation la plus basse ; Précision la plus faible |

**_Intervalle Capteur_** : le service de géoloc va activement essayer de mettre à jour la position à cet intervalle. Donc cela peut aussi avoir un impact sur l’autonomie de la batterie. Ce n’est pas un intervalle exact, dans le sens où il ne veut pas forcément dire que vous recevrez une update à ce moment exactement.

**_Distance détection_** : correspond à la distance en mètres, que l’appareil doit parcourir afin de générer un évènement géoloc. Cette distance peut être « élastique » si « Activer Elasticité » est cochée.  
C’est-à-dire que quand Elasticité est active, Distance Détection augmente si la vitesse augmente et vice versa.  
Exemple :  
pour un vélo à 7.7m/sec, avec un Distance Détection de 30m, alors la distance ajustée est 60m.  
sur autoroute, à une vitesse de 27m/s, avec un Distance Détection de 50m, c’est ajusté à 300m.  
Ceci afin d’éviter les envois inutiles vers le serveur, car ce n’est pas forcément le GPS qui consomme le plus, la connexion et transfert de datas peuvent aussi beaucoup consommer.

**_Reconnaissance activité_** : Intervalle en secondes. Correspond aux moments où l’app vérifie qu’il y a une activité. Cette info est basée sur les différents capteurs du téléphone

![Geoloc-2-300x213.jpg.webp](/img/doc/Geoloc-2-300x213.jpg.webp)

**_Précision de la géolocalisation_** : permet de configurer la précision vs consommation de batterie

Pour plus de précisions concernant la distance de détection ou le mode « geofence seulement »:

[_https://pub.dev/documentation/flutter\_background\_geolocation/latest/flt\_background\_geolocation/Config/distanceFilter.html_](https://pub.dev/documentation/flutter_background_geolocation/latest/flt_background_geolocation/Config/distanceFilter.html)

[_https://pub.dev/documentation/flutter\_background\_geolocation/latest/flt\_background\_geolocation/Config/geofenceModeHighAccuracy.html_](https://pub.dev/documentation/flutter_background_geolocation/latest/flt_background_geolocation/Config/geofenceModeHighAccuracy.html)

Donc, pour optimiser la batterie il est mieux d’avoir Elasticité active, Forcer la géoloc désactivée. Et dans ce cas, lorsqu’aucune activité n’est détectée, alors le GPS etc sont stoppés pour conserver la batterie.

_Suivi de position et affichage du tracé_

Dans l’onglet position de votre équipement Jeemate se trouve 2 commandes de type infos (position et type d’activité).

![Capture-decran-2021-11-25-095102.png.webp](/img/doc/Capture-decran-2021-11-25-095102.png.webp)

Pour afficher une carte dans Jeemate il vous suffit d’importer votre équipement en le cochant dans la configuration Jeemate.  
Les génériques sont déja renseigné, si vous ne souhaitez pas remonter ces informations il faudra mettre aucun comme type générique.

![Geoloc04.png.webp](/img/doc/Geoloc04.png.webp)

Ensuite dans l’application vous pourrez afficher la carte de plusieurs façons.  
Simplement en cliquant sur l’icone présence dans la barre de résumé puis sur le nom de l’équipement.

Sinon vous pouvez ajouter une tuile sur vos onglets et soit cliquer dessus, soit l’agrandir.

## **Domicile et Zones (Geofence)**

### Gestion de la présence des membres

Il est possible, dans la barre des résumés d’afficher la présence des membres d’un foyer, leur géolocalisation, ainsi que leur trajet effectué.

Pour ceci, deux méthodes sont disponibles:

-   utilisation de l’équipement JeeMate seulement. Basée sur la géolocalisation et les zones déclarées dans JeeMate.
-   création d’un équipement Virtuel. Ceci permet plus de flexibilité dans le cas où vous souhaitez consolider/croiser votre info « zone » avec d’autres infos présentes dans jeedom

### Utilisation de l’équipement JeeMate seulement

Méthode recommandée, les générique sont déjà rempli, il vous suffit de cocher dans la configuration JeeMate votre équipement pour qu’il remonte ensuite dans l’application.

### Création d’un équipement Virtuel

La procédure à suivre est simple, et nécessite **un équipement Virtuel par membre**

![virtuel_presence.webp](/img/doc/virtuel_presence.webp)

Dans cet équipement, créer autant de commandes infos que d’états/zones possibles, comme sur la capture ci-dessus

-   Position : que vous pouvez lier à n’importe quel autre info géoloc, ou par exemple à la commande info de géoloc d’un équipement JeeMate. Cette info doit être de sous-type Autre. Cocher « Historiser » cette commande si vous souhaitez obtenir le tracé dans l’application mobile.
-   Etats/Zones : que vous pouvez lier à n’importe quel autre info provenant d’un autre plugin, ou par exemple à une commande info de géofence de l’équipement JeeMate.  
    Cette info doit être de **type Binaire**
-   **La commande info représentant la position doit avoir comme sous-type « Autre » et contenir: latitude,longitude**
-   **La commande info représentant l’état « présent/absent » doit avoir comme sous-type « Binaire » et contenir 0/1**

Ensuite, se rendre dans le plugin JeeMate, dans la section Configuration JeeMate

![virtuel_presence_display1.webp](/img/doc/virtuel_presence_display1.webp)

Puis dans l’onglet Objets, cliquer sur la roue crantée verte, et configurer l’équipement virtuel qui a été créé comme étant visible.

Et renseigner les types génériques comme ci-dessous,

-   Occupation
-   Géoloc

![virtuel_presence_generiques.webp](/img/doc/virtuel_presence_generiques.webp)

Cliquer sur Sauvegarder.

**Si un utilisateur ne souhaite pas être suivi, alors il suffit d’enlever le type générique pour la commande Position dans l’équipement Virtuel. Dans ce cas, seule sa présence ou non, sera indiqué dans l’application mobile.**

**Lorsque vous effectuez un changement dans la configuration d’un équipement Jeedom, alors il faut ensuite synchroniser l’application mobile en allant dans le menu Configuration/Jeedom/Regénérer l’interface..**

Pour afficher les informations de présence d’un utilisateur, depuis la barre de résumés, cliquer sur la première icône, une liste des utilisateurs sera alors affichée.

-   Cliquer sur l’icône pour accéder à la personnalisation des icônes états/zones et définir quel état représente la « présence à la maison » en activant la case à cocher si ce n’est pas déjà fait.
-   Cliquer sur un utilisateur dans la liste, et sera alors affichée la carte avec sa position, son tracé, la position des autres utilisateurs, ainsi que les différentes zones.

![trace.webp](/img/doc/trace.webp)