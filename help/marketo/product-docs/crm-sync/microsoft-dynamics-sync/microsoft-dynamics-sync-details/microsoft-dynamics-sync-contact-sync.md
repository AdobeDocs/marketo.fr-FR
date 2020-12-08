---
unique-page-id: 3571833
description: Microsoft Dynamics Sync - Contact Sync - Marketo Docs - Documentation du produit
title: Microsoft Dynamics Sync -Contact Sync
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Microsoft Dynamics Sync : Synchronisation des contacts {#microsoft-dynamics-sync-contact-sync}

Saviez-vous que Marketo synchronise votre base de données complète avec Dynamics ? Il se synchronise, puis attend 5 minutes puis se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la façon dont Marketo traite spécifiquement les contacts Dynamics.

## Comment les détails sont-ils synchronisés entre les deux systèmes ? {#how-are-details-kept-in-sync-between-the-two-systems}

La synchronisation des contacts est bidirectionnelle. Si vous apportez des modifications à un contact dans Dynamics ou à une personne dans Marketo, vos mises à jour seront répercutées dans les deux systèmes.

## Que se passe-t-il si des modifications sont apportées au même champ dans les deux systèmes en même temps ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les gens et Dynamics gagnera pour les contacts. Cela est dû au fait que nous considérons le service marketing comme faisant autorité pour les gens, alors que le système officiel d&#39;enregistrement des contacts se trouve dans le service des ventes (CRM).

## Puis-je créer un contact à l’aide de Marketo ? {#can-i-create-a-contact-using-marketo}

Oui. [Voici comment](microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>Lors de l&#39;utilisation de l&#39;action de flux &quot;Synchroniser la personne avec Microsoft&quot; (dans une campagne de déclenchement uniquement), le prospect/contact est créé en temps réel dans Dynamics.

## Puis-je forcer manuellement la synchronisation d&#39;une personne ou d&#39;un contact ? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Non, la synchronisation en arrière-plan automatisée est le seul moyen de synchroniser les mises à jour entre Marketing et Dynamics. La personne [synchronisée avec Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) ne forcera pas la synchronisation du prospect.

## Quels champs seront synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) lors de la configuration. Mais Marketo synchronise uniquement les champs auxquels votre utilisateur Dynamics sync a accès.

## Marketo respectera-t-il les règles de validation Dynamics ? {#will-marketo-respect-the-dynamics-validation-rules}

Oui, en cas de conflit, il consigne le résultat dans le journal des Activités des pistes.
