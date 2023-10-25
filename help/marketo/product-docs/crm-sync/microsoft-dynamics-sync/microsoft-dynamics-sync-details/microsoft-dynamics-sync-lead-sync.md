---
unique-page-id: 3571848
description: Synchronisation Microsoft Dynamics - Synchronisation des pistes - Documents Marketo - Documentation du produit
title: Synchronisation Microsoft Dynamics - Synchronisation des pistes
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Synchronisation Microsoft Dynamics : synchronisation des pistes {#microsoft-dynamics-sync-lead-sync}

Marketo Engage à la synchronisation Dynamics est très puissant. Voici les détails.

## Comment les détails sont-ils synchronisés entre les deux systèmes ? {#how-are-details-kept-in-sync-between-the-two-systems}

La synchronisation est bidirectionnelle. Si vous apportez des modifications à un prospect dans Dynamics ou à une personne dans Marketo, votre mise à jour sera répercutée dans les deux systèmes.

>[!NOTE]
>
>Les suppressions ne se synchronisent pas toujours automatiquement dans les deux directions. Voir [Suppression d’un prospect ou d’un contact](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## Que se passe-t-il si des modifications sont apportées simultanément au même champ dans les deux systèmes ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les personnes (pistes) et Dynamics gagnera pour les contacts. En effet, nous considérons que le service marketing fait autorité pour les personnes, alors que le système officiel d&#39;enregistrement des contacts est celui des ventes (CRM).

## Puis-je créer un prospect dans Dynamics à l’aide de Marketo ? {#can-i-create-a-lead-in-dynamics-using-marketo}

Oui, utilisez le [Synchronisation de la personne avec Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} action de flux. Cela créera une piste dans Dynamics si la piste n’existe pas. Si la piste existe, l’étape de flux n’effectue aucune action.

>[!NOTE]
>
>Lors de l’utilisation de l’action de flux &quot;Synchroniser la personne avec Microsoft&quot; (dans une campagne de déclenchement uniquement), le prospect/contact est créé en temps réel dans Dynamics.

## Puis-je forcer manuellement la synchronisation d’une personne de Marketo vers un prospect dans Dynamics ? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Non, la synchronisation en arrière-plan automatisée est le seul moyen de synchroniser les mises à jour entre Marketo et Dynamics. La variable [Synchronisation de la personne avec Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} l’action de flux ne force pas la synchronisation du prospect.

## Quels champs seront synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration.

## Marketo respectera-t-il les règles de validation Dynamics ? {#will-marketo-respect-the-dynamics-validation-rules}

Oui. La synchronisation échoue si le format des données est incorrect ou si les informations de champ requises sont manquantes. Marketo consigne le résultat dans le journal d’activité de la personne si cela se produit.
