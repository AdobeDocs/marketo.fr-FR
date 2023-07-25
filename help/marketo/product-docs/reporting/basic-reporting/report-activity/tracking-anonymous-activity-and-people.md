---
unique-page-id: 2360181
description: Suivi de l’activité anonyme et des personnes - Documents Marketo - Documentation du produit
title: Suivi de l’activité anonyme et des personnes
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Suivi de l’activité anonyme et des personnes {#tracking-anonymous-activity-and-people}

Première visite d’un visiteur dans Marketo [landing page](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (ou une page de votre site web qui contient la variable [Code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crée une _activité anonyme_ et utilise un cookie de navigateur pour en effectuer le suivi. Une fois le visiteur identifié, il devient une personne et l’historique associé au cookie du navigateur est fusionné.

1. Une activité anonyme est créée lorsqu&#39;une personne :

   * Visite de votre Marketo [landing page](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) la première fois.
   * Visite une page de votre site qui comporte [Tracking Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Cliquez sur le bouton [Afficher comme page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) dans un email Marketo.

   >[!NOTE]
   >
   >Contrairement aux autres liens des emails Marketo, l’option Afficher comme page web n’est pas suivie en tant que clic sur un email.

   Une activité anonyme est fusionnée en une nouvelle personne ou une personne existante lorsqu’une personne :

   * Cliquez sur un [lien dans un email Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Remplissage d’un Marketo [formulaire](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Utilise Marketo [API REST](https://developers.marketo.com/rest-api/lead-database/leads/) ou [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API (pour les développeurs) pour associer une activité anonyme à un enregistrement connu.

   Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents appareils et navigateurs pour consulter votre site.

   >[!NOTE]
   >
   >Lorsque des enregistrements anonymes sont fusionnés en un nouvel enregistrement de personne ou un enregistrement de personne existant, les valeurs de champ personnalisées sont **not** transférer.

   >[!MORELIKETHIS]
   >
   >[Affichage des personnes ou des visiteurs anonymes dans les rapports web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
