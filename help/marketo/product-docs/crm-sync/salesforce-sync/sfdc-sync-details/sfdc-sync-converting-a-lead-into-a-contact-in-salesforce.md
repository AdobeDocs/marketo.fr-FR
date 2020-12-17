---
unique-page-id: 2953465
description: Synchronisation SFDC - Conversion d'une piste en contact dans Salesforce - Docs marketing - Documentation du produit
title: Synchronisation SFDC - Conversion d'une piste en contact dans Salesforce
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Synchronisation SFDC : Conversion d&#39;une piste en contact dans Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imaginez trois scénarios différents dans Salesforce : (n’utilisant pas l’[étape de flux Convertir une personne](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) dans Marketo)

1. Conversion d&#39;une piste en **nouveau contact et nouveau compte**
1. Conversion d&#39;une piste en **nouveau contact** dans un **compte existant**

1. Conversion d&#39;un prospect en **contact existant** dans un **compte existant** (ce comportement est identique à [fusion](sfdc-sync-merging-a-lead-contact-person.md))

Dans les trois cas, vous obtenez **1 contact et aucun prospect dans Salesforce et 1 contact et aucune personne dans Marketo.**

Dans Marketo, l’enregistrement aura désormais un type SFDC = Contact.

>[!TIP]
>
>Lors de la conversion dans Salesforce, vérifiez que vos champs personnalisés [de piste sont bien mappés ](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Vous ne voulez pas perdre de données.

Vous pouvez déclencher et filtrer à l’aide de : &quot;Le prospect est converti&quot; et &quot;Le prospect a été converti&quot;.