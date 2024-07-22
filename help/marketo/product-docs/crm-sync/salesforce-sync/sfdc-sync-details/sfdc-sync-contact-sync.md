---
unique-page-id: 2953457
description: Synchronisation SFDC - Synchronisation des contacts - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation des contacts
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Synchronisation SFDC : synchronisation des contacts {#sfdc-sync-contact-sync}

Saviez-vous que Marketo Engage synchronise entièrement votre base de données avec Salesforce ? Il se synchronise, puis attend 5 minutes et se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les contacts Salesforce.

## Direction de la synchronisation {#sync-direction}

La synchronisation des contacts est bidirectionnelle. Si vous apportez des modifications à un contact dans Salesforce ou Marketo, vos mises à jour seront répercutées dans les deux systèmes.

## Que se passe-t-il si des modifications sont effectuées simultanément dans les deux systèmes ? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Nous sommes gentils et laissons Salesforce gagner. Il est rare que ce genre de collision de données se produise.

## Puis-je convertir une personne en contact dans Marketo ? {#can-i-convert-a-person-into-a-contact-in-marketo}

Oui, utilisez l’action de flux **[Convert Person](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>La conversion d’une personne dans Marketo génère un nouveau compte et une nouvelle opportunité dans Salesforce. Si vous ne souhaitez pas de comptes en double, utilisez Salesforce pour effectuer la conversion.

## Puis-je forcer manuellement la synchronisation d’un contact ? {#can-i-manually-force-a-sync-of-a-contact}

Oui, utilisez l’action de flux **[Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** et elle se synchronise en temps réel.

## Chaque champ standard est-il synchronisé avec Marketo ? {#does-every-single-standard-field-sync-to-marketo}

Non, tous les champs standard ne sont pas utiles. Tous les champs personnalisés peuvent être synchronisés.

>[!NOTE]
>
>Marketo synchronise uniquement les champs auxquels votre utilisateur de synchronisation Marketo a accès.

## Marketo respectera-t-il les règles de validation Salesforce ? {#will-marketo-respect-the-salesforce-validation-rules}

Oui, en cas de conflit, le résultat sera consigné dans le journal d’activité des prospects.
