---
unique-page-id: 2953459
description: Synchronisation de SFDC - Synchronisation de compte - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Synchronisation des comptes
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 2%

---

# Synchronisation SFDC : synchronisation de compte {#sfdc-sync-account-sync}

Marketo synchronise également les informations de votre compte avec [!DNL Salesforce]. Voici quelques informations spécifiques à connaître !

## De quelle manière les informations sont-elles synchronisées ? {#which-way-does-the-information-sync}

Un seul moyen : de SFDC à Marketo.

## Comment fonctionnent les mises à jour ? {#how-do-the-updates-work}

Si vous mettez à jour le champ Compte d’un contact dans Marketo, les valeurs de tous les contacts appartenant à ce compte dans Marketo sont modifiées. Il n’est pas synchronisé avec SFDC. Cependant, la prochaine fois que ce compte sera mis à jour dans SFDC, les modifications remplaceront toutes les informations du compte dans Marketo.

## Un contact peut-il appartenir à plusieurs comptes ?  {#can-a-contact-belong-to-multiple-accounts}

Non. Un compte peut avoir plusieurs contacts, un contact ne peut avoir qu’un seul compte.

## Puis-je créer des comptes à partir de Marketo ? {#can-i-create-accounts-from-marketo}

La plupart du temps, non. Cependant, si vous utilisez l’étape de flux [ Convertir la personne ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} pour une personne, un nouveau contact, un nouveau compte et une nouvelle opportunité seront créés.

>[!CAUTION]
>
>Cette étape de flux présente un cas d’utilisation très limité. Si vous n&#39;êtes pas sûr, vous ne devriez probablement pas l&#39;utiliser.

## Une modification apportée à un champ de compte dans [!DNL Salesforce] entraîne-t-elle la création d’un journal d’activité Modifier la valeur des données pour chaque contact ?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Surtout, oui. Cependant, si un compte comporte plus de 5 000 contacts et qu’un champ de ce compte change dans SFDC, nous synchronisons la modification, mais n’enregistrons pas l’activité pour plus de 5 000 contacts.
