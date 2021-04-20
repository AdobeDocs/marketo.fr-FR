---
title: override-person-restrictions-in-a-smart-campaign
description: Remplacer les restrictions de personne dans une Campaign dynamique
exl-id: efdd6c68-a95e-4b2a-9249-e2e1f550b628
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---

# Remplacer les restrictions de personne dans une Campaign dynamique

<br> 

Marketo vous permet de définir le nombre maximal de personnes pouvant bénéficier d’une campagne intelligente ; cela vous permet d’éviter d’envoyer par courrier électronique l’intégralité de votre base de données. Si vous voulez remplacer cette limite, voici comment.

>[!IMPORTANT]
>
>Veillez à [activer les restrictions de personne pour les campagnes intelligentes](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) dans Marketo [!UICONTROL Admin].

1. Recherchez votre campagne intelligente et cliquez sur **[!UICONTROL Planification]**.

   ![Image un](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Cliquez sur **[!UICONTROL Règles de qualification]**.

   ![Image 2](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >La limite par défaut est celle définie dans Admin.

1. En regard de **[!UICONTROL Abandonner la campagne si les pistes qualifiées dépassent]**, entrez une nouvelle limite.

   ![Image trois](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>La campagne intelligente ne s’exécute pas si le nombre de personnes admissibles dépasse la limite définie.

>[!CAUTION]
>
>Soyez prudent avec cette fonctionnalité afin de ne pas inclure accidentellement trop de personnes.
