---
unique-page-id: 1146958
description: Envoyer une alerte - Documents marketing - Documentation du produit
title: Envoyer une alerte
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Envoyer l&#39;alerte {#send-alert}

## Aperçu {#overview}

Marketo peut envoyer une alerte par courriel contenant des informations personnelles à n’importe qui - le vendeur, un partenaire ou quelqu’un d’autre. Utilisez l’étape de flux **Envoyer une alerte**.

![](assets/one-1.png)

## Utilisation {#usage}

1. Recherchez et sélectionnez le courriel à envoyer.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Votre alerte par courrier électronique doit contenir toutes les informations d’en-tête et être à l’état **Approuvé**.

1. Vous pouvez cliquer sur l’icône de prévisualisation pour vous assurer que vous avez sélectionné le courriel approprié.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Veillez à utiliser le jeton **Envoyer les informations d’alerte** dans votre courrier électronique.

1. Sélectionnez le destinataire d&#39;alerte. Vous pouvez sélectionner Propriétaire du compte ou Propriétaire du compte.

   ![](assets/four-2.png)

1. Vous pouvez éventuellement ajouter toute autre adresse électronique de votre choix (en la séparant par une virgule ou un point-virgule).

   ![](assets/five.png)

   >[!TIP]
   >
   >Dans les campagnes de déclenchement, vous pouvez utiliser des jetons dans **Autres adresses électroniques** telles que `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}` tant que les valeurs sont des adresses électroniques valides. Les jetons de **vers d’autres adresses électroniques** ne fonctionneront pas dans une campagne par lot.

C&#39;est tout ! Vous savez maintenant comment utiliser l’étape de flux **Envoyer une alerte**.

>[!MORELIKETHIS]
>
>[Créer un courriel](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
