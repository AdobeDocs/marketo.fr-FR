---
unique-page-id: 557331
description: Découvrez comment trouver toutes les personnes à une étape de chiffre d’affaires. Utilisez le filtre d’étape de chiffre d’affaires pour créer une liste ou un segment.
title: Rechercher toutes les personnes présentes dans une étape de cycle de revenus
exl-id: aa5b30bf-96f1-4c1f-8170-86ba808e9705
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/-cODXA865GaIRdn34vnODbn7HCmp7Tf8J9OOOOOaswQ'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 8%
---
# Rechercher toutes les personnes présentes dans une étape de cycle de revenus {#find-all-people-in-a-revenue-stage}

>[!PREREQUISITES]
>
>[Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

## Rechercher tous les membres d’une étape de chiffre d’affaires spécifique {#find-all-members-of-a-specific-revenue-stage}

1. Dans une liste dynamique, cliquez sur l’onglet **[!UICONTROL Liste dynamique]**, recherchez le filtre **[!UICONTROL Étape de chiffre d’affaires]** et faites-le glisser dans la zone de travail.

   ![](assets/draginrevenuefilter.png)

1. Sélectionnez une **[!UICONTROL étape de chiffre d’affaires]**.

   ![](assets/two.jpg)

1. Accédez à l’onglet **[!UICONTROL Personnes]** pour afficher les résultats.

   ![](assets/peopleresults.jpg)

## Exécuter une étape de flux sur les membres d’une étape de revenus {#run-a-flow-step-on-the-members-of-a-revenue-stage}

Maintenant que vous savez quelles personnes se trouvent à quelles étapes du chiffre d’affaires, vous pouvez vous adresser directement à elles. En plus de choisir **[!UICONTROL Étape du chiffre d’affaires]** comme filtre de liste dynamique, vous pouvez également le choisir en tant que filtre « Si » dans le flux.

1. À l’étape de flux souhaitée, cliquez sur **[!UICONTROL Ajouter un choix]** et sélectionnez **[!UICONTROL Étape du chiffre d’affaires]** dans la liste déroulante.

   ![](assets/six.png)

   De là, vous pouvez choisir les membres qui sont affectés par l&#39;aspect de l&#39;étape de flux.
