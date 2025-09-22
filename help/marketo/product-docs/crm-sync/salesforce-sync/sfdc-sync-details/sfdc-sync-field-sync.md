---
unique-page-id: 2953461
description: Synchronisation de SFDC - Synchronisation de champ - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Synchronisation de champ
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Synchronisation SFDC : synchronisation de champ {#sfdc-sync-field-sync}

Marketo synchronise les informations de champ à partir de [!DNL Salesforce]. Voici les détails.

## Quels champs sont synchronisés ? {#which-fields-are-synced}

Nous synchronisons la plupart des champs standard dans SFDC et tout champ personnalisé que l’utilisateur de la synchronisation est autorisé à voir.

## Comment déterminer si un enregistrement dans Marketo est un prospect ou un contact dans [!DNL Salesforce] ? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Il existe un champ dans Marketo appelé Type de SFDC. Il a trois valeurs possibles : lead, contact, ou il est vide. S’il est vide, cela signifie que ce prospect Marketo n’existe pas dans SFDC.

## Comment déterminer si un prospect ou un contact est supprimé dans SFDC ? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Il existe un champ dans Marketo appelé SFDC isDeleted. Si la valeur est définie sur « true », le prospect a été supprimé dans SFDC.

## Comment puis-je m’assurer qu’un nouveau champ que j’ajoute dans SFDC est également ajouté à Marketo ? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Si vous souhaitez créer un champ dans les deux systèmes, commencez par le créer dans SFDC. Il sera automatiquement synchronisé avec Marketo.

Si vous ajoutez un nouveau champ dans SFDC et que l’utilisateur de synchronisation est autorisé à l’afficher, il est automatiquement ajouté à Marketo.

## Que se passe-t-il si je modifie le libellé d’un champ dans SFDC ? {#what-if-i-change-a-field-label-in-sfdc}

La modification du libellé du champ dans SFDC n’affecte pas le libellé du champ dans Marketo.

## Que se passe-t-il si je modifie un type de champ dans SFDC ? {#what-if-i-change-a-field-type-in-sfdc}

Lorsque vous modifiez un type de champ, Marketo supprime les données des champs si elles ne correspondent pas (mais affiche d’abord un avertissement). Pour conserver les données, veillez à les exporter et à les réimporter après avoir modifié le type de champ.

## Que se passe-t-il si je modifie le nom d’une API dans SFDC ? {#what-if-i-change-an-api-name-in-sfdc}

Si vous modifiez le nom d’API d’un champ dans SFDC, un nouveau champ est créé dans Marketo.

## Que se passe-t-il si j’ajoute une nouvelle valeur de liste de sélection dans SFDC ? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Si une nouvelle valeur de liste de sélection est ajoutée dans SFDC à un champ, Marketo vous enverra une notification.

## Qu’en est-il des champs de recherche SFDC personnalisés ? {#what-about-custom-sfdc-lookup-fields}

Les champs de recherche dans SFDC synchronisent l’identifiant, mais pas le nom référencé.

## Qu’en est-il des champs de formule SFDC ? {#what-about-sfdc-formula-fields}

Les champs de formule sont synchronisés. Toutefois, les mises à jour apportées aux références de la formule ne sont synchronisées que lorsqu’un [horodatage de modification du système](https://help.salesforce.com/apex/HTViewSolution?id=000193203&language=en_US){target="_blank"} est mis à jour.

## Que se passe-t-il lorsque je supprime d’[!DNL Salesforce] un champ qui était précédemment synchronisé avec Marketo ? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Si vous supprimez un champ dans SFDC, le champ n’est pas automatiquement supprimé dans Marketo, la synchronisation s’arrête simplement.
