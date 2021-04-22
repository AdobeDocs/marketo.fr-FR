---
unique-page-id: 45417322
description: Suppression d'une piste ou d'un contact - Documents Marketo - Documentation du produit
title: Suppression d'une piste ou d'un contact
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Suppression d&#39;une piste ou d&#39;un contact {#deleting-a-lead-or-contact}

Il y a quelques éléments à savoir lorsqu&#39;il s&#39;agit de supprimer des pistes/contacts dans Microsoft Dynamics.

* Marketo ne supprime pas automatiquement les personnes simplement parce que les pistes ont été supprimées dans Dynamics. Au contraire, un indicateur de champ &quot;Microsoft is Deleted&quot; est défini sur true. Si vous le souhaitez, vous pouvez déclencher la suppression de ce champ dans Marketo.

* Action de flux &quot;Supprimer la personne&quot; : Ceci supprime uniquement une personne dans Marketo (une option pour les supprimer également dans Dynamics n&#39;est pas disponible).

* Si une piste est supprimée dans Marketo (mais pas dans Dynamics) et qu&#39;elle est mise à jour dans Dynamics par la suite, elle créera une nouvelle personne dans Marketo (même adresse électronique, nouvel identifiant de personne).

* Si une piste est supprimée dans Dynamics (mais pas dans Marketo) et s&#39;exécute ensuite par le biais de l&#39;action de flux &quot;Synchroniser la personne avec Microsoft&quot;, elle créera une piste dans Dynamics.
