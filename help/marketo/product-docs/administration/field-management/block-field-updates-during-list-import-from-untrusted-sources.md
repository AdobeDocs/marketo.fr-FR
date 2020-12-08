---
unique-page-id: 2360335
description: Bloquer les mises à jour des champs pendant l'importation de Listes à partir de sources non approuvées - Documents marketing - Documentation du produit
title: Bloquer les mises à jour des champs pendant l'importation de Listes à partir de sources non approuvées
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Bloquer les mises à jour des champs pendant l&#39;importation de Listes à partir de sources non approuvées {#block-field-updates-during-list-import-from-untrusted-sources}

Vous pouvez faire plus confiance aux données de certaines listes que d’autres. Vous disposez parfois de données douteuses et souhaitez les saisir si le champ est vide, mais pas s’il existe une valeur. Pour ce faire, vous pouvez bloquer les mises à jour de champs sur les champs clés.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Blocage des mises à jour des champs à partir de sources non approuvées {#blocking-field-updates-from-untrusted-sources}

1. Accédez à **Admin** et cliquez sur Gestion des **** champs.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Recherchez le champ de votre choix, sélectionnez-le, puis sous Actions **de** champ, cliquez sur **Bloquer les mises à jour** de champ.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Cochez **Liste Importer une source** non approuvée et cliquez sur **Appliquer**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Vous pouvez protéger les champs de toutes les listes, qu’elles soient approuvées ou non, en cochant également **Liste Importer une source** approuvée.

Répétez les étapes ci-dessus pour tous les autres champs que vous souhaitez protéger des listes non approuvées.

## Exécution d&#39;une importation de Liste non approuvée {#running-an-untrusted-list-import}

1. Lors de l&#39;exécution de l&#39;importation de votre liste, veillez à sélectionner **Non approuvé **si vous souhaitez que tous les champs configurés à l&#39;étape précédente soient sûrs.

   ![](assets/importpersondetails.jpg)

Pour obtenir des instructions détaillées sur l’importation de listes, voir [Importation d’une Liste de personnes](../../../getting-started/quick-wins/import-a-list-of-people.md).

Bon travail ! Vous savez maintenant comment protéger les champs clés des listes non approuvées.
