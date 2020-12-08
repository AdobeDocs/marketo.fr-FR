---
unique-page-id: 2953457
description: Synchronisation SFDC - Synchronisation des contacts - Documents marketing - Documentation du produit
title: Synchronisation SFDC - Synchronisation des contacts
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---


# Synchronisation SFDC : Synchronisation des contacts {#sfdc-sync-contact-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Saviez-vous que Marketo synchronise votre base de données complète avec Salesforce ? Il se synchronise, puis attend 5 minutes puis se synchronise à nouveau, toute la journée, tous les jours. Voici quelques détails sur la manière dont Marketo traite spécifiquement les contacts Salesforce.

## Direction de la synchronisation {#sync-direction}

La synchronisation des contacts est bidirectionnelle. Si vous apportez des modifications à un contact dans Salesforce ou Marketo, vos mises à jour seront répercutées dans les deux systèmes.

## Que se passe-t-il si des modifications sont effectuées simultanément dans les deux systèmes ? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Nous sommes gentils et laissons Salesforce gagner. Il est rare que ce genre de collision de données se produise.

## Puis-je convertir une personne en contact dans Marketo ? {#can-i-convert-a-person-into-a-contact-in-marketo}

Oui, utilisez l’action de flux ** [Convertir une personne](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**.

>[!CAUTION]
>
>La conversion d’une personne sur le marché se traduira par un nouveau compte et une nouvelle opportunité dans Salesforce. Si vous ne souhaitez pas de comptes de duplicata, utilisez Salesforce pour effectuer une conversion.

## Puis-je forcer manuellement la synchronisation d&#39;un contact ? {#can-i-manually-force-a-sync-of-a-contact}

Oui, utilisez l&#39;action ** [Sync Personne to SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **flow et elle sera synchronisée en temps réel.

## Est-ce que chaque champ standard est synchronisé avec Marketo ? {#does-every-single-standard-field-sync-to-marketo}

Non, tous les champs standard ne sont pas utiles. Tous les champs personnalisés peuvent faire partie de la synchronisation.

>[!NOTE]
>
>Marketo synchronise uniquement les champs auxquels l’utilisateur de synchronisation du marketing a accès.

## Marketo respectera-t-il les règles de validation Salesforce ? {#will-marketo-respect-the-salesforce-validation-rules}

Oui, en cas de conflit, il consigne le résultat dans le journal des Activités des pistes.
