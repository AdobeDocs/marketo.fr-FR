---
unique-page-id: 45417322
description: Suppression d’un lead ou d’un contact - Documents Marketo - Documentation du produit
title: Suppression d’un lead ou d’un contact
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 6%

---

# Suppression d’un lead ou d’un contact {#deleting-a-lead-or-contact}

Il y a quelques choses à savoir lorsqu’il s’agit de supprimer des prospects/contacts dans [!DNL Microsoft Dynamics].

* Marketo ne supprime pas automatiquement les personnes simplement parce que des prospects ont été supprimés en [!DNL Dynamics]. À la place, un indicateur de champ « Microsoft est supprimé » est défini sur « true ». Vous pouvez déclencher l’action hors de ce champ pour supprimer l’enregistrement dans Marketo, le cas échéant.

* Action de flux « Supprimer une personne » : supprime uniquement une personne dans Marketo (aucune option permettant de les supprimer également dans Dynamics n’est disponible).

* Si un prospect est supprimé dans Marketo (mais pas dans [!DNL Dynamics]) et mis à jour dans [!DNL Dynamics] par la suite, une nouvelle personne est créée dans Marketo (même adresse e-mail, nouvel ID de personne).

* Si un prospect est supprimé dans [!DNL Dynamics] (mais pas dans Marketo), puis s’exécute par la suite via l’action de flux « Synchroniser la personne avec Microsoft », un nouveau prospect est créé dans [!DNL Dynamics].
