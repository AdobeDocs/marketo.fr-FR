---
unique-page-id: 3571838
description: Synchronisation de Microsoft Dynamics - Synchronisation des champs - Documents Marketo - Documentation du produit
title: Synchronisation Microsoft Dynamics - Synchronisation des champs
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Synchronisation des [!DNL Microsoft Dynamics] : synchronisation des champs {#microsoft-dynamics-sync-field-sync}

La synchronisation de Marketo vers [!DNL Dynamics] est très puissante. Voici les détails.

## Comment les détails des champs sont-ils synchronisés entre les deux systèmes ? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La synchronisation est bidirectionnelle pour les entités de prospect et de contact. Si vous apportez des modifications à un prospect ou un contact dans [!DNL Dynamics] ou à une personne dans Marketo, vos mises à jour seront répercutées sur les deux systèmes.

Pour les entités de compte, d’utilisateur, d’opportunité, d’équipe et personnalisées, la synchronisation est unidirectionnelle : [!DNL Dynamics] vers Marketo. Si vous apportez des modifications à ces entités dans [!DNL Dynamics], vos mises à jour seront répercutées dans Marketo.

## Que faire si des modifications sont apportées simultanément au même champ dans les deux systèmes ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les personnes (prospects) et [!DNL Dynamics] gagnera pour les contacts. En effet, nous considérons que le service marketing fait autorité pour les personnes, alors que le système officiel d’enregistrement des contacts se trouve dans le service des ventes (CRM). Pour les entités de synchronisation unidirectionnelles, [!DNL Dynamics] gagnera toujours.

## Puis-je créer un champ dans [!DNL Dynamics] à l’aide de Marketo ? {#can-i-create-a-field-in-dynamics-using-marketo}

Non, ceci n’est actuellement pas pris en charge.

## J&#39;ai créé un champ dans [!DNL Dynamics]. Puis-je le synchroniser avec Marketo ? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Oui, vous pouvez [synchroniser le champ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) tant que l’utilisateur de la synchronisation y a accès dans [!DNL Dynamics].

## Quels champs vont être synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration.

## Que se passe-t-il si je dois ajouter un champ personnalisé après la synchronisation de Marketo et [!DNL Dynamics] ? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Vous pouvez ajouter des champs à tout moment et vous attendre à ce que les données soient actualisées de [!DNL Dynamics] vers Marketo. Pour plus d’informations[&#x200B; consultez la section  [!DNL Microsoft Dynamics] Utiliser la synchronisation rapide avec pour un nouveau champ personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) .

## Que se passe-t-il si je souhaite supprimer un champ dans [!DNL Dynamics] après l’ajout du champ pour la synchronisation ? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans [!DNL Dynamics], nous vous recommandons de le faire avec la [synchronisation désactivée](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Ensuite, actualisez le schéma dans Marketo en modifiant et en enregistrant le [&#x200B; Sélectionner les champs à synchroniser &#x200B;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
