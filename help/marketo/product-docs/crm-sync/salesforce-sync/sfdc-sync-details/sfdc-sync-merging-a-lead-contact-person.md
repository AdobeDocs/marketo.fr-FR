---
unique-page-id: 7515133
description: Synchronisation SFDC - Fusionner une piste/un contact/une personne - Documents marketing - Documentation du produit
title: Synchronisation SFDC - Fusionner une piste/un contact/une personne
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Synchronisation SFDC : Fusionner une piste, un contact ou une personne {#sfdc-sync-merging-a-lead-contact-person}

Parfois, il est préférable de simplement liste les règles. Et voici :

* Lorsque vous fusionnez deux pistes dans **Salesforce**, la synchronisation normale indique à Marketo et les pistes sont fusionnées automatiquement en tant que personnes dans Marketo.
* La fusion de deux personnes dans **Marketo** appelle en fait le même processus que leur fusion comme pistes dans Salesforce. Il fonctionne toujours automatiquement.
* La fusion d&#39;une **piste (personne) dans un contact** fonctionne de la même manière. Vous vous retrouvez avec un seul contact de part et d&#39;autre.
* Lors de la fusion, le score par défaut est additionné.

>[!NOTE]
>
>**Exemple**
>
>Fusion de 3 pistes (personnes) avec des scores de 10 chacune, donnera un résultat de 1 piste (personne) avec un score de 30.

* Les valeurs de champ conflictuelles proviennent de l&#39;&quot;enregistrement gagnant&quot;. (Enregistrer = le prospect ou le contact résultant)
* Si le &quot;record perdant&quot; (celui qui est en train de disparaître) avait une valeur et que le record gagnant n&#39;en a aucune, nous garderons le record perdant. En d&#39;autres termes, &quot;Une valeur vaut mieux qu&#39;aucune valeur.&quot;
* Tous les éléments du journal des activités sont fusionnés.

>[!NOTE]
>
>**Plongée profonde**
>
>Explorez en profondeur pour plus d&#39;informations sur [la fusion de personnes dans Marketo](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).

