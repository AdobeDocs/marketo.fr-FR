---
unique-page-id: 1147322
description: Présentation de l'Activité et des personnes anonymes - Documents marketing - Documentation du produit
title: Présentation de l'Activité et des personnes anonymes
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Présentation de l&#39;Activité et des personnes anonymes {#understanding-anonymous-activity-and-people}

La première fois qu’une personne visite un Marketo [l `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) (ou une page de votre site Web qui comporte le code [de suivi](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin), Marketo crée une **activité* anonyme *et utilise un cookie de navigateur pour le suivre. Une fois identifié, il devient une personne et l&#39;historique associé au cookie de son navigateur est fusionné.

**Une activité anonyme** est créée lorsqu’une personne :

* Visite votre landing page Marketing pour la première fois.

* Visite une page de votre site qui est suivie [par](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin.

* Cliquez sur le lien [Vue en tant que page](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Web dans un courrier électronique de Marketo.

>[!NOTE]
>
>Contrairement à d&#39;autres liens dans les courriers électroniques de Marketo, la [Vue en tant que page](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Web n&#39;est pas suivie en tant que clic électronique.

Une activité anonyme est fusionnée en une personne nouvelle ou existante lorsqu’une personne :

* Cliquez sur un [lien dans un courriel](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)marketing.
* Remplit un [formulaire](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)Marketo.
* Utilise l’API [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846) ou [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) de Marketo (pour les développeurs) pour associer une personne anonyme à un enregistrement connu.

Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents périphériques et navigateurs pour visiter votre site.

>[!NOTE]
>
>Lorsque des enregistrements anonymes sont fusionnés dans un enregistrement de personne nouveau ou existant, les valeurs de champ personnalisé **ne sont pas** transférées.

