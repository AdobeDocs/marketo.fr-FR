---
unique-page-id: 2953455
description: Synchronisation SFDC - Synchronisation des pistes - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation des pistes
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Synchronisation SFDC : synchronisation des pistes {#sfdc-sync-lead-sync}

Connaissez-vous les synchronisations des Marketo Engage de votre base de données Salesforce ? Il se synchronise, attend 5 minutes, puis se synchronise à nouveau. Toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les prospects Salesforce.

## Direction de la synchronisation {#sync-direction}

La synchronisation des contacts et des pistes est bidirectionnelle. Si vous apportez des modifications à un enregistrement dans Salesforce ou Marketo, vos mises à jour seront répercutées dans les deux systèmes.

## Que se passe-t-il si des modifications sont effectuées simultanément dans les deux systèmes ? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo l&#39;emporte. Il est rare que ce genre de collision de données se produise.

## Puis-je créer un prospect dans Salesforce à l’aide de Marketo ? {#can-i-create-a-lead-in-salesforce-using-marketo}

Oui, utilisez le [Personne synchronisée avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} action de flux. Cela créera un prospect dans Salesforce si le prospect n’existe pas.

## Puis-je forcer manuellement la synchronisation d’une personne dans Marketo avec un prospect dans Salesforce ? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Oui, utilisez le [Personne synchronisée avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} l’action de flux et elle se synchronise en temps réel.

## Chaque champ standard est-il synchronisé avec Marketo ? {#does-every-single-standard-field-sync-to-marketo}

Non, tous les champs standard ne sont pas utiles. Tous les champs personnalisés peuvent être synchronisés.

>[!NOTE]
>
>Marketo synchronise uniquement les champs auxquels votre utilisateur de synchronisation Salesforce a accès.

## Marketo respectera-t-il les règles de validation Salesforce ? {#will-marketo-respect-the-salesforce-validation-rules}

Oui. La synchronisation échoue si le format des données est incorrect ou si les informations de champ requises sont manquantes. Marketo consigne le résultat dans le journal d’activité des prospects si cela se produit.
