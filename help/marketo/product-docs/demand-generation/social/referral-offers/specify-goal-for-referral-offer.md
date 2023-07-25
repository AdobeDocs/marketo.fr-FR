---
unique-page-id: 2359791
description: Définition de l’objectif pour l’offre de référent - Documents Marketo - Documentation du produit
title: Définition de l’objectif pour l’offre de référent
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Définition de l’objectif pour l’offre de référent {#specify-goal-for-referral-offer}

Lorsque vous [créer une offre de référence](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), vous devez définir l’objectif d’exécution. L’objectif peut être défini par l’activité de la personne sur la page web, comme les visites ou les inscriptions. Vous pouvez même utiliser une [événement JavaScript personnalisé](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Vous pouvez également utiliser un déclencheur de liste dynamique dans Marketo pour attendre tout jalon, comme une opportunité créée pour la personne référencée.

Exemples d’objectifs :

* 10 visites référencées
* 5 inscriptions référencées
* 1 opportunité référencée créée
* 2 achats de commerce électronique référencés
* 5 participants au webinaire référencés

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Sélectionnez l’offre de parrainage, puis cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Dans l&#39;éditeur d&#39;offres de parrainage, accédez à **Paramètres de l’application** > **Détails de l’offre**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Sous **Paramètres**, choisissez un type d’événement dans la variable **Objectif d’exécution** menu déroulant.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Si vous prévoyez d’utiliser la variable **Attribuer du crédit au référent** étape de flux, vous devez sélectionner **Déclencheur de liste dynamique** comme type d’objectif d’exécution ici.

* Visites référencées : Les participants à l’offre obtiennent du crédit pour chaque visite d’un ami sur la page hébergeant votre offre.
* Signatures référencées : Les participants à l’offre reçoivent du crédit pour chaque ami qui s’inscrit à l’offre.
* Smart List Trigger : Les participants à l’offre obtiennent du crédit pour chaque ami qui remplit les conditions d’un [liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) déclencheur dans un [campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Par exemple, vous pouvez utiliser un déclencheur qui se déclenche lorsqu’un prospect référencé s’inscrit à un webinaire.

* Événement JavaScript personnalisé : Les participants à l’offre obtiennent du crédit pour chaque ami qui déclenche un événement JavaScript défini sur votre page. Voir [Script de conversion pour les événements personnalisés](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>De nouveaux filtres et déclencheurs sont disponibles dans les campagnes dynamiques pour surveiller l’activité sociale. Voir [utiliser des déclencheurs et des filtres pour les activités sociales ;](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Ensuite, vous pouvez [sélectionner les emails d’inscription et d’exécution ;](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) pour envoyer à partir de votre offre de parrainage.
