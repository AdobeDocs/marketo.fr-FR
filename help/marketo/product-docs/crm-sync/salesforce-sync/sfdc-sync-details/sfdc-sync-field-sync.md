---
unique-page-id: 2953461
description: Synchronisation SFDC - Synchronisation des champs - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation des champs
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Synchronisation SFDC : synchronisation des champs {#sfdc-sync-field-sync}

Marketo Engage synchronise les informations de champ de Salesforce. Voici les détails.

## Quels champs sont synchronisés ? {#which-fields-are-synced}

Nous synchronisons la plupart des champs standard dans SFDC et tous les champs personnalisés que l’utilisateur de synchronisation est autorisé à voir.

## Comment déterminer si un enregistrement dans Marketo est un prospect ou un contact dans Salesforce ? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Nous avons un champ dans Marketo appelé SFDC Type. Il a trois valeurs possibles : plomb, contact ou vide. S’il est vide, cela signifie que ce prospect Marketo n’existe pas dans SFDC.

## Comment déterminer si un prospect ou un contact est supprimé dans SFDC ? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Nous avons un champ dans Marketo appelé SFDC isDeleted. Si la valeur est true, la piste a été supprimée dans SFDC.

## Comment puis-je m’assurer qu’un nouveau champ que j’ajoute dans SFDC soit également ajouté à Marketo ? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Si vous souhaitez qu’un champ soit présent dans les deux systèmes, créez-le d’abord dans SFDC et il sera automatiquement synchronisé avec Marketo.

Si vous ajoutez un nouveau champ dans SFDC et que l’utilisateur de synchronisation est autorisé à le voir, il sera automatiquement ajouté à Marketo.

## Que se passe-t-il si je modifie un libellé de champ dans SFDC ? {#what-if-i-change-a-field-label-in-sfdc}

La modification du libellé du champ dans la collecte de données régionale n’a aucune incidence sur le libellé du champ dans Marketo.

## Que se passe-t-il si je modifie un type de champ dans SFDC ? {#what-if-i-change-a-field-type-in-sfdc}

Lorsque vous modifiez un type de champ, Marketo supprime les données des champs si elles ne correspondent pas (mais affiche d’abord un avertissement). Pour conserver les données, veillez à les exporter et à les réimporter une fois que vous avez modifié le type de champ.

## Que se passe-t-il si je modifie le nom d’une API dans SFDC ? {#what-if-i-change-an-api-name-in-sfdc}

Si vous modifiez le nom d’API d’un champ dans SFDC, un nouveau champ est créé dans Marketo.

## Que se passe-t-il si j’ajoute une nouvelle valeur de liste de sélection dans SFDC ? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Si une nouvelle valeur de liste de sélection est ajoutée à un champ dans la SFDC, Marketo vous envoie une notification.

## Qu’en est-il des champs de recherche personnalisés SFDC ? {#what-about-custom-sfdc-lookup-fields}

Les champs de recherche dans SFDC synchronisent l’identifiant mais pas le nom référencé.

## Qu&#39;en est-il des champs de formule de la DDC ? {#what-about-sfdc-formula-fields}

Les champs de formule sont synchronisés. Toutefois, les mises à jour apportées aux références de la formule ne sont pas synchronisées tant qu’une mise à jour n’a pas été effectuée sur l’[horodatage de la mémoire système](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US){target="_blank"}.

## Que se passe-t-il lorsque je supprime un champ de Salesforce qui était synchronisé avec Marketo ? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Si vous supprimez un champ dans SFDC, il ne supprime pas automatiquement le champ dans Marketo, la synchronisation s’arrête.
