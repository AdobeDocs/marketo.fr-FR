---
unique-page-id: 2360335
description: Bloquer les mises à jour des champs pendant l'importation de Listes à partir de sources non approuvées - Documents marketing - Documentation du produit
title: Bloquer les mises à jour des champs pendant l'importation de Listes à partir de sources non approuvées
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Bloquer les mises à jour des champs pendant l&#39;importation de Listes à partir de sources non approuvées {#block-field-updates-during-list-import-from-untrusted-sources}

Vous pouvez faire plus confiance aux données de certaines listes que d’autres. Vous disposez parfois de données douteuses et souhaitez les saisir si le champ est vide, mais pas s’il existe une valeur. Pour ce faire, vous pouvez bloquer les mises à jour de champs sur les champs clés.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Bloquer les mises à jour des champs à partir de sources non approuvées {#blocking-field-updates-from-untrusted-sources}

1. Accédez à **Admin** et cliquez sur **Gestion des champs**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Recherchez le champ de votre choix, sélectionnez-le, puis sous **Actions de champ**, cliquez sur **Bloquer les mises à jour de champ**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Cochez **Liste Importer la source non approuvée** et cliquez sur **Appliquer**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Vous pouvez protéger les champs de toutes les listes, qu&#39;elles soient approuvées ou non, en vérifiant également **Liste Importer la source approuvée**.

Répétez les étapes ci-dessus pour tous les autres champs que vous souhaitez protéger des listes non approuvées.

## Exécution d&#39;une importation de Liste non approuvée {#running-an-untrusted-list-import}

1. Lors de l’exécution de l’importation de votre liste, veillez à sélectionner **Non approuvé** si vous souhaitez que tous les champs configurés à l’étape précédente soient sûrs.

   ![](assets/importpersondetails.jpg)

Pour obtenir des instructions détaillées sur l’importation de listes, voir [Importation d’une Liste de personnes](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Bon travail ! Vous savez maintenant comment protéger les champs clés des listes non approuvées.
