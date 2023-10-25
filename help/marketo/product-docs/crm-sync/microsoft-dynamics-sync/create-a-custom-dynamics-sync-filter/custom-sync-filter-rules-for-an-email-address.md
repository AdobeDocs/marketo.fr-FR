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

* Lorsqu’une piste est créée OU lorsque le champ de l’adresse électronique de la piste est mis à jour, vérifiez si elle comporte une adresse électronique et, si c’est le cas, remplacez Synchroniser avec le Mkto. **[!UICONTROL True]**. Sinon, remplacez par **[!UICONTROL False]**.

* Lors de la création d’un contact OU lorsque le champ de l’adresse email du contact est mis à jour, vérifiez si le contact dispose d’une adresse email et, dans le cas contraire, remplacez Synchroniser avec le Mkto par **[!UICONTROL True]** et remplacez Synchroniser par Marque **[!UICONTROL True]** dans l’enregistrement Compte . Sinon, remplacez par **[!UICONTROL False]**.

* Lorsque le champ Nom de la société du contact (parentcustomerid) est mis à jour, vérifiez si le champ Synchroniser avec le contact est vrai. Si tel est le cas, remplacez Synchroniser par Mkto sur le compte par **[!UICONTROL True]** également.

* Lorsque le champ Client potentiel (customerid) de l&#39;opportunité ou Contact (parentcontactid) est mis à jour, vérifiez si le champ Synchroniser avec le Mkto du compte est vrai ou si le champ Synchroniser avec le Mkto du contact est vrai. Si c’est le cas, modifiez Synchroniser avec Mkto sur l’opportunité de **[!UICONTROL True]** également.
