---
title: Notifications
description: 
published: true
date: 2022-03-31T19:40:37.543Z
tags: 
editor: markdown
dateCreated: 2022-03-13T19:32:26.432Z
---

2 types de notifications sont disponibles :

Notification générale avec laquelle vous pouvez envoyer des notifications et faire des Ask.

Notifications personnalisées qui vous permettent (pour le moment) seulement l’envoi de notifications.

La notification générale nécessite une configuration dans le champ titre.

Les notifications personnalisées sont plus simples à mettre en œuvre.

Avant tout, il est important d’activer les notifications dans l’application Jeemate.  
 

![](https://jeemate.fr/wp-content/uploads/2021/11/IMG_20211105_220431-1024x713.jpg)

Ici vous devez activer les notifications.  
Vous pouvez aussi les passer en mode vocal, dans ce cas elles seront lues lors de leur ouverture.  
En fonction de vos préférences, régler plus ou moins la rapidité de lecture.

Suivant votre appareil, il vous sera sans doute nécessaire d’effectuer des réglages Système et de configurer vos différents types de notifications :

![](https://jeemate.fr/wp-content/uploads/2021/11/Alerte01.jpg)

  
  
 

_Notification générale :_

La commande (N) Notif Général est créée automatiquement lors de la création de votre équipement.

![](https://jeemate.fr/wp-content/uploads/2021/11/Notif01.png)

Vous pourrez utiliser celle-ci de la plus simple des façons, jusqu’à(s) des personnalisations plus poussées.

Commençons par une notification classique :

![](https://jeemate.fr/wp-content/uploads/2021/11/Notif02-1024x63.png)

Dans le champ titre, il vous est possible de configurer différents aspects de votre notification.

**Il est important de respecter les points suivants lors de la personnalisation des notifications:**

-   respecter la casse (caractères en majuscules ou en minuscules)
-   séparer les paramètres avec ;; (cf exemples ci-dessous)

| **fonction** | **exemple** | **default** |
| --- | --- | --- |
| title | title=mon test des notifications. |     |
| customIcon | customIcon=<i class=’fas fa-user’></i>  <br>customIcon=fas fa-user  <br>  <br>les 2 sont possibles, liste d’icônes ici : [_Font Awesome_](https://fontawesome.com/) | Ellipsis H |
| iconColor | iconColor=00FF00 | vert (00ff00) |
| groupKey | groupKey=TEST  <br>  <br>vous permet de classer vos notifications |     |
| channelKey | channelKey=jeemateMax  <br>  <br>Au choix jeemateMax, jeemateHigh, jeemateDefault, jeemateMin  <br>Sur votre système, vous pourrez en fonction de la puissance des notifications mettre des sons différents. | jeemateMax |
| bigPicture | bigPicture=https://static.dw.com/image/49519617\_303.jpg  <br>  <br>Ajouter une image à votre message. |     |
| notificationLayout | Valeurs possibles: Default, BigPicture, BigText, Inbox, ProgressBar, MediaPlayer  <br>  <br>Personnalise la notification dans le centre de notifications système. | Default |
| largeIcon | largeIcon=https://jeemate.fr/wp-content/webp-express/webp-images/uploads/2021/07/cropped-splash-40×40.png.webp  <br>  <br>ceci ajoute une icône à droite du texte |     |
| backgroungColor | backgroundColor=0xff0000 (rouge)  <br>  <br>L’icône dans le centre de notifications système sera sur fond rouge |     |
|     |     |     |

Exemple avec un scénario de test :

Dans Jeedom, créez un nouveau scénario et importez le template suivant (enlevez l’extension txt)

[_TestNotifJeemate.json_Télécharger](https://jeemate.fr/wp-content/uploads/2021/11/TestNotifJeemate.json-1.txt)

![](https://jeemate.fr/wp-content/uploads/2021/11/Template-1024x182.png)

![](https://jeemate.fr/wp-content/uploads/2021/11/template2-1024x202.png)

1 – Importer le fichier template que vous venez de télécharger.  
2 – Sélectionner le.  
3 – Choisir la commande Notifications Général de votre Jeemate.  
4 – Appliquer les changement.

Le scénario est prêt à être utilisé, il envoie 7 notifications avec à chaque fois une commande de personnalisation différente en plus.

1 – Pour débuter seulement le titre en gras.

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotifJ-7-1024x265.jpg)

Notification Jeemate

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotif-2-1024x296.jpg)

Notification Système

2 – Personnalisation de la couleur et de l’icône dans la bulle.

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotifJ-6-1024x307.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotif-3-1024x298.jpg)

3 – Ajout d’un smiley et modification de la couleur du texte.  
Suivant les versions de Jeedom, le champ titre peut ne pas accepter les smileys, passez par un tag pour contourner le soucis.

L’emoji peut être saisi selon différents formats.  
L’exemple ci-dessous est au format PHP & Ruby: \\u suivi de l’emoji 26C4 entre crochet. \\u{26c4}  
Liste d’emojis ici : [_https://www.w3schools.com/charsets/ref\_emoji\_smileys.asp_](https://www.w3schools.com/charsets/ref_emoji_smileys.asp)  
 

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotifJ-4-1024x256.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotif-4-1024x300.jpg)

4 – Ajout d’une image dans le centre de notifications de Jeemate.

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotifJ-3-1024x530.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotif-5-1024x289.jpg)

5 – Rendre visible cette même image dans le centre de notifications du système.

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotifJ-5-1024x551.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotif-6-1024x763.jpg)

6 – Personnalisation de l’icône qui se trouve à droite du texte dans le centre de notifications système.

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotifJ-1-1024x560.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotif-7-1024x762.jpg)

7 – Personnalisation de l’icône Jeemate dans le centre de notifications système.

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotifJ-2-1024x576.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ScenarioNotif-1-1024x758.jpg)

_Notifications personnalisées_ :

Les notifications personnalisées sont à configurer dans l’onglet Notification du plugin Jeemate.

![](https://jeemate.fr/wp-content/uploads/2021/11/NotifPerso01-resize-1024x191.png)

![](https://jeemate.fr/wp-content/uploads/2021/11/NotifPerso02-resize.png)

Nom : celui qui vous permettra de retrouver la commande, elle sera sous la forme (N) votre nom  
Icône : sélectionner l’icône qui sera affiché dans le centre de notifications Jeemate.  
Couleur de l’icône : la couleur que prend la bulle de l’icône dans le centre de notifications Jeemate.  
Groupe de notifications : Si vous voulez classer vos notifications.  
URL d’une vidéo :  
URL d’une image :  
Puissance de notification : Correspond aux différents types de notifications acceptés par votre mobile  
Design : Sélectionner en fonction du type de notification que vous souhaitez recevoir.

**Une fois que vous avez configuré un type de notifications, vous devez la sauvegarder.**  
**Une fois cela fait, vous la retrouverez dans votre onglet notifications et il vous sera possible de l’éditer ou de la supprimer.**

Voici un exemple sur une notification Alerte, ici on choisit une couleur rouge et un icône explicite. On la classe dans un groupe Alerte et on met la puissance Max.

![](https://jeemate.fr/wp-content/uploads/2021/11/NotifPerso03-1-1024x105.png)

Avant de pouvoir utiliser votre notification, il est important d’ouvrir l’équipement (smartphone ou tablette) dans le plugin Jeemate et de faire un click sur sauvegarder, cela afin d’y remonter la nouvelle commande créée.  
  
A savoir que lorsque vous créez un nouvel équipement, toutes les notifications présentes dans l’onglet Notification seront automatiquement ajoutées.

![](https://jeemate.fr/wp-content/uploads/2021/11/NotifPerso04-1024x143.png)

Maintenant, vous pouvez utiliser cette notification dans vos scénarios d’alerte.

![](https://jeemate.fr/wp-content/uploads/2021/11/NotifPerso05-1024x64.png)

![](https://jeemate.fr/wp-content/uploads/2021/11/Alerte02.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/Alerte03.jpg)

_Ask :_

Avec des scénarios et commandes ASK, il vous est possible de « dialoguer » avec votre Jeedom. Votre scénario vous pose une question, suivant la réponse, vous effectuez des commandes différentes.  
Avec la commande de notification générale, il vous est possible de gérer ces scénarios avec Jeemate.  
  
Exemple d’un scénario ASK simple et de l’affichage de celui-ci soit dans le centre de notifications système, soit dans le centre de notifications Jeemate.

![](https://jeemate.fr/wp-content/uploads/2021/11/Scenario.png)

![](https://jeemate.fr/wp-content/uploads/2021/11/ASK-2-975x1024.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ASK-3-988x1024.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ASK-5-1024x383.jpg)

Il vous est possible de laisser le champ réponse vide, dans ce cas Jeemate attendra une réponse écrite. Vous aurez donc ceci comme notification :

![](https://jeemate.fr/wp-content/uploads/2021/11/ASK-6-1024x383.jpg)

![](https://jeemate.fr/wp-content/uploads/2021/11/ASK-1-1024x383.jpg)

Scénario de test Ask avec réponse enregistré et réponse libre.  
  
Question avec 3 réponses = bonne réponse = fin  
Question avec 3 réponses = mauvaise réponse = question avec réponse libre  
  
 

[_TestAskJeemate.json_Télécharger](https://jeemate.fr/wp-content/uploads/2021/11/TestAskJeemate.json.txt)

A vous de jouer !  
En cas de soucis, venez nous en parler sur Discord et n’oubliez pas, afin que l’on puisse au mieux vous aider, de nous préciser :  
  
Système et version  
Version de Jeemate  
Version du plugin  
Version de Jeedom  
  
Ici les tests ont été réalisés sur les systèmes suivants :  
  
Xiaomi mi11 / Android 11, Miui 12.5.7 / Jeemate app 0.9.10+96 / Plugin 2021-11-12 22:51:32 / Jeedom beta 4.2.5  
  
Pocophone F1 / Android 10, Miui 11.0.9/ Jeemate app 0.9.10+96 / Plugin 2021-11-12 22:51:32 / Jeedom beta 4.2.5  
  
Honor 8 / Android 7, EMUI 5.0.1/ Jeemate app 0.9.10+96 / Plugin 2021-11-12 22:51:32 / Jeedom beta 4.2.5  
(backgroundColor n’est pas pris en compte)  
  
iphone 11 / iOS 15.0 / jeemate app : 0.9.10+95 / jeemate plugin : 2021-11-12 22:51:35 / jeedom beta 4.2.5  
  
Iphone 6 / iOS 12.5.5/ Jeemate app 0.9.10+96 / Plugin 2021-11-12 22:51:32 / Jeedom beta 4.2.5  
Si Jeemate est ouvert en premier plan, tout arrive  
Si Jeemate est en arrière plan ou fermé, c’est plus aléatoire (utilisez les notifications système)