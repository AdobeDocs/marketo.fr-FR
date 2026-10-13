---
unique-page-id: 2360243
description: Définissez un nombre maximal de personnes pouvant être qualifiées pour une campagne intelligente afin d’éviter d’envoyer accidentellement par e-mail l’ensemble de la base de données.
title: Activer les restrictions de personne pour les campagnes intelligentes
exl-id: 45bdaf3f-874c-493f-9746-440f7703713c
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/6VwkOwN9nTqSyNcXvzyggPTk0Um5x1GPXIp2DBf2kww'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 11%
---
# Activer les restrictions de personne pour les campagnes intelligentes {#enable-person-restrictions-for-smart-campaigns}

Marketo offre une fonctionnalité permettant de limiter le nombre _maximum_ de personnes pouvant se qualifier pour une campagne intelligente. Cela évite d’envoyer accidentellement par e-mail l’ensemble de votre base de données.

>[!NOTE]
>
>**Autorisations d’administration requises**

>[!CAUTION]
>
>Cela s’applique uniquement aux campagnes par lots et aux programmes de messagerie.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-1.png)

1. Cliquez sur **[!UICONTROL Campagne intelligente]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-2.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-3.png)

   >[!CAUTION]
   >
   >Si le nombre de personnes pouvant être exécutées par une campagne intelligente dépasse la limite définie, l’opération ne sera pas exécutée du tout.

1. Saisissez une limite et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-4.png)

   >[!TIP]
   >
   >Désactivez cette fonctionnalité en laissant ce champ vide.

   >[!CAUTION]
   >
   >Cette limite est appliquée à toutes les campagnes intelligentes, mais peut être remplacée au niveau de la campagne. Découvrez comment [remplacer les restrictions de personne dans une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md).

>[!MORELIKETHIS]
>
>[Remplacer les restrictions de personne dans une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)
