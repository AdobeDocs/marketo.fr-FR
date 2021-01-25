---
unique-page-id: 1147322
description: Présentation de l'Activité et des personnes anonymes - Documents marketing - Documentation du produit
title: Présentation de l'Activité et des personnes anonymes
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# Présentation de l&#39;Activité anonyme et des personnes {#understanding-anonymous-activity-and-people}

Lors de la première visite d’un landing page Marketo (ou d’une page de votre site Web contenant le [code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crée une _activité anonyme_ et utilise un cookie de navigateur pour effectuer le suivi. Une fois identifié, il devient une personne et l&#39;historique associé au cookie de son navigateur est fusionné.

**Une** activité anonyme est créée lorsqu’une personne :

* Visite votre landing page Marketing pour la première fois.
* Visite une page de votre site qui comporte [suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Cliquez sur le lien [Vue en tant que page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) dans un courrier électronique Marketo.

>[!NOTE]
>
>Contrairement à d&#39;autres liens dans les courriers électroniques de Marketo, [la Vue en tant que page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) n&#39;est pas suivie en tant que clic électronique.

Une activité anonyme est fusionnée en une personne nouvelle ou existante lorsqu’une personne :

* Cliquez sur un lien [dans un courrier électronique Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Remplit un Marketo [Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Utilise l&#39;API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) ou [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) de Marketo (pour les développeurs) pour associer une personne anonyme à un enregistrement connu.

Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents périphériques et navigateurs pour visiter votre site.

>[!NOTE]
>
>Lorsque des enregistrements anonymes sont fusionnés dans un enregistrement de personne nouveau ou existant, les valeurs de champ personnalisé **ne sont** pas transférées.
