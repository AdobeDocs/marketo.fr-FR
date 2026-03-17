---
unique-page-id: 1147066
description: Découvrez comment remplacer les restrictions de personne dans une campagne dynamique. Autoriser les utilisateurs à exécuter même s’ils atteignent les limites de communication.
title: Ignorer les restrictions de personnes dans une campagne intelligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 9%

---

# Ignorer les restrictions de personnes dans une campagne intelligente {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage vous permet de définir le nombre maximal de personnes pouvant se qualifier pour une campagne dynamique. Vous pouvez ainsi éviter d’envoyer accidentellement par e-mail l’ensemble de votre base de données. Si vous souhaitez _contourner_ cette limite, procédez comme suit.

>[!PREREQUISITES]
>
>Veillez à [activer les restrictions de personne pour les campagnes intelligentes](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} dans Marketo Admin.

1. Dans **[!UICONTROL Activités marketing]**, accédez à votre campagne intelligente et cliquez sur **[!UICONTROL Planifier]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Dans les paramètres de campagne intelligente, cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >La limite par défaut est celle définie dans Admin.

1. Saisissez une nouvelle limite et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   La campagne intelligente ne s’exécute pas si le nombre de personnes remplissant les conditions requises dépasse la limite définie.

   >[!CAUTION]
   >
   >Faites attention avec cette fonctionnalité afin de ne pas inclure accidentellement trop de personnes.
