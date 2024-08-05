---
unique-page-id: 2359791
description: Définition de l’objectif pour l’offre de référent - Documents Marketo - Documentation du produit
title: Définition de l’objectif pour l’offre de référent
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# Définition de l’objectif pour l’offre de référent {#specify-goal-for-referral-offer}

Lorsque vous [créez une offre de référence](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), vous devez définir l’objectif d’exécution. L’objectif peut être défini par l’activité de la personne sur la page web, comme les visites ou les inscriptions. Vous pouvez même utiliser un [événement JavaScript personnalisé](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

>[!IMPORTANT]
>
>Le 31 juillet 2024, nous avons commencé à abandonner cette fonctionnalité. Il n’est plus possible de créer de nouvelles ressources. Les ressources existantes continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Vous pouvez également utiliser un déclencheur de liste dynamique dans Marketo Engage pour attendre tout jalon, par exemple une opportunité créée pour la personne référencée.

Exemples d’objectifs :

* 10 visites référencées
* 5 inscriptions référencées
* 1 opportunité renvoyée créée
* 2 achats de commerce électronique référencés
* 5 participants au webinaire référencés

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Sélectionnez l’offre de référence, puis cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Dans l’éditeur d’offres de référence, accédez à **Paramètres de l’application** > **Détails de l’offre**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Sous **Paramètres**, choisissez un type d’événement dans la liste déroulante **Objectif d’exécution**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Si vous prévoyez d’utiliser l’étape de flux **Attribuer du crédit au référent**, vous devez sélectionner ici le type d’objectif d’exécution **Déclencheur de liste dynamique**.

* Visites référencées : les participants à l’offre obtiennent du crédit pour chaque visite d’un ami sur la page qui héberge votre offre.
* Abonnements différés : les participants à l’offre obtiennent du crédit pour chaque ami qui s’inscrit à l’offre.
* Déclencheur de liste dynamique : les participants à l’offre obtiennent du crédit pour chaque ami qui répond aux conditions d’un déclencheur [liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) dans une [campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Par exemple, vous pouvez utiliser un déclencheur qui se déclenche lorsqu’un prospect référencé s’inscrit à un webinaire.

* Événement JavaScript personnalisé : les participants à l’offre obtiennent du crédit pour chaque ami qui déclenche un événement JavaScript défini sur votre page. Voir [Script de conversion pour les événements personnalisés](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>De nouveaux filtres et déclencheurs sont disponibles dans les campagnes dynamiques pour surveiller l’activité sociale. Voir [Utilisation de déclencheurs et de filtres pour les activités sociales](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Ensuite, vous pouvez [sélectionner les emails d’inscription et d’exécution](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) à envoyer à partir de votre offre de parrainage.
