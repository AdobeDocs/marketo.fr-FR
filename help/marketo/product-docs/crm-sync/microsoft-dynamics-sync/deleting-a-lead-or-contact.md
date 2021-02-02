---
unique-page-id: 45417322
description: Suppression d'une piste ou d'un contact - Documents marketing - Documentation du produit
title: Suppression d'une piste ou d'un contact
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Suppression d&#39;une piste ou d&#39;un contact {#deleting-a-lead-or-contact}

Il y a quelques éléments à savoir lorsqu&#39;il s&#39;agit de supprimer des pistes/contacts dans Microsoft Dynamics.

* Marketo ne supprime pas automatiquement les personnes simplement parce que les pistes ont été supprimées dans Dynamics. Au contraire, un indicateur de champ &quot;Microsoft is Deleted&quot; est défini sur true. Si vous le souhaitez, vous pouvez déclencher la suppression de ce champ afin de supprimer l’enregistrement dans Marketing.

* Action de flux &quot;Supprimer la personne&quot; : Cela supprime uniquement une personne dans Marketing (une option permettant de les supprimer également dans Dynamics n&#39;est pas disponible).

* Si une piste est supprimée dans Marketo (mais pas dans Dynamics) et qu&#39;elle est mise à jour dans Dynamics par la suite, elle créera une nouvelle personne dans Marketo (même adresse électronique, nouvel identifiant de personne).

* Si une piste est supprimée dans Dynamics (mais pas dans Marketo) et qu&#39;elle passe ensuite par l&#39;action de flux &quot;Synchroniser la personne avec Microsoft&quot;, elle créera une piste dans Dynamics.
