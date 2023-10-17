---
unique-page-id: 1146958
description: Envoyer une alerte - Documents Marketo - Documentation du produit
title: Envoyer une alerte
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# Envoyer une alerte {#send-alert}

## Vue d’ensemble {#overview}

Marketo peut envoyer une alerte par courrier électronique contenant des informations sur la personne de tout le monde, à tout le monde (propriétaire commercial, partenaire ou autre). Utilisez le[!UICONTROL Envoyer une alerte]&quot; étape de flux.

![](assets/one-1.png)

## Utilisation {#usage}

1. Recherchez et sélectionnez l’email que vous souhaitez envoyer.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Votre alerte par e-mail doit contenir toutes les informations d’en-tête et figurer dans la variable **[!UICONTROL Approuvé]** état.

1. Vous pouvez cliquer sur l’icône d’aperçu pour vous assurer que vous avez sélectionné l’email correct.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Veillez à utiliser le[!UICONTROL Envoyer les informations d’alerte]&quot; dans votre email.

1. Sélectionnez le destinataire de l’alerte. Vous pouvez choisir [!UICONTROL Propriétaire des ventes] ou [!UICONTROL Propriétaire du compte].

   ![](assets/four-2.png)

1. Vous pouvez éventuellement ajouter toute autre adresse électronique (séparée par une virgule ou un point-virgule).

   ![](assets/five.png)

   >[!TIP]
   >
   >Pour déclencher des campagnes, vous pouvez utiliser des jetons dans **[!UICONTROL À d’autres courriers électroniques]** par exemple `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}` tant que les valeurs sont des adresses électroniques valides. Jetons dans **[!UICONTROL À d’autres courriers électroniques]** ne fonctionnera pas dans une campagne par lots.

>[!MORELIKETHIS]
>
>[Créer un email](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
