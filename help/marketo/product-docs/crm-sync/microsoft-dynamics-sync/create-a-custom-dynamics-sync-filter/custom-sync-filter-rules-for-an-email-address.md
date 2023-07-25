---
unique-page-id: 10095307
description: Règles de filtrage de synchronisation personnalisées pour une adresse électronique - Documents Marketo - Documentation du produit
title: Règles de filtre de synchronisation personnalisées pour une adresse électronique
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Règles de filtre de synchronisation personnalisées pour une adresse électronique {#custom-sync-filter-rules-for-an-email-address}

Pour empêcher la synchronisation d&#39;enregistrements qui ne possèdent pas d&#39;adresse email, suivez ces règles.

* Lors de la création d’une piste OU lorsque le champ de l’adresse électronique du prospect est mis à jour, vérifiez si l’adresse électronique du prospect est renseignée et, dans le cas contraire, remplacez Synchroniser avec le Mkto par **True**. Sinon, remplacez par **False**

* Lors de la création d’un contact OU lorsque le champ de l’adresse email du contact est mis à jour, vérifiez si le contact dispose d’une adresse email et, dans le cas contraire, remplacez Synchroniser avec le Mkto par **True** et remplacez Synchroniser par Marque **True** dans l’enregistrement Compte . Sinon, remplacez par **False**

* Lorsque le champ Nom de la société du contact (parentcustomerid) est mis à jour, vérifiez si le champ Synchroniser avec le contact est défini sur &quot;true&quot;. Si tel est le cas, remplacez Synchroniser par Mkto sur le compte par **True** également
* Lorsque le champ Client potentiel (customerid) de l’opportunité ou Contact (parentcontactid) est mis à jour, vérifiez si le champ Synchroniser avec le Mkto du compte est défini sur true ou si le champ Synchroniser avec le Mkto du contact est défini sur true. Si c’est le cas, modifiez Synchroniser avec Mkto sur l’opportunité de **True** également
