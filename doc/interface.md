---
title: Interface
description: 
published: true
date: 2022-03-31T19:40:13.202Z
tags: 
editor: markdown
dateCreated: 2022-03-13T19:15:34.386Z
---

# Présentation de l’interface

JeeMate a été conçue pour être facile à utiliser

L’application est décomposée en plusieurs parties

L’application est décomposée en quatre onglets, par défaut. Il est possible d’en créer, cacher, réorganiser, ou customiser leur icône.

-   Favoris Maison
-   Pièces
-   Designs Jeedom et pages web favorites
-   Caméras

![Interface-481x1024.jpg.webp](/img/doc/Interface-481x1024.jpg.webp)

Pour naviguer entre les onglets, il suffit de cliquer sur les boutons dans la barre d’onglets en bas de l’application.

Lorsque vous cliquez sur les boutons Pièces, ainsi que Designs, une liste apparaitra afin de sélectionner la Pièce ou le Design que vous souhaitez afficher

Pour créer un nouvel onglet, ou éditer un onglet existant il suffit de faire un appui long sur la barre d’onglet afin d’afficher la page d’édition.

![](/img/doc/Onglets-1-273x300.jpg.webp)

Depuis la page d’édition, faire un appui long puis glisser pour réorganiser les onglets et cocher pour rendre visible.

**Les onglets par défaut ne peuvent pas être supprimés. L’onglet Maison ne peut être ni caché, ni déplacé.**

Cliquer sur le nom d’un onglet pour accéder à sa configuration.

![](/img/doc/Onglet-configuration-2-207x300.jpg.webp)


# Onglets Favoris Maison

L’écran principal contient les sections suivantes :

![](/img/doc/zone-interface.png.webp)

1.  Barre d’outil tout en haut.  
    Permet d’accéder au menu latéral gauche de configuration JeeMate, au statut de connexion, aux notifications, de rafraîchir les statuts des équipements, ou bien d’ouvrir le menu latéral droit.
2.  Résumé global Jeedom (dépend de la configuration des résumés dans Jeedom) ainsi que l’affichage des membres présents si configurés dans votre Jeedom (un clic sur l’icône permet d’afficher la liste des membres et leur statut).
3.  Scénarios favoris
4.  Equipements et applications Android favoris
5.  barre d’onglets

![](/img/doc/resume.png.webp)

Les résumés peuvent être personnalisés. Pour cela il suffit de faire un appui long sur la barre de résumés. Vous pourrez alors modifier les icônes et couleurs. Pour revenir en arrière et avoir de nouveau les icones et couleur configuré dans Jeedom, faite réinitialiser puis sélectionner les icones souhaitées.

### Ajout de favori

Pour ajouter un favori (Équipements, Scénarios, Groupes, Applis Android), cliquez sur le crayon en haut à gauche de l’écran, puis choisir le type de favori que vous souhaitez ajouter.

![favoris-206x300.jpg.webp](/img/doc/favoris-206x300.jpg.webp)

### Personnalisation des tuiles

Dans les onglets, il est possible de réorganiser et redimensionner les tuiles.

Pour pouvoir réorganiser les tuiles, il suffit de cliquer sur le bouton « Crayon » dans la barre, coin haut droit de l’écran. Puis dans le menu latéral, activer la fonction « Éditer ».

Une fois le mode « Éditer » actif, il est alors possible de réorganiser une tuile en faisant un clic long puis en la déplaçant. Mais aussi, de faire un double clic pour redimensionner la tuile (suivi d’un double clic pour valider le redimensionnement)

Pour afficher le menu de personnalisation d’une tuile, il suffit de faire un appui long sur la tuile.

Note: le menu est disponible si le mode « Éditer » est **inactif**.

D’autres options peuvent être accessibles en fonction du type de tuile (Groupes/Panels etc)

![EditionTuile-285x300.jpg.webp](/img/doc/EditionTuile-285x300.jpg.webp)

Tuile Taille mini ou normale :

![MiniNormale-300x168.jpg.webp](/img/doc/MiniNormale-300x168.jpg.webp)

Contenu centré ou aligné à gauche :

![IMG_20211029_144514-2-300x151.jpg.webp](/img/doc/IMG_20211029_144514-2-300x151.jpg.webp)

Grille : permet de changer le nombre de colonnes de tuiles dans les onglets.

![Grille.gif](/img/doc/Grille.gif)

Configuration : Ici on accède à tous les réglages disponible sur une tuile (changer le nom, l’icone, etc…)

![ConfigurationTuile-768x1156.jpg.webp](/img/doc/ConfigurationTuile-768x1156.jpg.webp)

**Configurer les commandes (coché)**  
  
**Commandes infos et actions :**  
La liste des ID des commandes de votre équipement.  
  
**Rendu conditionnel :**  
Modifications de l’icone, un mode avancé permet de personnaliser encore davantage.  
  
**Commandes optionnelles :**  
Si votre équipement en dispose vous pouvez mettre les infos batterie, connecté, etc…, ce sera visible sur la page détails de votre tuile.  
  
**Rendu conditionnel vue détails :**  
Ajouter une image de fond sur la page détails de votre tuile, possibilité d’y mettre également des conditions.  
  
**Personnaliser tuile :** (plus d’info en dessous)  
  
**Indicateur lumineux tuile :**  
Utiliser la led de la tuile dans des conditions.  
de base rouge fixe si la batterie est faible, rouge qui clignote si info sabotage activé.  
Il vous est possible d’ajouter des conditions (voir info dédié)

