---
unique-page-id: 2953465
description: Découvrez ce qui se passe lorsque vous convertissez un prospect en contact dans Salesforce. Découvrez comment Marketo reflète la modification et utilisez des déclencheurs et des filtres Lead converti .
title: Synchronisation de SFDC - Conversion d’un prospect en contact dans Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/Z5ApDpLvZhGu3-DeZHwQanilG1WILGFQF7VnDxQikr4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 169
ht-degree: 0%

---

# Synchronisation SFDC : conversion d’un prospect en contact dans [!DNL Salesforce] {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Imaginez trois scénarios différents dans [!DNL Salesforce] : (sans utiliser l’étape [Convertir le flux de personnes](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) dans Marketo)

1. Convertir un lead en **nouveau contact et nouveau compte**
1. Convertir un prospect en **nouveau contact** dans un **compte existant**

1. Convertir un prospect en **contact existant** dans un **compte existant** (fonctionnement identique à [fusion](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

Dans les trois cas, vous vous retrouvez avec un contact **1 et aucun prospect dans [!DNL Salesforce] et 1 contact et aucune personne dans Marketo.**

Dans Marketo, l’enregistrement aura désormais un Type de SFDC = Contact.

>[!TIP]
>
>Lors de la conversion dans [!DNL Salesforce], assurez-vous que vos [champs personnalisés de prospect](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm) sont bien mappés. Vous ne voulez pas perdre de données.

Vous pouvez déclencher et filtrer en utilisant les options suivantes : « [!UICONTROL Lead converti] » et « [!UICONTROL Lead converti] ».
