---
unique-page-id: 1146958
description: Découvrez comment envoyer une alerte dans une étape de flux de campagne intelligente. Avertir les utilisateurs lorsqu’une personne entre dans le flux ou répond aux critères.
title: Envoyer une alerte
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 2%

---

# Envoyer une alerte {#send-alert}

Marketo Engage peut envoyer une alerte par e-mail contenant des informations personnelles à n’importe qui : le commercial, un partenaire ou quelqu’un d’autre. Utilisez l’étape de flux « [!UICONTROL &#x200B; Envoyer l’alerte &#x200B;] ».

![](assets/send-alert-1.png)

1. Recherchez et sélectionnez l’e-mail à envoyer.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >Votre alerte par e-mail doit contenir toutes les informations d’en-tête et présenter le statut **[!UICONTROL Approuvé]**.

1. Vous pouvez cliquer sur l’icône d’aperçu pour vous assurer d’avoir sélectionné l’e-mail approprié.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Veillez à utiliser le jeton « [!UICONTROL &#x200B; Envoyer les informations d’alerte &#x200B;] » dans votre e-mail.

1. Sélectionnez le destinataire de l’alerte. Vous pouvez choisir [!UICONTROL Propriétaire de ventes] ou [!UICONTROL Propriétaire de compte].

   ![](assets/send-alert-4.png)

1. Vous pouvez éventuellement ajouter d’autres adresses e-mail de votre choix (séparées par une virgule ou un point-virgule).

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >Dans les campagnes de déclenchement, vous pouvez utiliser des jetons dans **[!UICONTROL Vers d’autres e-mails]** tels que `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}`, tant que les valeurs sont des adresses e-mail valides. Les jetons dans **[!UICONTROL Vers d’autres e-mails]** ne fonctionneront pas dans une campagne par lots.

>[!MORELIKETHIS]
>
>[Créer un e-mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
