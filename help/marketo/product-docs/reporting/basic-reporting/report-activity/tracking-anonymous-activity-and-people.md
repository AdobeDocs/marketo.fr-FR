---
unique-page-id: 2360181
description: Découvrez le suivi des activités et des personnes anonymes dans Marketo Engage, y compris le suivi des activités et des personnes anonymes. Utilisez ce guide pour passer à l’étape suivante.
title: Suivi des activités et des personnes anonymes
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
TQID: https://experienceleague.adobe.com/BZakQFVtQystRyrlzo81s-p8N65LXHUJ2ZoSAzeTG6Q
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 8%

---

# Suivi des activités et des personnes anonymes {#tracking-anonymous-activity-and-people}

La première fois qu’une personne visite une [page de destination](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) Marketo (ou une page de votre site Web comportant le [code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crée une _activité anonyme_ et utilise un cookie de navigateur pour la suivre. Une fois le visiteur identifié, il devient une personne et l’historique associé au cookie du navigateur est fusionné.

1. Une activité anonyme est créée lorsque quelqu’un :

   * Première visite de votre [page de destination](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) Marketo.
   * Visite une page de votre site qui a un [suivi &#x200B;](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Clique sur le lien [Afficher en tant que page web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) dans un e-mail Marketo.

   >[!NOTE]
   >
   >Contrairement aux autres liens dans les e-mails Marketo, Afficher en tant que page web n&#39;est pas suivi comme un clic sur un e-mail.

   Une activité anonyme est fusionnée en une personne nouvelle ou existante lorsque quelqu’un :

   * Clique sur un [lien dans un email Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Remplit un [formulaire](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) Marketo.
   * Utilise l’API Marketo [API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) ou l’API [Munchkin](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) (pour les développeurs) pour associer une activité anonyme à un enregistrement connu.

   Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents appareils et navigateurs pour visiter votre site.

   >[!NOTE]
   >
   >Lorsque des enregistrements anonymes sont fusionnés dans un enregistrement de personne nouveau ou existant, les valeurs de champ personnalisé ne sont **transférées**

   >[!MORELIKETHIS]
   >
   >[Afficher des personnes ou des visiteurs anonymes dans des rapports web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
