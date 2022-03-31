---
title: SendAction
description: 
published: true
date: 2022-03-31T20:03:10.750Z
tags: 
editor: markdown
dateCreated: 2022-03-13T19:35:57.722Z
---

# _Les commandes Send Action_

## _Afficher la page météo :_

Affiche la page des informations avancée de votre widget météo.  
 

## _Afficher Horloge :_

Non fonctionnel pour le moment  
 

## _Afficher Alarme :_

Affiche la page avancée de vos Alarme, celle affichée sera la première par ordre Alphabétique.  
 

## _Afficher le digicode :_

Affiche si vous en effet configuré un dans les options de jeemate le digicode. Entrer votre code pour le fermer.  
  
 

## _Afficher la synthèse :_

Affiche la page synthèse de votre installation, vous pouvez personnaliser les images des pièces ainsi que les résumes depuis la page objets de Jeedom.  
  
 

## _Smart Caméra :_

Non fonctionnel pour le moment  
  
 

## _Verrouiller application :_

Non fonctionnel pour le moment  
  
 

## _Assistant vocal :_

Non fonctionnel pour le moment  
  
 

## _Régénerer interface :_

Permet de faire un regen de votre interface jeemate  
  
 

## _Lancer une application :_

Vous permet de démarrer une des applications présente sur votre équipement.  
saisir dans le champ « message » le nom de l’apk.  
  
_exemple_  
pour lancer chrome saisir _com.android.chrome_  
pour lancer anticovid saisir _fr.gouv.android.stopcovid_

Pour récupérer facilement le nom de l’apk (android), click long sur l’icone de votre application, informations, puis le petit i en haut à droite.

![](https://jeemate.fr/wp-content/uploads/2021/11/LaunchApp02-300x212.jpg)

  
  
  
 

## _Afficher un design :_

Dans le champ message saisir l’id du design. Seule les designs coché dans Jeemate configuration sont affichable par cette commande.  
  
Vous trouverez cette informations soit dans l’url de votre design, soit dans le fichier GetDesign (Jeemate / Debug Fonction)  
  
  
 

## _Afficher la pièce :_

Dans le champ message saisir l’id de la pièce. Seule les pièces cochées dans Jeemate configuration sont affichable par cette commande.  
  
Vous trouverez cette informations soit dans l’url de votre pièce, soit dans le fichier GetObjects (Jeemate / Debug Fonction)  
  
  
 

## _Afficher un onglet :_

Dans le champ message saisir l’id de l’onglet à afficher.  
  
L’id de l’onglet Home est le 0, ensuite l’id est incrémenter sur les onglets actifs.  
  
  
 

## _Show Flap :_

Non fonctionnel pour le moment

## _Set Android Alarm :_

Vous permet de créer un Alarme sur votre devise Android.

Dans le champ titre il vous faut indiquer les informations de répétition, soit non, soit les jours de répétition.

![](https://jeemate.fr/wp-content/uploads/2021/11/android-alarm-03.png)

  
Pour que l’alarme soit seulement sur la journée en cour laisser le champ vide.  
Pour répéter l’alarme le lundi, jeudi et samedi mettre 2,5,7 ou 0,2,5

![](https://jeemate.fr/wp-content/uploads/2021/11/android-alarm-01.png)

Exemple sur le dashboard

Dans le champ message indiquer l’heure et le titre de l’alarme sous la forme suivante :  
heure;titre  
12:00;mon alarme

![](https://jeemate.fr/wp-content/uploads/2021/11/android-alarm-02-1024x52.png)

exemple depuis un scénario

  
  
  
 

## _Afficher URL :_

Saisir simplement l’url au format www.jeemate.fr dans le champ message.  
  
  
 

## _Show Screen :_

Vous permets d’allumer ou d’éteindre votre équipement Android.

Important : il faut autoriser Jeemate à faire un ScreenOnOff dans les paramètre android (Applis d’administration de l’appareil).

![](https://jeemate.fr/wp-content/uploads/2021/11/ShowScreen01.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ShowScreen02.jpg)

Pas le choix, il faut en assumer les risques.

  
  
  
 

## _TTS Speak :_

Plus d’infos à venir dans une section dédiée.

## _Envoyer des SMS :_

 Plus d’infos à venir dans une section dédiée.