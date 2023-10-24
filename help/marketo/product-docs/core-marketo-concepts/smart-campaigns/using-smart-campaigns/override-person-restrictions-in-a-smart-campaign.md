---
unique-page-id: 1147066
description: Remplacement des restrictions de personne dans une campagne dynamique - Documents Marketo - Documentation du produit
title: Remplacement des restrictions de personne dans une campagne dynamique
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Remplacement des restrictions de personne dans une campagne dynamique {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage vous permet de définir le nombre maximal de personnes pouvant être qualifiées pour une campagne dynamique, ce qui vous permet d’éviter d’envoyer accidentellement par courrier électronique l’ensemble de votre base de données. Si vous voulez _override_ cette limite, voilà comment.

>[!PREREQUISITES]
>
>Veillez à [Activation des restrictions de personne pour les campagnes dynamiques](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} dans l’administration Marketo.

1. Dans **[!UICONTROL Activités marketing]**, accédez à votre campagne dynamique et cliquez sur **[!UICONTROL Planification]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Dans Paramètres de campagne dynamique, cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >La limite par défaut est celle définie dans Admin.

1. Saisissez une nouvelle limite et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   La campagne dynamique ne s’exécute pas si le nombre de personnes remplissant les critères dépasse la limite définie.

   >[!CAUTION]
   >
   >Soyez prudent avec cette fonctionnalité afin de ne pas inclure trop de personnes par inadvertance.
