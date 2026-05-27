---
unique-page-id: 1147322
description: Découvrez l’activité anonyme et les personnes dans Marketo. Découvrez comment les visiteurs anonymes sont suivis avant la conversion.
title: Présentation des activités et des personnes anonymes
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
TQID: https://experienceleague.adobe.com/avWmJKBGktOEseVl3uIYB9Bp19Rq3HQgo98gKJFDtIc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 271
ht-degree: 3%

---

# Présentation des activités et des personnes anonymes {#understanding-anonymous-activity-and-people}

La première fois qu’une personne visite une page de destination de Marketo (ou une page de votre site web comportant le [code de suivi Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}), Marketo crée une *activité anonyme* et utilise un cookie de navigateur pour la suivre. Une fois identifié, il devient une personne et l’historique associé à son cookie de navigateur est fusionné.

>[!IMPORTANT]
>
>L’activation de la fonction Beta **[!DNL Munchkin]l’activité de relecture anonyme V2 sur Connu** garantit que les campagnes déclenchées par la promotion de prospect anonyme seront toujours relues une fois le prospect anonyme fusionné avec succès dans l’enregistrement connu. Par conséquent, les champs personnalisés modifiés par les étapes Modifier la valeur des données dans les campagnes relues seront conservés dans l’enregistrement connu.

Une activité **Anonyme** est créée lorsque quelqu’un :

* Première visite de votre page de destination Marketo.
* Visite une page de votre site qui a un [suivi ](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Clique sur le lien [Afficher en tant que page web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} dans un e-mail Marketo.

>[!NOTE]
>
>Contrairement aux autres liens dans les e-mails Marketo, [Afficher en tant que page web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} n’est pas suivi comme un clic sur un e-mail.

Une activité anonyme est fusionnée en une personne nouvelle ou existante lorsque quelqu’un :

* Clique sur un [lien dans un email Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Remplit un Marketo [Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}.
* Utilise l’API de Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} ou [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} (pour les développeurs) pour associer une personne anonyme à un enregistrement connu.

Un nom de la base de données peut être lié à de nombreux cookies, car les visiteurs utilisent souvent différents appareils et navigateurs pour visiter votre site.

>[!NOTE]
>
>Lorsque des enregistrements anonymes sont fusionnés dans un enregistrement de personne nouveau ou existant, les valeurs de champ personnalisé ne sont *transférées*
