---
unique-page-id: 2360181
description: Suivi des personnes et des activités anonymes - Documents Marketo - Documentation du produit
title: Suivi de l’activité anonyme et des personnes
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Suivi de l’activité anonyme et des personnes {#tracking-anonymous-activity-and-people}

La première fois qu’une personne visite une [landing page](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) Marketo (ou une page de votre site web qui comporte le [ code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crée une _activité anonyme_ et utilise un cookie de navigateur pour en effectuer le suivi. Une fois le visiteur identifié, il devient une personne et l’historique associé au cookie du navigateur est fusionné.

1. Une activité anonyme est créée lorsqu&#39;une personne :

   * Visite la première [landing page](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) de Marketo.
   * Visite une page de votre site qui a le [suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Clique sur le lien [Afficher comme page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) dans un courrier électronique Marketo.

   >[!NOTE]
   >
   >Contrairement à d’autres liens dans les emails Marketo, l’option Afficher comme page web n’est pas suivie en tant que clic sur un email.

   Une activité anonyme est fusionnée en une nouvelle personne ou une personne existante lorsqu’une personne :

   * Clique sur un lien [dans un email Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Remplit un Marketo [form](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Utilise l’ [API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/lead-database/leads) ou l’ [ API Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking) de Marketo (pour les développeurs) pour associer une activité anonyme à un enregistrement connu.

   Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents appareils et navigateurs pour consulter votre site.

   >[!NOTE]
   >
   >Lorsque des enregistrements anonymes sont fusionnés en un nouvel enregistrement de personne ou un enregistrement de personne existant, les valeurs de champ personnalisé **et non** sont transférées.

   >[!MORELIKETHIS]
   >
   >[ Afficher des personnes ou des visiteurs anonymes dans les rapports Web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
