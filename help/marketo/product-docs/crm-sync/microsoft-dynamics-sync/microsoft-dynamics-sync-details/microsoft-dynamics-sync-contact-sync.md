---
unique-page-id: 3571833
description: Synchronisation Microsoft Dynamics - Synchronisation des contacts - Documents Marketo - Documentation du produit
title: Synchronisation Microsoft Dynamics - Synchronisation des contacts
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Synchronisation Microsoft Dynamics : synchronisation des contacts {#microsoft-dynamics-sync-contact-sync}

Saviez-vous que Marketo Engage synchronise entièrement votre base de données avec Dynamics ? Il se synchronise, puis attend 5 minutes et se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les contacts Dynamics.

## Comment les détails sont-ils synchronisés entre les deux systèmes ? {#how-are-details-kept-in-sync-between-the-two-systems}

La synchronisation des contacts est bidirectionnelle. Si vous apportez des modifications à un contact dans Dynamics ou à une personne dans Marketo, vos mises à jour seront répercutées dans les deux systèmes.

## Que se passe-t-il si des modifications sont apportées simultanément au même champ dans les deux systèmes ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les personnes et Dynamics gagnera pour les contacts. En effet, nous considérons que le service marketing fait autorité pour les personnes, alors que le système officiel d&#39;enregistrement des contacts est celui des ventes (CRM).

## Puis-je créer un contact à l’aide de Marketo ? {#can-i-create-a-contact-using-marketo}

Oui. [Voici comment ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>Lors de l’utilisation de l’action de flux &quot;Synchroniser la personne avec Microsoft&quot; (dans une campagne de déclenchement uniquement), le prospect/contact est créé en temps réel dans Dynamics.

## Puis-je forcer manuellement la synchronisation d’une personne ou d’un contact ? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Non, la synchronisation en arrière-plan automatisée est le seul moyen de synchroniser les mises à jour entre Marketo et Dynamics. La [personne synchronisée avec Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} ne force pas la synchronisation de l’avance.

## Quels champs seront synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration. Mais Marketo synchronise uniquement les champs auxquels votre utilisateur de synchronisation Dynamics a accès.

## Marketo respectera-t-il les règles de validation Dynamics ? {#will-marketo-respect-the-dynamics-validation-rules}

Oui, en cas de conflit, le résultat sera consigné dans le journal d’activité des prospects.
