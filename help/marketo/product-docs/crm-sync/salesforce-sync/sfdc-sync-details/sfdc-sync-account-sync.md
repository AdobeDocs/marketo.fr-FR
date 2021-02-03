---
unique-page-id: 2953459
description: Synchronisation SFDC - Synchronisation des comptes - Documents marketing - Documentation du produit
title: Synchronisation SFDC - Synchronisation des comptes
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# Synchronisation SFDC : Synchronisation du compte {#sfdc-sync-account-sync}

Marketo synchronise également les informations de votre compte avec Salesforce. Voici quelques éléments spécifiques que vous devriez savoir !

## De quelle façon les informations sont-elles synchronisées ? {#which-way-does-the-information-sync}

Un seul moyen : de la DDC à Marketo.

## Comment fonctionnent les mises à jour ? {#how-do-the-updates-work}

Si vous mettez à jour un champ Compte pour un contact dans Marketo, il modifie les valeurs de tous les contacts appartenant à ce compte dans Marketo. Il n’est pas synchronisé avec SFDC. Cependant, la prochaine fois que ce compte sera mis à jour dans SFDC, les modifications remplaceront toutes les informations de compte dans Marketing Cloud.

## Un contact peut-il appartenir à plusieurs comptes ?  {#can-a-contact-belong-to-multiple-accounts}

Non. Un compte peut avoir plusieurs contacts, un contact ne peut avoir qu&#39;un seul compte.

## Puis-je créer des comptes à partir de Marketo ? {#can-i-create-accounts-from-marketo}

Surtout, non. Cependant, si vous utilisez l&#39;étape de flux [Convertir une personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) sur une personne, cela créera un nouveau contact, un nouveau compte et une nouvelle opportunité.

>[!CAUTION]
>
>Cette étape de flux présente un cas d’utilisation très limité. Si vous n&#39;êtes pas sûr, vous ne devriez probablement pas l&#39;utiliser.

## Est-ce qu&#39;une modification d&#39;un champ de compte dans Salesforce entraîne un Journal d&#39;Activité de la valeur des données de modification pour chaque contact ?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Surtout, oui. Cependant, si un compte a plus de 5 000 contacts et qu’un champ sur ce compte change dans la DDC, nous synchronisons la modification mais ne consignons pas l’activité pour plus de 5 000 contacts.
