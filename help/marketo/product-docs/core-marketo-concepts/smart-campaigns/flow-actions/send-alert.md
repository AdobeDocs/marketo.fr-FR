---
unique-page-id: 1146958
description: Envoyer une alerte - Documents Marketo - Documentation du produit
title: Envoyer une alerte
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 2%

---

# Envoyer une alerte {#send-alert}

Marketo Engage peut envoyer une alerte par courrier électronique contenant des informations personnelles à tout le monde, au propriétaire du commerce, à un partenaire ou à une autre personne. Utilisez l’étape de flux &quot;[!UICONTROL Envoyer une alerte]&quot;.

![](assets/send-alert-1.png)

1. Recherchez et sélectionnez l’email que vous souhaitez envoyer.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >Votre alerte par e-mail doit contenir toutes les informations d’en-tête et être à l’état **[!UICONTROL Approuvé]**.

1. Vous pouvez cliquer sur l’icône d’aperçu pour vous assurer que vous avez sélectionné l’email correct.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Veillez à utiliser le jeton &quot;[!UICONTROL Send Alert Info]&quot; dans votre email.

1. Sélectionnez le destinataire de l’alerte. Vous pouvez choisir [!UICONTROL Propriétaire des ventes] ou [!UICONTROL Propriétaire du compte].

   ![](assets/send-alert-4.png)

1. Vous pouvez éventuellement ajouter toute autre adresse électronique (séparée par une virgule ou un point-virgule).

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >Dans les campagnes de déclenchement, vous pouvez utiliser des jetons dans **[!UICONTROL To Other Emails]** tels que `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}` tant que les valeurs sont des adresses électroniques valides. Les jetons de **[!UICONTROL vers d’autres emails]** ne fonctionneront pas dans une campagne par lots.

>[!MORELIKETHIS]
>
>[Créer un email](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