**Personnaliser tuile :**

![PersonnaliserTuile.jpg.webp](/img/doc/PersonnaliserTuile.jpg.webp)

**D’autres options peuvent être accessibles en fonction du type de tuile (Groupes/Panels etc)**

## Contrôle d’un équipement

**_Simple clic sur tuile_**

Sur les tuiles actions de type lumières, volets ou prises, exécute l’action.  
**– Si dans jeedom un mot de passe est défini pour la commande à exécuter alors il vous sera demandé à l’aide du digicode ou du capteur d’empreinte.**  
Sur les tuiles actions du style multimédias, thermostats, etc…, ouvre la page dédiée.

Sur les tuiles infos du style température, ouvrant, détecteur, etc…, ouvre la page détails et historique.

**_Double click sur tuile_**

Sur les tuiles actions du style lumières, volets, ouvre la page des commandes supplémentaires.

**_Les pages spécifiques_**

| **Thermostat** | **Alarme** | **Mode** |
| --- | --- | --- |
| ![](/img/doc/PageThermostat-scaled.jpg.webp) | ![](/img/doc/PageAlarme.jpg.webp) | ![](/img/doc/PageMode-scaled.jpg.webp) |
|     |     |     |
|     |     |     |
| Eclairage Luminosité | Eclairage Température de couleur | Eclairage couleur |
| ![](/img/doc/PageLumiereLum-scaled.jpg.webp) | ![](/img/doc/PageLumiereTemp-scaled.jpg.webp) | ![](/img/doc/PageLumiereCouleur-scaled.jpg.webp) |
|     |     |     |
|     |     |     |
| Multimédia |     |     |
| ![](/img/doc/PageMultimedia-2-scaled.jpg.webp) |     |     |

## Onglet Pièces

![](/img/doc/Photo1-1.webp)

De la même manière que pour l’onglet Favoris, l’écran contient trois sections :

1.  Résumés
2.  Scénarios
3.  Equipements  
      
    La personnalisation des tuiles est identique aux onglets favoris, ici seul l’option afficher nom de la pièce ne sera pas pris en compte.

Il est possible de customiser l’affichage pour chaque pièces en cliquant sur l’icône d’édition (crayon) en haut à droite dans la barre d’outils JeeMate.

![](/img/doc/jeemate_edit_piece.webp)

Il sera alors possible de :

-   Définir la pièce par défaut lorsque l’on clique sur la barre d’onglet pour accéder aux pièces
-   Renommer la pièce
-   Choisir une image de fond
-   Choisir l’image de Synthèse Jeedom en fond
-   Choisir une couleur/dégradé de fond
-   Utiliser le thème par défaut
-   rendre visible ou non les tuiles

## Designs Jeedom et pages web favorites

Cet onglet permet d’afficher des pages web. Telles que :

-   Designs Jeedom
-   Vos dashboards Grafana préférés
-   etc

Pour cela, il suffit de cliquer sur le bouton Onglet « Design » dans la barre en bas, puis sur l’icône « Roue crantée ».

![](/img/doc/jeemate_onglet_design.webp)

Dans la page « Liste des designs », il est possible de :

-   Ajouter un design
-   Choisir d’afficher le design par défaut au démarrage de JeeMate
-   Trier par ordre alphabétique les designs de la modale de sélection
-   Changer l’ordre des designs, de la même manière que les tuiles en appuyant pendant quelques secondes sur le design puis déplacer
-   Éditer la configuration d’un design en cliquant dessus

Pour ajouter un « design » ou url vers une page web, il suffit de cliquer sur le bouton « + », puis

-   Visible : si vous souhaitez cacher ou non le design dans la modale de sélection
-   Défaut : pour définir le design par défaut à afficher lorsque l’on clique sur le bouton Onglet « Design »
-   Saisir un nom
-   Saisir son URL
-   La fréquence de rafraichissement si besoin

## Onglet Caméras

L’onglet Caméras permet de visualiser toutes les caméras disponibles dans Jeedom ou non, et en Live!  
Les caméras présentes dans Jeedom sont automatiquement importées.

![](/img/doc/jeemate_onglet_camera.webp)

Cliquer sur le bouton « + » pour ajouter une caméra puis :

-   saisir un nom
-   et son URL

La caméra apparaitra alors dans JeeMate. Vous pourrez ensuite rééditer ses paramètres, ou bien la supprimer, en swipant sur son nom pour faire apparaître le menu de configuration.

La liste des caméras peut être réorganisée. Pour cela, il suffit d’appuyer pendant quelques secondes dessus et ensuite de la placer à l’endroit souhaité.

Un clic simple sur la caméra permet de l’afficher en plein écran et avoir accès aux boutons PTZ.

# Menu JeeMate

Accessible depuis le bouton Menu, dans la barre d’outils JeeMate, en haut, il permet :

![](/img/doc/jeemate_burger.webp)

Accessible depuis le bouton Menu, dans la barre d’outils JeeMate, en haut, il permet :

-   d’afficher la page Synthèse Jeedom
-   d’afficher la page Timeline de Jeedom
-   d’accéder à la configuration de Jeemate
-   A propos  
      
    Vous sera demandé pour la version de l’application et la résolution lors de débug.  
    Liens github (pour les signalements de bugs)  
    Liens discord (pour discuter et s’entre-aider)