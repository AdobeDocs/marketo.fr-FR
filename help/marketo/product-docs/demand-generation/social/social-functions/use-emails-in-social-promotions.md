---
unique-page-id: 2359793
description: Utiliser des courriers électroniques dans les promotions sociales - Documents marketing - Documentation du produit
title: Utiliser des courriers électroniques dans les promotions sociales
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# Utiliser des courriers électroniques dans les promotions sociales {#use-emails-in-social-promotions}

Lorsque vous créez une [offre de renvoi](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) ou un tirage [, vous pouvez inclure des courriers électroniques à envoyer lorsque la personne s&#39;inscrit, puis à nouveau lorsque la personne a gagné la récompense.](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)

>[!TIP]
>
>Pour créer un courrier électronique, voir [Envoyer un message électronique ](/help/marketo/getting-started/quick-wins/send-an-email.md).

Dans les courriels, utilisez les jetons suivants :

* **Courriel** d&#39;inscription : Utilisez  **`{{social.Share Url}}`** pour envoyer à chaque participant un lien de partage personnalisé.

* **Adresse électronique** d’exécution : Utilisez  **`{{social.Promo Code}}`** pour envoyer à chaque gagnant un code [ de ](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)promotion.

>[!PREREQUISITES]
>
>Avant de pouvoir ajouter un courrier électronique à une application sociale, il doit être _opérationnel_ et _approuvé_. Voir [Modifier les paramètres pour un courrier électronique](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Sélectionnez l’application, puis cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Dans l’éditeur d’applications sociales, accédez à **Paramètres de l’application > Détails de l’Offre** (ou **Détails des tirages**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Ajoutez le courrier électronique d’inscription.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >L&#39;e-mail de confirmation est envoyé automatiquement lorsqu&#39;une personne s&#39;inscrit.

1. Ajoutez le courrier électronique d’exécution.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. Dans une offre de référence, choisissez si le courrier électronique d’exécution est envoyé automatiquement ou manuellement.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>Lors d’un tirage, le courrier électronique d’exécution est toujours envoyé automatiquement lorsque vous [sélectionnez le gagnant](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Définition**
>
>* **auto sur objectif** : Le courrier électronique d’exécution est envoyé automatiquement lorsque chaque participant atteint l’objectif.
>* **envoi** manuel : Une fois que les personnes ont début d’atteindre l’objectif, retournez à votre offre de référence pour  [envoyer manuellement le courrier électronique](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) d’exécution.

>



>[!MORELIKETHIS]
>
>Vous pouvez ensuite [choisir l’URL de partage](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) ou, dans votre offre de référence, [télécharger les codes promotionnels](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) que vous enverrez.
