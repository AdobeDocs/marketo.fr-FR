---
unique-page-id: 2953465
description: Synchronisation SFDC - Conversion d'une piste en contact dans Salesforce - Docs marketing - Documentation du produit
title: Synchronisation SFDC - Conversion d'une piste en contact dans Salesforce
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Synchronisation SFDC : Conversion d&#39;une piste en contact dans Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Imaginez trois scénarios différents dans Salesforce : (n’utilisant pas l’étape [de flux](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) Convertir une personne dans Marketo)

1. Conversion d&#39;une piste en un **nouveau contact et un nouveau compte**
1. Conversion d&#39;une piste en un **nouveau contact** dans un compte **existant**

1. Conversion d&#39;un prospect en contact **** existant dans un compte **** existant (ce comportement est identique à celui de la [fusion](sfdc-sync-merging-a-lead-contact-person.md))

Dans les trois cas, vous finissez avec **1 contact et aucun prospect dans Salesforce et 1 contact et aucune personne dans Marketo.**

Dans Marketo, l’enregistrement aura désormais un type SFDC = Contact.

>[!TIP]
>
>Lors de la conversion dans Salesforce, assurez-vous que vos champs personnalisés de [piste sont bien](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)mappés. Vous ne voulez pas perdre de données.

Vous pouvez déclencher et filtrer à l’aide de : &quot;Le prospect est converti&quot; et &quot;Le prospect a été converti&quot;.