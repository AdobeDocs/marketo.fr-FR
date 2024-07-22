---
unique-page-id: 2360335
description: Mises à jour de champ de bloc pendant l’importation de liste à partir de sources non approuvées - Documents Marketo - Documentation du produit
title: Mises à jour de champ de bloc pendant l’importation de liste à partir de sources non approuvées
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Mises à jour de champ de bloc pendant l’importation de liste à partir de sources non approuvées {#block-field-updates-during-list-import-from-untrusted-sources}

Vous pouvez faire plus confiance aux données de certaines listes que d’autres. Il arrive que vous ayez des données discutables et que vous souhaitiez les extraire si le champ est vide, mais pas s’il existe une valeur. Pour ce faire, bloquez les mises à jour des champs sur les champs clés.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Blocage des mises à jour de champ à partir de sources non approuvées {#blocking-field-updates-from-untrusted-sources}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Cliquez sur **[!UICONTROL Gestion des champs]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Recherchez le champ de votre choix, sélectionnez-le, puis, sous **[!UICONTROL Actions de champ]**, cliquez sur **[!UICONTROL Bloquer les mises à jour de champ]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Cochez **[!UICONTROL List Import untrust source]** et cliquez sur **[!UICONTROL Apply]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Vous pouvez protéger les champs de toutes les listes, qu’ils soient de confiance ou non, en cochant également la case **[!UICONTROL Source de confiance d’import de liste]**.

Répétez les étapes ci-dessus pour tous les autres champs que vous souhaitez protéger des listes non approuvées.

## Exécution d’une importation de liste non approuvée {#running-an-untrusted-list-import}

1. Lors de l’exécution de l’importation de votre liste, veillez à sélectionner **[!UICONTROL Non approuvé]** si vous souhaitez que tous les champs que vous avez configurés à l’étape précédente soient sûrs.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Pour obtenir des instructions détaillées sur l&#39;importation de listes, voir [Importer une liste de personnes](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Beau travail ! Vous savez maintenant comment protéger les champs clés des listes non approuvées.
