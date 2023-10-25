---
unique-page-id: 1147322
description: Présentation de l’activité anonyme et des personnes - Documents Marketo - Documentation du produit
title: Présentation de l’activité anonyme et des personnes
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Présentation de l’activité anonyme et des personnes {#understanding-anonymous-activity-and-people}

la première fois qu’une personne visite une page d’entrée Marketo (ou une page de votre site web qui contient la variable [Code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}), Marketo crée une *activité anonyme* et utilise un cookie de navigateur pour en effectuer le suivi. Une fois identifié, il devient une personne et l’historique associé au cookie de son navigateur est fusionné.

>[!IMPORTANT]
>
>Activation de la fonctionnalité bêta **Activité de relecture anonyme Munchkin V2 sur connu** garantit que les campagnes déclenchées par une promotion de piste anonyme seront toujours relues une fois que la piste anonyme sera fusionnée dans l’enregistrement connu. Par conséquent, les champs personnalisés modifiés par les étapes Modifier la valeur des données dans toutes les campagnes relues seront conservés dans l’enregistrement connu.

**Un Anonyme** l’activité est créée lorsqu’une personne :

* Visite votre page d’entrée Marketo la première fois.
* Visite une page de votre site qui comporte [Tracking Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Cliquez sur le bouton [Afficher comme page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} dans un email Marketo.

>[!NOTE]
>
>Contrairement aux autres liens des emails Marketo, [Afficher comme page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} n’est pas suivi en tant que clic sur un email.

Une activité anonyme est fusionnée en une nouvelle personne ou une personne existante lorsqu’une personne :

* Cliquez sur un [lien dans un email Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Remplissage d’un Marketo [Formulaire](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}.
* Utilise Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} or [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} API (pour les développeurs) pour associer une personne anonyme à un enregistrement connu.

Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents appareils et navigateurs pour consulter votre site.

>[!NOTE]
>
>Lorsque des enregistrements anonymes sont fusionnés en un nouvel enregistrement de personne ou un enregistrement de personne existant, les valeurs de champ personnalisées sont *not* transférer.
