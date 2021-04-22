---
unique-page-id: 7515133
description: Synchronisation SFDC - Fusionner une piste/un contact/une personne - Marketo Docs - Documentation sur le produit
title: Synchronisation SFDC - Fusionner une piste/un contact/une personne
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 1%

---

# Synchronisation SFDC : Fusionner une piste, un contact ou une personne {#sfdc-sync-merging-a-lead-contact-person}

Parfois, il est préférable de simplement liste les règles. C&#39;est parti:

* Lorsque vous fusionnez deux pistes dans **Salesforce**, la synchronisation normale indique à Marketo et les pistes sont fusionnées automatiquement en tant que personnes dans Marketo.
* La fusion de deux personnes dans **Marketo** appelle en fait le même processus que leur fusion comme pistes dans Salesforce. Il fonctionne toujours automatiquement.
* La fusion d&#39;une **piste (personne) dans un contact** fonctionne de la même manière. Vous finissez avec un seul contact des deux côtés.
* Lors de la fusion, le score par défaut est additionné.

>[!NOTE]
>
>Fusion de 3 pistes (personnes) avec des scores de 10 chacune, donnera un résultat de 1 piste (personne) avec un score de 30.

* Les valeurs de champ conflictuelles proviennent de l&#39;&quot;enregistrement gagnant&quot;. (Enregistrer = le prospect ou le contact résultant)
* Si le &quot;record perdant&quot; (celui qui est en train de disparaître) avait une valeur et que le record gagnant n&#39;en a aucune, nous garderons le record perdant. En d&#39;autres termes, &quot;Une valeur vaut mieux qu&#39;aucune valeur.&quot;
* Tous les éléments du journal des activités sont fusionnés.

>[!NOTE]
>
>Explorez en profondeur pour plus d&#39;informations sur [la fusion de personnes à Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
