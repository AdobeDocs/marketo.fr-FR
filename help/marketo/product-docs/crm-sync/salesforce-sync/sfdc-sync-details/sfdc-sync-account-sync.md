---
unique-page-id: 2953459
description: Synchronisation SFDC - Synchronisation des comptes - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation des comptes
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# Synchronisation SFDC : synchronisation des comptes {#sfdc-sync-account-sync}

Marketo Engage synchronise également les informations de votre compte avec Salesforce. Voici quelques choses spécifiques que vous devriez savoir !

## De quelle manière les informations se synchronisent-elles ? {#which-way-does-the-information-sync}

Une seule solution : de la SFDC à Marketo.

## Comment fonctionnent les mises à jour ? {#how-do-the-updates-work}

Si vous mettez à jour un champ Compte pour un contact dans Marketo, cela modifie les valeurs de tous les contacts appartenant à ce compte dans Marketo. Il ne se synchronise pas avec SFDC. Toutefois, la prochaine fois que ce compte sera mis à jour dans la collecte de données régionale, les modifications remplaceront toutes les informations de compte dans Marketo.

## Un contact peut-il appartenir à plusieurs comptes ?  {#can-a-contact-belong-to-multiple-accounts}

Non. Un compte peut avoir de nombreux contacts, un contact ne peut avoir qu&#39;un seul compte.

## Puis-je créer des comptes à partir de Marketo ? {#can-i-create-accounts-from-marketo}

Surtout, non. Cependant, si vous utilisez la variable [Convertir une personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} l’étape de flux sur une personne crée un contact, un nouveau compte et une nouvelle opportunité.

>[!CAUTION]
>
>Cette étape de flux présente un cas d’utilisation très limité. Si vous n&#39;êtes pas sûr, vous ne devriez probablement pas l&#39;utiliser.

## Une modification d’un champ de compte dans Salesforce entraîne-t-elle un journal d’activité de modification de la valeur des données pour chaque contact ?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Surtout, oui. Cependant, si un compte a plus de 5000 contacts et qu’un champ de ce compte change dans la DDC, nous synchronisons les modifications mais ne consignons pas l’activité pour plus de 5000 contacts.
