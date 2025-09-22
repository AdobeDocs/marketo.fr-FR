---
unique-page-id: 2951220
description: Créer un rapport de performances des personnes avec des colonnes de plateforme mobile - Documents Marketo - Documentation du produit
title: Créer un rapport de performances des personnes avec des colonnes Mobile Platform
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 6%

---

# Créer un rapport de performances des personnes avec des colonnes Mobile Platform {#build-a-people-performance-report-with-mobile-platform-columns}

Pour créer un rapport de performances des personnes avec des colonnes de plateforme mobile (iOS/Android), procédez comme suit.

## Créer des listes dynamiques mobiles {#create-mobile-smart-lists}

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/ma.png)

1. Choisissez un programme.

   ![](assets/two-1.png)

1. Sous **[!UICONTROL Nouveau]**, sélectionnez **[!UICONTROL Nouvelle ressource locale]**.

   ![](assets/three-1.png)

1. Cliquez sur **[!UICONTROL Liste dynamique]**.

   ![](assets/four-1.png)

1. Saisissez un nom, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/five-1.png)

1. Recherchez le filtre [!UICONTROL E-mail ouvert] et faites-le glisser dans la zone de travail.

   ![](assets/six-1.png)

1. Définissez E-mail sur **[!UICONTROL est n’importe lequel]**.

   ![](assets/seven.png)

1. Cliquez sur **[!UICONTROL Ajouter une contrainte]** et sélectionnez **[!UICONTROL Plateforme]**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Dans cet exemple, nous avons utilisé le filtre [!UICONTROL E-mail ouvert]. Vous pouvez également utiliser le filtre [!UICONTROL E-mail cliqué], car il contient la contrainte Plateforme .

1. Définissez [!UICONTROL Platform] sur **[!UICONTROL iOS]**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Au moins une personne doit avoir ouvert l’un de vos e-mails sur un appareil iOS pour que les suggestions automatiques de Marketo puissent le retrouver. S’il n’apparaît pas, vous pouvez le saisir manuellement et l’enregistrer.

   Créez maintenant une deuxième liste dynamique pour la plateforme « Android ». Une fois que c&#39;est fait, passez à la section suivante.

## Créer un rapport de performances des personnes {#create-a-people-performance-report}

1. Sous Activités marketing, sélectionnez le programme qui héberge vos listes dynamiques **[!UICONTROL iOS]** et **[!UICONTROL Android]**.

   ![](assets/ten.png)

1. Sous **[!UICONTROL Nouveau]**, sélectionnez **[!UICONTROL Nouvelle ressource locale]**.

   ![](assets/eleven.png)

1. Cliquez sur **[!UICONTROL Rapport]**.

   ![](assets/twelve.png)

1. Définissez Type sur **[!UICONTROL Performances des personnes]**.

   ![](assets/thirteen.png)

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/fourteen.png)

   Vous vous en sortez bien ! Passez maintenant à la section suivante.

## Ajouter des listes dynamiques mobiles en tant que colonnes {#add-mobile-smart-lists-as-columns}

1. Dans le rapport que vous venez de créer, cliquez sur **[!UICONTROL Configuration]**, puis faites glisser **[!UICONTROL Colonnes personnalisées]** dans la zone de travail.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >Par défaut, le rapport Performances des personnes examine les 7 derniers jours. Vous pouvez modifier la période en double-cliquant dessus.

1. Recherchez et sélectionnez les listes dynamiques que vous avez créées précédemment et cliquez sur **[!UICONTROL Appliquer]**.

   ![](assets/sixteen.png)

1. Cliquez sur **[!UICONTROL Rapport]** pour exécuter le rapport et afficher vos données.

   ![](assets/seventeen.png)

   Plutôt cool, non ? Bien joué !
