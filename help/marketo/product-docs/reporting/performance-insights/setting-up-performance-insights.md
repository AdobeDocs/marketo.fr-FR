---
unique-page-id: 12981145
description: Configuration D’Informations Sur Les Performances - Documents Marketo - Documentation Du Produit
title: Configuration de Performance Insights
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 2%

---

# Configuration De [!UICONTROL Performances Insights] {#setting-up-performance-insights}

Suivez les étapes ci-dessous pour configurer MPI.

## Configuration de l’opportunité {#opportunity-setup}

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Cliquez sur **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Si vous n&#39;avez pas de RCA, vous devez sélectionner **[!UICONTROL Analyse de programme]** pour l&#39;étape 2.

1. Sous Attribution, cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/three-1.png)

1. Les Paramètres d’attribution s’affichent.

   ![](assets/four-2.png)

   Si l’attribution est explicite, assurez-vous que le rôle de contact de l’opportunité a été renseigné (soit via le point d’entrée du rôle d’opportunité, soit via l’intégration CRM).

   Si l’attribution est implicite, assurez-vous que le champ société du prospect/contact est identique au nom du compte de l’opportunité.

   >[!NOTE]
   >
   >Assurez-vous que les champs appropriés sont renseignés pour toutes les opportunités :
   >
   >* [!UICONTROL Montant de l’opportunité]
   >* [!UICONTROL Est Fermé]
   >* [!UICONTROL Est Gagné]
   >* [!UICONTROL  Date de création ] (peut ne pas être définie dans votre cas)
   >* [!UICONTROL Date de clôture] (peut ne pas être définie dans votre cas)
   >* [!UICONTROL  Type d’opportunité ]

## Configuration du programme {#program-setup}

Mettez à jour les coûts du programme pendant au moins 12 mois. Vous pouvez le faire manuellement ou à l’aide de l’API du programme. Dans cet exemple, nous le faisons manuellement.

1. Cliquez sur **[!UICONTROL Activités marketing]**.

   ![](assets/ma.png)

1. Recherchez et sélectionnez votre programme.

   ![](assets/select-program.png)

1. Cliquez sur l’onglet **[!UICONTROL Configuration]**.

   ![](assets/setup-tab.png)

1. Faites glisser **[!UICONTROL Coût de la période]** sur la zone de travail.

   ![](assets/period-cost.png)

1. Définissez le mois du programme sur au moins 12 mois, puis cliquez sur **[!UICONTROL Ok]**.

   ![](assets/set-period.png)

1. Définissez le coût de la période et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/set-cost.png)

Examinez ensuite le comportement des analyses pour indiquer si un canal particulier doit être inclus dans les analyses. Définissez le comportement d’Analytics (normal, inclusif, opérationnel).

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Cliquez sur **[!UICONTROL Balises]**.

   ![](assets/tags.png)

1. Cliquez sur **+** pour développer la liste Canal .

   ![](assets/channel.png)

1. Double-cliquez sur le canal de votre choix.

   ![](assets/channel-click.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Comportement d’Analytics]** et sélectionnez le comportement souhaité.

   ![](assets/edit-channel.png)

1. Définissez les critères de réussite.

   ![](assets/success.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/save.png)

## Lier le programme à la personne {#tie-the-program-to-the-person}

1. Assurez-vous que le Programme d’acquisition et la Date d’acquisition ont été définis pour chaque personne de votre base de données afin que l’attribution du premier contact fonctionne.
1. Assurez-vous que vos programmes définissent des états de succès pour vos salariés.

>[!NOTE]
>
>Les modifications apportées ne sont pas instantanées. Une période de nuit est nécessaire avant que les modifications ne prennent effet.
