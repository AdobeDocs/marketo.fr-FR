---
unique-page-id: 10095307
description: Règles de filtrage de synchronisation personnalisées pour une adresse électronique - Documents Marketo - Documentation du produit
title: Règles de filtre de synchronisation personnalisées pour une adresse électronique
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Règles de filtre de synchronisation personnalisées pour une adresse électronique {#custom-sync-filter-rules-for-an-email-address}

Pour empêcher la synchronisation d&#39;enregistrements qui ne possèdent pas d&#39;adresse email, suivez ces règles.

* Lorsqu’une piste est créée OU lorsque le champ de l’adresse électronique de la piste est mis à jour, vérifiez si elle comporte une adresse électronique et, si c’est le cas, remplacez Synchroniser avec Mkto par **[!UICONTROL True]**. Sinon, remplacez-le par **[!UICONTROL False]**.

* Lors de la création d’un contact OU de la mise à jour du champ de l’adresse électronique du contact, vérifiez si le contact possède une adresse électronique et, le cas échéant, remplacez Synchroniser avec le Mkto par **[!UICONTROL True]** et remplacez Synchroniser avec le Mkto par **[!UICONTROL True]** dans l’enregistrement du compte. Sinon, remplacez-vous par **[!UICONTROL False]**.

* Lorsque le champ Nom de la société du contact (parentcustomerid) est mis à jour, vérifiez si le champ Synchroniser avec le contact est vrai. Si tel est le cas, remplacez également Synchroniser avec Mkto sur le compte par **[!UICONTROL True]**.

* Lorsque le champ Client potentiel (customerid) de l&#39;opportunité ou Contact (parentcontactid) est mis à jour, vérifiez si le champ Synchroniser avec le Mkto du compte est vrai ou si le champ Synchroniser avec le Mkto du contact est vrai. Si tel est le cas, remplacez Synchroniser avec Mkto sur l’opportunité de **[!UICONTROL True]** également.
