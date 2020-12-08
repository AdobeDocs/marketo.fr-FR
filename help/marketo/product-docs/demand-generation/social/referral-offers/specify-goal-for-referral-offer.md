---
unique-page-id: 2359791
description: Définition de l’objectif pour l’Offre de référence - Documents marketing - Documentation du produit
title: Définition de l’objectif pour l’Offre de renvoi
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Définition de l’objectif pour l’Offre de renvoi {#specify-goal-for-referral-offer}

Lorsque vous [créez une offre](create-a-referral-offer.md)de référence, vous devez définir l’objectif d’exécution. L’objectif peut être défini par l’activité d’une personne sur la page Web, telle que les visites de page ou les abonnements. Vous pouvez même utiliser un événement [JavaScript](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)personnalisé.

Vous pouvez également utiliser un déclencheur [de liste](specify-goal-for-referral-offer.md) intelligente dans Marketo pour attendre tout jalon, tel qu’une opportunité créée pour la personne référencée.

Exemples d’objectifs :

* 10 visites référencées
* 5 abonnements référencés
* 1 opportunité renvoyée créée
* 2 achats de commerce électronique référencés
* 5 participants webinaires référencés

1. Accédez à Activités **** marketing.

   ![](assets/ma.png)

1. Sélectionnez l’offre de référence, puis cliquez sur **Modifier le brouillon.**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Dans l’éditeur d’offres de référence, accédez à Paramètres **de l’** application > Détails de l’ **Offre.**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Sous **Paramètres**, choisissez un type d&#39;événement dans la liste déroulante Objectif **d’** exécution.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Si vous prévoyez d&#39;utiliser l&#39;étape de flux **Donner du crédit au Parrain** , vous devez sélectionner Déclencheur de Liste **intelligente** comme type d&#39;objectif d&#39;exécution ici.

* Visites référencées : Les participants à l’Offre reçoivent du crédit pour chaque visite d’un ami à la page qui héberge votre offre.
* Abonnements référencés : Les participants à l&#39;Offre reçoivent du crédit pour chaque ami qui s&#39;inscrit à l&#39;offre.
* Déclencheur de Liste intelligente : Les participants à l’Offre reçoivent du crédit pour chaque ami qui répond aux conditions d’un déclencheur de liste [](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) intelligente dans une campagne [](http://docs.marketo.com/display/docs/smart+campaigns)intelligente. Par exemple, vous pouvez utiliser un déclencheur qui se déclenche lorsqu’une prospect référencée se connecte à un webinaire.

* Événement JavaScript personnalisé : Les participants à l’Offre reçoivent du crédit pour chaque ami qui déclenche un événement JavaScript défini sur votre page. Voir Script de [conversion pour Événements](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)personnalisés.

>[!NOTE]
>
>De nouveaux filtres et déclencheurs sont disponibles dans les campagnes dynamiques pour surveiller l’activité sociale. Voir [Utilisation de déclencheurs et de filtres pour les activités](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)sociales.

>[!NOTE]
>
>**Articles connexes**
>
>Vous pouvez ensuite [sélectionner les courriers électroniques](send-referral-offer-fulfillment-email.md) d’inscription et d’exécution à envoyer à partir de votre offre de référence.

