---
unique-page-id: 12981145
description: Découvrez comment configurer des informations sur les performances en configurant la configuration des opportunités, les coûts du programme, le comportement des analyses et les critères de réussite. Garantissez une attribution et un flux de données appropriés pour des rapports précis.
title: Configuration de Performance Insights
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
TQID: https://experienceleague.adobe.com/xH9HG3hKoUFG3428IngBYFG6n4W3k1Bd-baVI7WTMrE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2:
  - id: b9f06cb0-cdf7-4b83-a9d1-a701d132779b
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 331
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
   >* [!UICONTROL &#x200B; Date de création &#x200B;] (peut ne pas être définie dans votre cas)
   >* [!UICONTROL Date de clôture] (peut ne pas être définie dans votre cas)
   >* [!UICONTROL &#x200B; Type d’opportunité &#x200B;]

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
