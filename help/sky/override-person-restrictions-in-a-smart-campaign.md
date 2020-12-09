---
title: override-person-restrictions-in-a-smart-campaign
description: Remplacer les restrictions de personne dans une Campaign dynamique
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Remplacer les restrictions de personne dans une Campaign dynamique

<br> 

Marketo vous permet de définir le nombre maximal de personnes pouvant bénéficier d’une campagne intelligente ; cela vous permet d’éviter d’envoyer par courrier électronique l’intégralité de votre base de données. Si vous voulez remplacer cette limite, voici comment.

>[!IMPORTANT]
>
>Veillez à [activer les restrictions de personnes pour les campagnes](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) dynamiques dans [!UICONTROL l’administrateur]de Marketing Cloud.

1. Recherchez votre campagne intelligente et cliquez sur **[!UICONTROL Planifier]**.

   ![Image un](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Cliquez sur Règles **[!UICONTROL de]** qualification.

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
