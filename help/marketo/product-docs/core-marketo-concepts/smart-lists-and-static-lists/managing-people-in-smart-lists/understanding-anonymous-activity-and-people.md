---
unique-page-id: 1147322
description: Présentation de l’activité anonyme et des personnes - Documents Marketo - Documentation du produit
title: Présentation de l’activité anonyme et des personnes
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Présentation de l’activité anonyme et des personnes {#understanding-anonymous-activity-and-people}

La première fois qu’une personne visite une page d’entrée Marketo (ou une page de votre site web qui comporte le [code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}), Marketo crée une *activité anonyme* et utilise un cookie de navigateur pour en effectuer le suivi. Une fois identifié, il devient une personne et l’historique associé au cookie de son navigateur est fusionné.

>[!IMPORTANT]
>
>L’activation de la fonction Beta **Munchkin V2 Anonymous Replay Activity on Known** garantit que les campagnes déclenchées par une promotion de piste anonyme seront toujours relues une fois le prospect anonyme fusionné dans l’enregistrement connu. Par conséquent, les champs personnalisés modifiés par les étapes Modifier la valeur des données dans toutes les campagnes relues seront conservés dans l’enregistrement connu.

**Une activité Anonyme** est créée lorsqu’une personne :

* Visite votre page d’entrée Marketo la première fois.
* Visite une page de votre site qui a le [suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Clique sur le lien [Afficher comme page Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} dans un courrier électronique Marketo.

>[!NOTE]
>
>Contrairement à d’autres liens dans les emails Marketo, [Afficher comme page web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} n’est pas suivi comme un clic d’email.

Une activité anonyme est fusionnée en une nouvelle personne ou une personne existante lorsqu’une personne :

* Clique sur un lien [dans un email Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Remplit un [formulaire](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} Marketo.
* Utilise l’API Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} ou [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} (pour les développeurs) pour associer une personne anonyme à un enregistrement connu.

Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents appareils et navigateurs pour consulter votre site.

>[!NOTE]
>
>Lorsque des enregistrements anonymes sont fusionnés en un nouvel enregistrement de personne ou un enregistrement de personne existant, les valeurs de champ personnalisé *et non* sont transférées.
