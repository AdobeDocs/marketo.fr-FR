---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Documentation du produit
title: Microsoft Dynamics Sync -Field Sync
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---


# Microsoft Dynamics Sync : Synchronisation des champs {#microsoft-dynamics-sync-field-sync}

Marketo to Dynamics sync est très puissant. Voici les détails.

## Comment les détails des champs sont-ils synchronisés entre les deux systèmes ? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La synchronisation est bidirectionnelle pour les entités de piste et de contact. Si vous apportez des modifications à une piste ou un contact dans Dynamics ou à une personne dans Marketo, vos mises à jour seront répercutées dans les deux systèmes.

Pour les entités de compte, d’utilisateur, d’opportunité, d’équipe et personnalisées, la synchronisation est à sens unique : Dynamique vers marketing. Si vous apportez des modifications à ces entités dans Dynamics, vos mises à jour seront répercutées dans Marketo.

## Que se passe-t-il si des modifications sont apportées au même champ dans les deux systèmes en même temps ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les gens (pistes) et Dynamics gagnera pour les contacts. Cela est dû au fait que nous considérons le service marketing comme faisant autorité pour les gens, alors que le système officiel d&#39;enregistrement des contacts se trouve dans le service des ventes (CRM). Pour les entités de synchronisation à sens unique, Dynamics gagnera toujours.

## Puis-je créer un champ dans Dynamics using Marketo ? {#can-i-create-a-field-in-dynamics-using-marketo}

Non, ceci n&#39;est pas pris en charge actuellement.

## J&#39;ai créé un champ dans Dynamics. Puis-je le synchroniser avec Marketo ? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Oui, vous pouvez [synchroniser le champ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) tant que votre utilisateur de synchronisation y a accès dans Dynamics.

## Quels champs seront synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) pendant la configuration.

## Que se passe-t-il si je dois ajouter un champ personnalisé après la synchronisation de Marketing et de Dynamics ? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Vous pouvez ajouter des champs à tout moment et vous attendez à ce que les données soient actualisées de Dynamics vers Marketo. Voir [Utilisation de la synchronisation rapide avec Microsoft Dynamics pour un nouveau champ personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) pour plus d&#39;informations.

## Que se passe-t-il si je souhaite supprimer un champ dans Dynamics après l&#39;ajout du champ à la synchronisation ? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans Dynamics, nous vous recommandons de le faire avec la [synchronisation désactivée](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Actualisez ensuite le schéma dans Marketo en modifiant et en enregistrant les [champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).