---
unique-page-id: 7515133
description: Découvrez comment fonctionnent les prospects, les contacts et les personnes qui fusionnent dans Salesforce et Marketo. Découvrez les règles de fusion pour les scores, les valeurs de champ et les journaux d’activité.
title: Synchronisation de SFDC - Fusion d’un lead/contact/d’une personne
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 3%

---

# Synchronisation SFDC : fusion d’un lead/d’un contact/d’une personne {#sfdc-sync-merging-a-lead-contact-person}

Parfois, il est préférable de simplement énumérer les règles. Et voilà :

* Lorsque vous fusionnez deux prospects dans **[!DNL Salesforce]**, la synchronisation normale indique à Marketo que les prospects sont fusionnés automatiquement en tant que personnes dans Marketo.
* La fusion de deux personnes dans **Marketo** appelle en fait le même processus que la fusion en tant que prospects dans [!DNL Salesforce]. Cela fonctionne toujours automatiquement.
* La fusion d’un **prospect (personne) dans un contact** fonctionne de la même manière. Vous vous retrouvez avec un seul contact des deux côtés.
* Lors de la fusion, le score par défaut est additionné.

>[!NOTE]
>
>La fusion de 3 prospects (personnes) avec un score de 10 chacun donnera un résultat de 1 prospect (personne) avec un score de 30.

* Les valeurs de champ en conflit proviennent de l’« enregistrement gagnant ». (Enregistrement = lead ou contact résultant)
* Si le « dossier perdu » (celui qui disparaît) avait une valeur et que le dossier gagnant n&#39;en a aucune, nous conserverons le dossier perdu. En d’autres termes, « une certaine valeur est préférable à aucune valeur ».
* Tous les éléments du journal d’activité sont fusionnés.

>[!NOTE]
>
>Séance d’immersion pour en savoir plus sur [la fusion de personnes dans Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}.
