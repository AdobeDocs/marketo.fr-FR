---
unique-page-id: 2953455
description: Synchronisation de SFDC - Synchronisation des leads - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Synchronisation des leads
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 2%

---

# Synchronisation SFDC : synchronisation des leads {#sfdc-sync-lead-sync}

Connaissiez-vous les synchronisations Marketo à partir de votre base de données [!DNL Salesforce] ? Il se synchronise, attend 5 minutes, puis se synchronise à nouveau. Toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les prospects [!DNL Salesforce].

## Direction de synchronisation {#sync-direction}

La synchronisation du prospect (personne) et du contact est bidirectionnelle. Si vous apportez des modifications à un enregistrement dans [!DNL Salesforce] ou Marketo, vos mises à jour seront répercutées sur les deux systèmes.

## Que faire si des modifications sont apportées simultanément dans les deux systèmes ? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gagne. Il est rare que ce genre de collision de données se produise.

## Puis-je créer un prospect dans [!DNL Salesforce] à l’aide de Marketo ? {#can-i-create-a-lead-in-salesforce-using-marketo}

Oui, utiliser l’action de flux [ Synchroniser la personne avec SFDC ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Cette opération crée un prospect dans [!DNL Salesforce] si le prospect n’existe pas.

## Puis-je forcer manuellement la synchronisation d’une personne dans Marketo avec un prospect dans [!DNL Salesforce] ? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Oui, utilisez l’action de flux [ Synchroniser la personne avec SFDC ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} et elle se synchronisera en temps réel.

## Chaque champ standard est-il synchronisé avec Marketo ? {#does-every-single-standard-field-sync-to-marketo}

Non, tous les champs standard ne sont pas utiles. Tous les champs personnalisés peuvent faire partie de la synchronisation.

>[!NOTE]
>
>Marketo synchronise uniquement les champs auxquels l’utilisateur de la synchronisation [!DNL Salesforce] a accès.

## Marketo respectera-t-il les règles de validation [!DNL Salesforce] ? {#will-marketo-respect-the-salesforce-validation-rules}

Oui. La synchronisation échoue si le format de données est incorrect ou s’il manque des informations de champ requises. Si cela se produit, Marketo consigne les résultats dans le journal d’activité des prospects.
