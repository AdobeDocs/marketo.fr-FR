---
unique-page-id: 1147322
description: Présentation de l'Activité et des personnes anonymes - Documents Marketo - Documentation du produit
title: Présentation de l'Activité et des personnes anonymes
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Présentation de l&#39;Activité anonyme et des personnes {#understanding-anonymous-activity-and-people}

Lors de la première visite d’un landing page Marketo (ou d’une page de votre site Web contenant le [code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crée une _activité anonyme_ et utilise un cookie de navigateur pour effectuer le suivi. Une fois identifié, il devient une personne et l&#39;historique associé au cookie de son navigateur est fusionné.

**Une** activité anonyme est créée lorsqu’une personne :

* Visite votre landing page Marketo la première fois.
* Visite une page de votre site qui comporte [suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Cliquez sur le lien [Vue en tant que page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) dans un courrier électronique Marketo.

>[!NOTE]
>
>Contrairement aux autres liens des courriers électroniques Marketo, [la Vue en tant que page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) n&#39;est pas suivie en tant que clic électronique.

Une activité anonyme est fusionnée en une personne nouvelle ou existante lorsqu’une personne :

* Cliquez sur un lien [dans un courrier électronique Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Remplit un Marketo [Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Utilise l&#39;API Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) ou [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) (pour les développeurs) pour associer une personne anonyme à un enregistrement connu.

Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents périphériques et navigateurs pour visiter votre site.

>[!NOTE]
>
>Lorsque des enregistrements anonymes sont fusionnés dans un enregistrement de personne nouveau ou existant, les valeurs de champ personnalisé **ne sont** pas transférées.
