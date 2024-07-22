---
unique-page-id: 3571838
description: Synchronisation Microsoft Dynamics - Synchronisation des champs - Documents Marketo - Documentation du produit
title: Synchronisation des champs Microsoft Dynamics
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Synchronisation Microsoft Dynamics : synchronisation des champs {#microsoft-dynamics-sync-field-sync}

Marketo Engage à la synchronisation Dynamics est très puissant. Voici les détails.

## Comment les détails des champs sont-ils synchronisés entre les deux systèmes ? {#how-are-field-details-kept-in-sync-between-the-two-systems}

La synchronisation est bidirectionnelle pour les entités de prospect et de contact. Si vous apportez des modifications à un prospect ou à un contact dans Dynamics ou à une personne dans Marketo, vos mises à jour seront répercutées dans les deux systèmes.

Pour les entités de compte, d’utilisateur, d’opportunité, d’équipe et personnalisées, la synchronisation est unidirectionnelle : Dynamics vers Marketo. Si vous apportez des modifications à ces entités dans Dynamics, vos mises à jour seront répercutées dans Marketo.

## Que se passe-t-il si des modifications sont apportées simultanément au même champ dans les deux systèmes ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les personnes (pistes) et Dynamics gagnera pour les contacts. En effet, nous considérons que le service marketing fait autorité pour les personnes, alors que le système officiel d&#39;enregistrement des contacts est celui des ventes (CRM). Pour les entités de synchronisation unidirectionnelle, Dynamics gagnera toujours.

## Puis-je créer un champ dans Dynamics à l’aide de Marketo ? {#can-i-create-a-field-in-dynamics-using-marketo}

Non, cela n’est actuellement pas pris en charge.

## J’ai créé un champ dans Dynamics. Puis-je le synchroniser avec Marketo ? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Oui, vous pouvez [synchroniser le champ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} tant que votre utilisateur de synchronisation y a accès dans Dynamics.

## Quels champs seront synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration.

## Que faire si je dois ajouter un champ personnalisé après la synchronisation de Marketo et de Dynamics ? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Vous pouvez ajouter des champs à tout moment et vous attendre à ce que les données soient actualisées de Dynamics vers Marketo. Pour plus d’informations, voir [Utilisation de la synchronisation rapide avec Microsoft Dynamics pour un nouveau champ personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md){target="_blank"} .

## Que se passe-t-il si je souhaite supprimer un champ dans Dynamics après l’ajout du champ à la synchronisation ? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo stocke une référence aux champs à synchroniser. Si vous supprimez un champ dans Dynamics, nous vous recommandons de le faire avec la [synchronisation désactivée](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Actualisez ensuite le schéma dans Marketo en modifiant et en enregistrant le [champ de sélection à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.
