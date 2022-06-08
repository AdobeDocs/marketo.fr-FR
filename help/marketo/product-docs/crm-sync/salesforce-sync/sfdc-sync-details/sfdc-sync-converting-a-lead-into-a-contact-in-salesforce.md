---
unique-page-id: 2953465
description: Synchronisation SFDC - Conversion d’un prospect en contact dans Salesforce - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Conversion d’un prospect en contact dans Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Synchronisation SFDC : Conversion d’un prospect en contact dans Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imaginez trois scénarios différents dans Salesforce : (sans utiliser la variable [Étape de flux Conversion de personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) dans Marketo)

1. Conversion d’une piste en **nouveau contact et nouveau compte**
1. Conversion d’une piste en **new contact** dans un **compte existant**

1. Conversion d’une piste en **contact existant** dans un **compte existant** (fonctionne de la même manière que [fusion](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

Dans les trois cas, vous obtenez **1 contact et aucun prospect dans Salesforce et 1 contact et aucune personne dans Marketo.**

Dans Marketo, l’enregistrement aura désormais un type SFDC = Contact.

>[!TIP]
>
>Lors de la conversion dans Salesforce, assurez-vous que la variable [les champs personnalisés de prospect sont bien mappés.](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Vous ne souhaitez pas perdre de données.

Vous pouvez déclencher et filtrer à l’aide des éléments suivants : &quot;Le prospect est converti&quot; et &quot;Le prospect a été converti&quot;.
