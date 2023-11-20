---
unique-page-id: 7515133
description: Synchronisation SFDC - Fusion d’un prospect/contact/personne - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Fusion d’un prospect/contact/personne
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 1%

---

# Synchronisation SFDC : fusion d’un prospect/contact/personne {#sfdc-sync-merging-a-lead-contact-person}

Parfois, il est préférable de simplement lister les règles. C&#39;est parti:

* Lorsque vous fusionnez deux pistes dans **Salesforce**, la synchronisation normale indique à Marketo Engage et les pistes sont fusionnées automatiquement en tant que personnes dans Marketo.
* Fusion de deux personnes dans **Marketo** invoque le même processus que leur fusion comme prospects dans Salesforce. Il fonctionne toujours automatiquement.
* Fusion d’une **diriger (personne) vers un contact** fonctionne de la même manière. Vous obtenez un seul contact des deux côtés.
* Lors de la fusion, le score par défaut est additionné.

>[!NOTE]
>
>Fusion de 3 pistes (personnes) avec des scores de 10 chacune, générera un résultat de 1 piste (personne) avec un score de 30.

* Les valeurs de champ en conflit proviennent de l’enregistrement &quot;gagnant&quot;. (Enregistrer = prospect ou contact résultant)
* Si le &quot;enregistrement perdant&quot; (celui qui disparaît) avait une valeur et que le record gagnant n&#39;a pas de valeur, nous conserverons le record perdant. En d’autres termes, &quot;Une valeur vaut mieux qu’aucune valeur.&quot;
* Tous les éléments du journal d’activité sont fusionnés.

>[!NOTE]
>
>Exploration approfondie pour en savoir plus [fusion de personnes dans Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}.
