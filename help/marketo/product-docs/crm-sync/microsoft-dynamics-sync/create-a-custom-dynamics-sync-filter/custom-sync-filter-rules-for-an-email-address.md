---
unique-page-id: 10095307
description: Règles de filtre de synchronisation personnalisée pour une adresse électronique - Documents marketing - Documentation du produit
title: Règles de filtre de synchronisation personnalisée pour une adresse électronique
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Règles de filtre de synchronisation personnalisée pour une adresse électronique {#custom-sync-filter-rules-for-an-email-address}

Pour empêcher la synchronisation d’enregistrements qui n’ont pas d’adresse électronique, suivez ces règles.

* Lorsqu&#39;une piste est créée OU lorsque le champ d&#39;adresse électronique de la piste est mis à jour, vérifiez si elle a une adresse électronique et, le cas échéant, remplacez Sync par Mkto par **True**. Sinon, passez à **False**

* Lorsqu’un contact est créé OU lorsque le champ d’adresse électronique du contact est mis à jour, vérifiez si le contact a une adresse électronique et, le cas échéant, remplacez Sync par Mkto par **True** et remplacez Sync par **True** dans l’enregistrement de compte. Sinon, passez à **False**

* Lorsque le champ Nom de la Société du contact (parentcustomerid) est mis à jour, vérifiez si le champ Synchroniser avec Mkto du contact est vrai. Si tel est le cas, remplacez Sync par Mkto sur le compte par **True** également.
* Lorsque le champ Client potentiel de l&#39;opportunité (ID client) ou Contact (parent contactid) est mis à jour, vérifiez si le champ Synchroniser avec Mkto du compte est vrai ou si le champ Synchroniser avec Mkto du contact est vrai. Si tel est le cas, remplacez Sync par Mkto sur l’opportunité **True** également.
