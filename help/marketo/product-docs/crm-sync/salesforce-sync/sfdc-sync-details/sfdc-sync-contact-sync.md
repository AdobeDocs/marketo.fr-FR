---
unique-page-id: 2953457
description: Synchronisation de SFDC - Synchronisation des contacts - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Synchronisation des contacts
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 1%

---

# Synchronisation SFDC : synchronisation de contact {#sfdc-sync-contact-sync}

Saviez-vous que Marketo synchronise l’ensemble de votre base de données avec [!DNL Salesforce] ? Il se synchronise, puis attend 5 minutes, puis se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la façon dont Marketo traite spécifiquement les contacts [!DNL Salesforce].

## Direction de synchronisation {#sync-direction}

La synchronisation des contacts est bidirectionnelle. Si vous apportez des modifications à un contact dans [!DNL Salesforce] ou Marketo, vos mises à jour seront répercutées sur les deux systèmes.

## Que faire si des modifications sont apportées simultanément dans les deux systèmes ? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Nous sommes gentils et laissons [!DNL Salesforce] gagner. Il est rare que ce genre de collision de données se produise.

## Puis-je convertir une personne en contact dans Marketo ? {#can-i-convert-a-person-into-a-contact-in-marketo}

Oui, utiliser l’action de flux **[Convertir la personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>La conversion d’une personne dans Marketo entraînera l’ouverture d’un nouveau compte et d’une nouvelle opportunité dans [!DNL Salesforce]. Si vous ne souhaitez pas que des comptes soient dupliqués, utilisez [!DNL Salesforce] pour effectuer la conversion.

## Puis-je forcer manuellement la synchronisation d&#39;un contact ? {#can-i-manually-force-a-sync-of-a-contact}

Oui, utilisez l’action de flux **[Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** et elle se synchronisera en temps réel.

## Chaque champ standard est-il synchronisé avec Marketo ? {#does-every-single-standard-field-sync-to-marketo}

Non, tous les champs standard ne sont pas utiles. Tous les champs personnalisés peuvent faire partie de la synchronisation.

>[!NOTE]
>
>Marketo synchronise uniquement les champs auxquels l’utilisateur de synchronisation Marketo a accès.

## Marketo respectera-t-il les règles de validation [!DNL Salesforce] ? {#will-marketo-respect-the-salesforce-validation-rules}

Oui, en cas de conflit, le résultat est consigné dans le journal d’activité des prospects.
