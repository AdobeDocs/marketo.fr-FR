---
unique-page-id: 2953465
description: Synchronisation SFDC - Conversion d’un prospect en contact dans Salesforce - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Conversion d’un prospect en contact dans Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# Synchronisation SFDC : conversion d’un prospect en contact dans Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imaginez trois scénarios différents dans Salesforce : (n’utilisez pas l’[étape de flux Convertir une personne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} en Marketo Engage)

1. Conversion d&#39;une piste en **nouveau contact et nouveau compte**
1. Conversion d&#39;une piste en **nouveau contact** dans un **compte existant**

1. Conversion d&#39;une piste en **contact existant** dans un **compte existant** (ce fonctionnement est identique à la [fusion](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

Dans les trois cas, vous obtenez **1 contact et aucune piste dans Salesforce et 1 contact et aucune personne dans Marketo.**

Dans Marketo, l’enregistrement aura désormais un type SFDC = Contact.

>[!TIP]
>
>Lors de la conversion dans Salesforce, assurez-vous que vos [champs personnalisés de piste sont bien mappés](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}. Vous ne souhaitez pas perdre de données.

Vous pouvez déclencher et filtrer l’affichage à l’aide des options suivantes : &quot;Le prospect est converti&quot; et &quot;Le prospect a été converti&quot;.
