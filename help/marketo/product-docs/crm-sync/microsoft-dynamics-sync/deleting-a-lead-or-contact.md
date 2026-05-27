---
unique-page-id: 45417322
description: Découvrez comment fonctionne la suppression des prospects et des contacts entre Microsoft Dynamics et Marketo. Utilisez l’indicateur Microsoft est supprimé et l’action de flux Supprimer la personne si nécessaire.
title: Suppression d’un lead ou d’un contact
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/4BwBuLQFJ2pRehuS8EqW-UrEcg5sVeqcstu3azh0NvQ
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 167
ht-degree: 5%

---

# Suppression d’un lead ou d’un contact {#deleting-a-lead-or-contact}

Il y a quelques choses à savoir lorsqu’il s’agit de supprimer des prospects/contacts dans [!DNL Microsoft Dynamics].

* Marketo ne supprime pas automatiquement les personnes uniquement parce que les prospects ont été supprimés en [!DNL Dynamics]. À la place, un indicateur de champ « Microsoft est supprimé » est défini sur « true ». Vous pouvez déclencher l’action hors de ce champ pour supprimer l’enregistrement dans Marketo, le cas échéant.

* Action de flux « Supprimer une personne » : supprime uniquement une personne dans Marketo (aucune option permettant de les supprimer également dans Dynamics n’est disponible).

* Si un prospect est supprimé dans Marketo (mais pas dans [!DNL Dynamics]) et mis à jour dans [!DNL Dynamics] par la suite, une nouvelle personne est créée dans Marketo (même adresse e-mail, nouvel ID de personne).

* Si un prospect est supprimé dans [!DNL Dynamics] (mais pas dans Marketo), puis s’exécute par la suite via l’action de flux « Synchroniser la personne avec Microsoft », un nouveau prospect est créé dans [!DNL Dynamics].
