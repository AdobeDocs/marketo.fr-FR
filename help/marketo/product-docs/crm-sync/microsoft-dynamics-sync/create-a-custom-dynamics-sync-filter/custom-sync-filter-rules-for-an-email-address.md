---
unique-page-id: 10095307
description: Règles de filtre de synchronisation personnalisé pour une adresse e-mail - Documents Marketo - Documentation du produit
title: Règles de filtre de synchronisation personnalisé pour une adresse e-mail
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Règles de filtre de synchronisation personnalisé pour une adresse e-mail {#custom-sync-filter-rules-for-an-email-address}

Pour empêcher la synchronisation des enregistrements qui n’ont pas d’adresse e-mail, suivez ces règles.

* Lorsqu’un prospect est créé OU lorsque le champ d’adresse électronique du prospect est mis à jour, vérifiez si le prospect possède une adresse électronique et, dans l’affirmative, définissez Synchronisation sur Mkto sur **[!UICONTROL Vrai]**. Sinon, remplacez par **[!UICONTROL False]**

* Lorsqu’un contact est créé OU lorsque le champ d’adresse e-mail du contact est mis à jour, vérifiez si le contact possède une adresse e-mail et, dans l’affirmative, remplacez Synchronisation par Mkto par **[!UICONTROL Vrai]** et Synchronisation par Mkto par **[!UICONTROL Vrai]** dans l’enregistrement Compte . Sinon, remplacez par **[!UICONTROL False]**

* Lorsque le champ Nom de la société du contact (parentcustomerid) est mis à jour, vérifiez si le champ Synchroniser avec Moto du contact est vrai. Si c’est le cas, définissez également Synchronisation sur Mkto sur le compte sur **[!UICONTROL Vrai]**
* Lorsque le champ Client potentiel (customerid) ou Contact (parentcontactid) de l’opportunité est mis à jour, vérifiez si le champ Synchroniser avec Mkto du compte est vrai ou si le champ Synchroniser avec Mkto du contact est vrai. Si c’est le cas, définissez Synchronisation sur Mkto à l’occasion de **[!UICONTROL Vrai]** également
