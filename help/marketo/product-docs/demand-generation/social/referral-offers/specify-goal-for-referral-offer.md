---
unique-page-id: 2359791
description: Définition de l’objectif pour l’Offre de référence - Documents marketing - Documentation du produit
title: Définition de l’objectif pour l’Offre de renvoi
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Spécifier l&#39;objectif pour l&#39;Offre de renvoi {#specify-goal-for-referral-offer}

Lorsque vous [créez une offre de référence](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), vous devez définir l&#39;objectif d&#39;exécution. L’objectif peut être défini par l’activité d’une personne sur la page Web, telle que les visites de page ou les abonnements. Vous pouvez même utiliser un [événement JavaScript personnalisé](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Vous pouvez également utiliser un déclencheur de liste dynamique dans Marketing pour attendre tout jalon, tel qu’une opportunité créée pour la personne référencée.

Exemples d’objectifs :

* 10 visites référencées
* 5 abonnements référencés
* 1 opportunité renvoyée créée
* 2 achats de commerce électronique référencés
* 5 participants webinaires référencés

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Sélectionnez l’offre de référence, puis cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Dans l’éditeur d’offres de référence, accédez à **Paramètres de l’application** > **Détails de l’Offre**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Sous **Paramètres**, choisissez un type d&#39;événement dans la liste déroulante **Objectif d’exécution**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Si vous prévoyez d&#39;utiliser l&#39;étape de flux **Attribuer du crédit au Parrain**, vous devez sélectionner **Déclencheur de Liste dynamique** comme type d&#39;objectif d&#39;exécution ici.

* Visites référencées : Les participants à l’Offre reçoivent du crédit pour chaque visite d’un ami à la page qui héberge votre offre.
* Abonnements référencés : Les participants à l&#39;Offre reçoivent du crédit pour chaque ami qui s&#39;inscrit à l&#39;offre.
* Déclencheur de Liste intelligente : Les participants à l&#39;Offre reçoivent le crédit de chaque ami qui répond aux conditions d&#39;un déclencheur [liste intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) dans une [campagne intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Par exemple, vous pouvez utiliser un déclencheur qui se déclenche lorsqu’une prospect référencée se connecte à un webinaire.

* Événement JavaScript personnalisé : Les participants à l’Offre reçoivent du crédit pour chaque ami qui déclenche un événement JavaScript défini sur votre page. Voir [Script de conversion pour Événements personnalisés](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>De nouveaux filtres et déclencheurs sont disponibles dans les campagnes dynamiques pour surveiller l’activité sociale. Voir [utilisation de déclencheurs et de filtres pour les activités sociales](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Vous pouvez ensuite [sélectionner les courriels d&#39;inscription et d&#39;exécution](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) à envoyer à partir de votre offre de référence.
