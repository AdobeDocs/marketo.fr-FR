---
unique-page-id: 2951220
description: Création d'un rapport sur les performances des personnes avec les colonnes des plateformes mobiles - Documents marketing - Documentation sur les produits
title: Création d’un rapport sur les performances des personnes avec des colonnes de plateformes mobiles
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---


# Création d’un rapport sur les performances des personnes avec des colonnes de plateformes mobiles {#build-a-people-performance-report-with-mobile-platform-columns}

Pour créer un rapport sur les performances des personnes avec des colonnes de plateformes mobiles (iOS/Android), procédez comme suit.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Création de Listes mobiles dynamiques {#create-mobile-smart-lists}

1. Accédez à Activités **** marketing.

   ![](assets/ma.png)

1. Choisissez un programme.

   ![](assets/two-1.png)

1. Sous **Nouveau**, sélectionnez **Nouveau fichier** local.

   ![](assets/three-1.png)

1. Cliquez sur Liste **** intelligente.

   ![](assets/four-1.png)

1. Saisissez un nom, puis cliquez sur **Créer**.

   ![](assets/five-1.png)

1. Recherchez et faites glisser le filtre Courrier électronique ouvert dans le canevas.

   ![](assets/six-1.png)

1. Définissez Courriel sur **est n’importe quel**.

   ![](assets/seven.png)

1. Cliquez sur **Ajouter la contrainte** et sélectionnez **Plateforme**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Nous avons utilisé le filtre Courrier électronique ouvert dans cet exemple. Vous pouvez également utiliser le filtre Courrier électronique cliqué, car il comporte la contrainte Plateforme.

1. Définissez la plate-forme sur **iOS**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Au moins une personne doit avoir ouvert l’un de vos courriels sur un périphérique iOS pour que Marketo propose automatiquement de le trouver. S’il ne s’affiche pas, vous pouvez le saisir manuellement et l’enregistrer.

   Créez maintenant une seconde liste intelligente pour la plate-forme &quot;Android&quot;. Une fois cela fait, passez à la section suivante.

## Création d’un rapport sur les performances des personnes {#create-a-people-performance-report}

1. Sous Activités marketing, sélectionnez le programme qui héberge vos listes dynamiques **iOS** et **Android** .

   ![](assets/ten.png)

1. Sous **Nouveau**, sélectionnez **Nouveau fichier** local.

   ![](assets/eleven.png)

1. Cliquez sur **Rapport**.

   ![](assets/twelve.png)

1. Définissez le type sur Performance **des** personnes.

   ![](assets/thirteen.png)

1. Cliquez sur **Créer**.

   ![](assets/fourteen.png)

   Tu te débrouilles bien ! Passons maintenant à la section suivante.

## Ajouter les Listes dynamiques mobiles en tant que colonnes {#add-mobile-smart-lists-as-columns}

1. Dans le rapport que vous venez de créer, cliquez sur **Configuration**, puis faites glisser des colonnes **** personnalisées dans le canevas.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >Par défaut, le rapport Performance des personnes examine les 7 derniers jours. Vous pouvez modifier la période en cliquant sur celle-ci par doublon.

1. Recherchez et sélectionnez les listes dynamiques que vous avez créées précédemment, puis cliquez sur **Appliquer**.

   ![](assets/sixteen.png)

1. Cliquez sur **Rapport** pour exécuter le rapport et afficher vos données.

   ![](assets/seventeen.png)

   Plutôt cool, non ? Bien joué !

