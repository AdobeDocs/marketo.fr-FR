---
unique-page-id: 45417322
description: Suppression d’un prospect ou d’un contact - Documents Marketo - Documentation du produit
title: Suppression d’un prospect ou d’un contact
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Suppression d’un prospect ou d’un contact {#deleting-a-lead-or-contact}

Quelques éléments à savoir lorsqu’il s’agit de supprimer des pistes/contacts dans Microsoft Dynamics.

* Marketo ne supprime pas automatiquement les personnes simplement parce que les pistes ont été supprimées dans Dynamics. L’indicateur &quot;Microsoft is Deleted&quot; du champ est défini sur true. Vous pouvez déclencher ce champ pour supprimer l’enregistrement dans Marketo si vous le souhaitez.

* Action de flux &quot;Supprimer la personne&quot; : Cela supprime uniquement une personne dans Marketo (une option pour la supprimer également dans Dynamics n’est pas disponible).

* Si une piste est supprimée dans Marketo (mais pas dans Dynamics) et est mise à jour dans Dynamics par la suite, elle créerait une nouvelle personne dans Marketo (même adresse électronique, nouvel ID de personne).

* Si une piste est supprimée dans Dynamics (mais pas dans Marketo) et qu’elle passe ensuite par l’action de flux &quot;Synchroniser la personne avec Microsoft&quot;, une nouvelle piste est créée dans Dynamics.
