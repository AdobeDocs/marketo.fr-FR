---
unique-page-id: 10095307
description: Règles de filtre de synchronisation personnalisée pour une adresse électronique - Docs Marketo - Documentation du produit
title: Règles de filtre de synchronisation personnalisée pour une adresse électronique
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Règles de filtre de synchronisation personnalisée pour une adresse électronique {#custom-sync-filter-rules-for-an-email-address}

Pour empêcher la synchronisation d’enregistrements qui n’ont pas d’adresse électronique, suivez ces règles.

* Lorsqu&#39;une piste est créée OU lorsque le champ de l&#39;adresse électronique de la piste est mis à jour, vérifiez si elle a une adresse électronique et, le cas échéant, remplacez Sync par Mkto par **True**. Sinon, passez à **False**

* Lorsqu’un contact est créé OU lorsque le champ d’adresse électronique du contact est mis à jour, vérifiez si le contact a une adresse électronique et, le cas échéant, remplacez Sync par Mkto par **True** et remplacez Sync par **True** dans l’enregistrement de compte. Sinon, passez à **False**

* Lorsque le champ Nom de la Société du contact (parentcustomerid) est mis à jour, vérifiez si le champ Synchroniser avec Mkto du contact est vrai. Si tel est le cas, remplacez Sync par Mkto sur le compte par **True** également.
* Lorsque le champ Client potentiel de l&#39;opportunité (ID client) ou Contact (parent contactid) est mis à jour, vérifiez si le champ Synchroniser avec Mkto du compte est vrai ou si le champ Synchroniser avec Mkto du contact est vrai. Si tel est le cas, remplacez Sync par Mkto sur l’opportunité **True** également.
