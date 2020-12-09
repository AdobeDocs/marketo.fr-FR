---
unique-page-id: 1146958
description: Envoyer une alerte - Documents marketing - Documentation du produit
title: Envoyer une alerte
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# Envoyer une alerte {#send-alert}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Présentation {#overview}

Marketo peut envoyer une alerte par courriel contenant des informations personnelles à n’importe qui - le vendeur, un partenaire ou quelqu’un d’autre. Utilisez l’étape de flux **Envoyer une alerte** .

![](assets/one-1.png)

## Utilisation {#usage}

1. Recherchez et sélectionnez le courriel à envoyer.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >Votre alerte par courrier électronique doit contenir toutes les informations d’en-tête et être à l’état **Approuvé** .

1. Vous pouvez cliquer sur l’icône de prévisualisation pour vous assurer que vous avez sélectionné le courriel approprié.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >Veillez à utiliser le jeton **Envoyer les informations** d&#39;alerte dans votre courrier électronique.

1. Sélectionnez le destinataire d&#39;alerte. Vous pouvez sélectionner Propriétaire du compte ou Propriétaire du compte.

   ![](assets/four-2.png)

1. Vous pouvez éventuellement ajouter toute autre adresse électronique de votre choix (en la séparant par une virgule ou un point-virgule).

   ![](assets/five.png)

   >[!TIP]
   >
   >Dans les campagnes de déclenchement, vous pouvez utiliser des jetons dans **À d’autres courriels** , tels que `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}` aussi longtemps que les valeurs sont des adresses électroniques valides. Les jetons **à d’autres courriels** ne fonctionneront pas dans une campagne par lot.

C&#39;est tout ! Vous savez maintenant comment utiliser l’étape de flux **Envoyer une alerte** .

>[!MORELIKETHIS]
>
>[Créer un courriel](../../../../product-docs/email-marketing/general/creating-an-email/create-an-email.md)

