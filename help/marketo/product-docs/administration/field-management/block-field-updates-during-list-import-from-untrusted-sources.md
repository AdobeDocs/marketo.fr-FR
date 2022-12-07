---
unique-page-id: 2360335
description: Mises à jour de champ de bloc pendant l’importation de liste à partir de sources non approuvées - Documents Marketo - Documentation du produit
title: Mises à jour de champ de bloc pendant l’importation de liste à partir de sources non approuvées
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 2%

---

# Mises à jour de champ de bloc pendant l’importation de liste à partir de sources non approuvées {#block-field-updates-during-list-import-from-untrusted-sources}

Vous pouvez faire plus confiance aux données de certaines listes que d’autres. Il arrive que vous ayez des données discutables et que vous souhaitiez les extraire si le champ est vide, mais pas s’il existe une valeur. Pour ce faire, bloquez les mises à jour des champs sur les champs clés.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Blocage des mises à jour de champ à partir de sources non approuvées {#blocking-field-updates-from-untrusted-sources}

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Cliquez sur **Gestion des champs**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Recherchez le champ de votre choix, sélectionnez-le, puis sous **Actions de champ**, cliquez sur **Mises à jour du champ de bloc**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Vérifier **Liste Importer une source non fiable** et cliquez sur **Appliquer**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Vous pouvez protéger les champs de toutes les listes, qu’ils soient de confiance ou non, en vérifiant également **Liste Importer une source de confiance**.

Répétez les étapes ci-dessus pour tous les autres champs que vous souhaitez protéger des listes non approuvées.

## Exécution d’une importation de liste non approuvée {#running-an-untrusted-list-import}

1. Lors de l’exécution de l’importation de votre liste, veillez à sélectionner **Non approuvé** si vous souhaitez que tous les champs configurés à l’étape précédente soient sûrs.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Pour obtenir des instructions détaillées sur l’importation de listes, voir [Importation d’une liste de personnes](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Beau travail ! Vous savez maintenant comment protéger les champs clés des listes non approuvées.
