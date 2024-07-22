---
unique-page-id: 2359793
description: Utilisation des courriers électroniques dans les promotions sociales - Documents Marketo - Documentation du produit
title: Utilisation des courriers électroniques dans les promotions de réseaux sociaux
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Utilisation des courriers électroniques dans les promotions de réseaux sociaux {#use-emails-in-social-promotions}

Lorsque vous créez une [offre de parrainage](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) ou un [tirage](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), vous pouvez inclure des courriers électroniques à envoyer lorsque la personne s’inscrit, et à nouveau lorsque la personne a gagné la récompense.

>[!TIP]
>
>Pour créer un email, voir [Envoyer un Email Blast](/help/marketo/getting-started/quick-wins/send-an-email.md).

Dans les emails, utilisez les jetons suivants :

* **E-mail d&#39;inscription** : utilisez **`{{social.Share Url}}`** pour envoyer à chaque personne participante un lien de partage personnalisé.

* **Adresse électronique d’exécution** : utilisez **`{{social.Promo Code}}`** pour envoyer à chaque gagnant un [code promotion](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>Avant de pouvoir ajouter un email à une application sociale, il doit être _opérationnel_ et _approuvé_. Voir [Modifier les paramètres d&#39;un email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Sélectionnez l’application et cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Dans l’éditeur d’applications sociales, accédez à **Paramètres de l’application > Détails de l’offre** (ou **Détails du tirage**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Ajoutez l&#39;email d&#39;inscription.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >L&#39;email de confirmation est envoyé automatiquement lorsqu&#39;une personne s&#39;inscrit.

1. Ajoutez l’email d’exécution.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. Dans une offre de parrainage, choisissez si l&#39;email d&#39;exécution est envoyé automatiquement ou manuellement.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>Dans un tirage, l’email d’exécution est toujours envoyé automatiquement lorsque vous [sélectionnez le gagnant](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Définition**
>
>* **auto sur l’objectif** : l’e-mail d’exécution est envoyé automatiquement lorsque chaque participant atteint l’objectif.
>* **envoyer manuellement** : une fois que les personnes commencent à atteindre l’objectif, revenez à votre offre de référence pour [envoyer manuellement l’email d’exécution](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>

>[!MORELIKETHIS]
>
>Ensuite, vous pouvez [choisir l&#39;URL de partage](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) ou, dans votre offre de parrainage, vous pouvez [télécharger les codes promotion](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) que vous enverrez.
