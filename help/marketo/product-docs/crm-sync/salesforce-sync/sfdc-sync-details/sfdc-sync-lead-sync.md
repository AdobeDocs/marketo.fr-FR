---
unique-page-id: 2953455
description: Synchronisation SFDC - Synchronisation des pistes - Documents marketing - Documentation du produit
title: Synchronisation SFDC - Synchronisation des pistes
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# Synchronisation SFDC : Synchronisation des pistes {#sfdc-sync-lead-sync}

Connaissez-vous Marketo synchronisé à partir de votre base de données Salesforce ? Il synchronise, attend 5 minutes, puis se synchronise à nouveau. Toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les pistes de Salesforce.

## Direction de synchronisation {#sync-direction}

Le prospect (personne) et la synchronisation des contacts sont bidirectionnels. Si vous apportez des modifications à un enregistrement dans Salesforce ou Marketo, vos mises à jour seront répercutées dans les deux systèmes.

## Que se passe-t-il si des modifications sont effectuées simultanément dans les deux systèmes ? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Le marché gagne. Il est rare que ce genre de collision de données se produise.

## Puis-je créer un prospect dans Salesforce en utilisant Marketo ? {#can-i-create-a-lead-in-salesforce-using-marketo}

Oui, utilisez l’action de flux [Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Cela créera un prospect dans Salesforce si le prospect n&#39;existe pas.

## Puis-je forcer manuellement la synchronisation d&#39;une personne dans Marketo vers une piste dans Salesforce ? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Oui, utilisez l’action de flux [Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) et elle sera synchronisée en temps réel.

## Est-ce que chaque champ standard est synchronisé avec Marketo ? {#does-every-single-standard-field-sync-to-marketo}

Non, tous les champs standard ne sont pas utiles. Tous les champs personnalisés peuvent faire partie de la synchronisation.

>[!NOTE]
>
>Marketo synchronise uniquement les champs auxquels votre utilisateur de synchronisation Salesforce a accès.

## Marketo respectera-t-il les règles de validation Salesforce ? {#will-marketo-respect-the-salesforce-validation-rules}

Oui. La synchronisation échoue si le format des données est incorrect ou si les informations de champ requises sont manquantes. Marketo consigne le résultat dans le journal des Activités des prospects si cela se produit.
