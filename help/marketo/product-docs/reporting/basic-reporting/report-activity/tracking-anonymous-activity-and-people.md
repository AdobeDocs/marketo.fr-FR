---
unique-page-id: 2360181
description: Suivi des Activités et des personnes anonymes - Documentation sur le marketing - Documentation sur les produits
title: Suivi des Activités et des personnes anonymes
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Suivi des Activités et des personnes anonymes {#tracking-anonymous-activity-and-people}

Lors de la première visite d’un Marketo [landing page](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (ou d’une page de votre site Web qui comporte le [code de suivi Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crée une *activité* anonyme *et utilise un cookie de navigateur pour le suivre.* Une fois le visiteur identifié, il devient une personne et l&#39;historique associé au cookie du navigateur est fusionné.

1. Une activité anonyme est créée lorsqu’une personne :

   * Visite votre Marketo [landing page](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) pour la première fois.
   * Visite une page de votre site qui comporte [suivi Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Cliquez sur le lien [Vue en tant que page Web](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) dans un courrier électronique Marketo.

   >[!NOTE]
   >
   >Contrairement à d&#39;autres liens dans les courriers électroniques de Marketo, la Vue en tant que page Web n&#39;est pas suivie en tant que clic électronique.

   Une activité anonyme est fusionnée en une personne nouvelle ou existante lorsqu’une personne :

   * Cliquez sur un lien [dans un courrier électronique Marketo](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Remplit un formulaire Marketo [a1/>.](https://docs.marketo.com/display/docs/forms)
   * Utilise l&#39;API [REST de Marketo](https://developers.marketo.com/rest-api/lead-database/leads/) ou [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) (pour les développeurs) pour associer une activité anonyme à un enregistrement connu.

   Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents périphériques et navigateurs pour visiter votre site.

   >[!NOTE]
   >
   >Lorsque des enregistrements anonymes sont fusionnés dans un enregistrement de personne nouveau ou existant, les valeurs de champ personnalisé **ne sont** pas transférées.

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [Affichage de personnes ou de Visiteurs anonymes dans les rapports Web](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**Plongée profonde**
   >
   >
   >En savoir plus sur [Rapports de base](https://docs.marketo.com/display/docs/basic+reporting).

