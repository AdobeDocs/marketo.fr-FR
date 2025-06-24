---
unique-page-id: 2360181
description: Suivi des activités et des personnes anonymes - Documents Marketo - Documentation du produit
title: Suivi des activités et des personnes anonymes
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Suivi des activités et des personnes anonymes {#tracking-anonymous-activity-and-people}

La première fois qu’une personne visite une [page de destination](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) Marketo (ou une page de votre site Web comportant le [code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crée une _activité anonyme_ et utilise un cookie de navigateur pour la suivre. Une fois le visiteur identifié, il devient une personne et l’historique associé au cookie du navigateur est fusionné.

1. Une activité anonyme est créée lorsque quelqu’un :

   * Première visite de votre [page de destination](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) Marketo.
   * Visite une page de votre site qui a un [suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Clique sur le lien [Afficher en tant que page web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) dans un e-mail Marketo.

   >[!NOTE]
   >
   >Contrairement aux autres liens dans les e-mails Marketo, Afficher en tant que page web n&#39;est pas suivi comme un clic sur un e-mail.

   Une activité anonyme est fusionnée en une personne nouvelle ou existante lorsque quelqu’un :

   * Clique sur un [lien dans un email Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Remplit un [formulaire](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) Marketo.
   * Utilise l’API Marketo [API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/lead-database/leads) ou l’API [Munchkin](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) (pour les développeurs) pour associer une activité anonyme à un enregistrement connu.

   Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents appareils et navigateurs pour visiter votre site.

   >[!NOTE]
   >
   >Lorsque des enregistrements anonymes sont fusionnés dans un enregistrement de personne nouveau ou existant, les valeurs de champ personnalisé ne sont **transférées**

   >[!MORELIKETHIS]
   >
   >[Afficher des personnes ou des visiteurs anonymes dans des rapports web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
