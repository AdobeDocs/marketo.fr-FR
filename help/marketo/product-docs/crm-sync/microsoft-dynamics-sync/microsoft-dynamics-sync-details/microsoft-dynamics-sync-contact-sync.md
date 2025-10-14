---
unique-page-id: 3571833
description: Synchronisation de Microsoft Dynamics - Synchronisation des contacts - Documents Marketo - Documentation du produit
title: Synchronisation Microsoft Dynamics - Synchronisation des contacts
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Synchronisation des [!DNL Microsoft Dynamics] : synchronisation des contacts {#microsoft-dynamics-sync-contact-sync}

Saviez-vous que Marketo synchronise l’ensemble de votre base de données avec [!DNL Dynamics] ? Il se synchronise, puis attend 5 minutes, puis se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la façon dont Marketo traite spécifiquement les contacts [!DNL Dynamics].

## Comment les détails sont-ils synchronisés entre les deux systèmes ? {#how-are-details-kept-in-sync-between-the-two-systems}

La synchronisation des contacts est bidirectionnelle. Si vous apportez des modifications à un contact dans [!DNL Dynamics] ou à une personne dans Marketo, vos mises à jour seront répercutées sur les deux systèmes.

## Que faire si des modifications sont apportées simultanément au même champ dans les deux systèmes ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les gens et [!DNL Dynamics] gagnera pour les contacts. En effet, nous considérons que le service marketing fait autorité pour les personnes, alors que le système officiel d’enregistrement des contacts se trouve dans le service des ventes (CRM).

## Puis-je créer un contact à l’aide de Marketo ? {#can-i-create-a-contact-using-marketo}

Oui. [Voici comment &#x200B;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>Lors de l’utilisation de l’action de flux « Synchroniser la personne avec Microsoft » (dans une campagne de déclenchement uniquement), le prospect/contact est créé en temps réel dans [!DNL Dynamics].

## Puis-je forcer manuellement la synchronisation d’une personne ou d’un contact ? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Non, la synchronisation en arrière-plan automatisée est la seule façon de synchroniser les mises à jour entre Marketo et [!DNL Dynamics]. La [Synchroniser la personne avec Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) ne force pas la synchronisation du prospect.

## Quels champs vont être synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) lors de la configuration. Cependant, Marketo ne synchronise que les champs auxquels l’utilisateur de la synchronisation [!DNL Dynamics] a accès.

## Marketo respectera-t-il les règles de validation [!DNL Dynamics] ? {#will-marketo-respect-the-dynamics-validation-rules}

Oui, en cas de conflit, le résultat est consigné dans le journal d’activité des prospects.
