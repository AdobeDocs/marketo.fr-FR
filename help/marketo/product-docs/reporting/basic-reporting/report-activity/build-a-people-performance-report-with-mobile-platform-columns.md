---
unique-page-id: 2951220
description: Création d’un rapport sur les performances des personnes avec les colonnes de la plateforme mobile - Documents Marketo - Documentation du produit
title: Création d’un rapport sur les performances des personnes avec des colonnes Mobile Platform
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Création d’un rapport sur les performances des personnes avec des colonnes Mobile Platform {#build-a-people-performance-report-with-mobile-platform-columns}

Pour créer un rapport Performance des personnes avec des colonnes de plateforme mobile (iOS/Android), procédez comme suit.

## Création de listes dynamiques mobiles {#create-mobile-smart-lists}

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Choisissez un programme.

   ![](assets/two-1.png)

1. Sous **New**, sélectionnez **New Local Asset**.

   ![](assets/three-1.png)

1. Cliquez sur **Liste dynamique**.

   ![](assets/four-1.png)

1. Saisissez un nom et cliquez sur **Créer**.

   ![](assets/five-1.png)

1. Recherchez et faites glisser le filtre Courrier électronique ouvert dans la zone de travail.

   ![](assets/six-1.png)

1. Définissez Email sur **est n’importe quel**.

   ![](assets/seven.png)

1. Cliquez sur **Ajouter la contrainte** et sélectionnez **Plateforme**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Nous avons utilisé le filtre Courrier électronique ouvert dans cet exemple. Vous pouvez également utiliser le filtre Email cliqué , car il a la contrainte Platform .

1. Définissez Platform sur **iOS**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Au moins une personne doit avoir ouvert l’un de vos emails sur un appareil iOS pour que Marketo vous suggère de le trouver automatiquement. S’il ne s’affiche pas, vous pouvez le saisir manuellement et l’enregistrer.

   Créez maintenant une deuxième liste dynamique pour la plateforme &quot;Android&quot;. Une fois cela fait, passez à la section suivante.

## Création d’un rapport Performance des personnes {#create-a-people-performance-report}

1. Sous Activités marketing, sélectionnez le programme qui héberge vos listes dynamiques **iOS** et **Android**.

   ![](assets/ten.png)

1. Sous **New**, sélectionnez **New Local Asset**.

   ![](assets/eleven.png)

1. Cliquez sur **Report**.

   ![](assets/twelve.png)

1. Définissez le type sur **Performance des personnes**.

   ![](assets/thirteen.png)

1. Cliquez sur **Créer**.

   ![](assets/fourteen.png)

   Tu t&#39;en sors bien ! Passons à la section suivante.

## Ajout de listes dynamiques mobiles en tant que colonnes {#add-mobile-smart-lists-as-columns}

1. Dans le rapport que vous venez de créer, cliquez sur **Configuration**, puis faites glisser **Colonnes personnalisées** dans la zone de travail.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >Par défaut, le rapport Performance des personnes examine les 7 derniers jours. Vous pouvez modifier la période en double-cliquant dessus.

1. Recherchez et sélectionnez les listes dynamiques que vous avez créées précédemment et cliquez sur **Appliquer**.

   ![](assets/sixteen.png)

1. Cliquez sur **Rapport** pour exécuter le rapport et afficher vos données.

   ![](assets/seventeen.png)

   Plutôt cool, n&#39;est-ce pas ? C&#39;est joli !
