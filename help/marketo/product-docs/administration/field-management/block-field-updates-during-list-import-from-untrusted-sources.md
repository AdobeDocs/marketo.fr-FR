---
unique-page-id: 2360335
description: Bloquer les mises à jour de champ lors de l’importation de liste à partir de sources non approuvées - Documents Marketo - Documentation du produit
title: Bloquer les mises à jour des champs lors de l’import de liste à partir de sources non approuvées
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 9%

---

# Bloquer les mises à jour des champs lors de l’import de liste à partir de sources non approuvées {#block-field-updates-during-list-import-from-untrusted-sources}

Vous pouvez faire davantage confiance aux données de certaines listes qu’à celles d’autres. Parfois, vous avez des données douteuses et vous voulez les utiliser si le champ est vide, mais pas s’il existe une valeur existante. Pour ce faire, vous pouvez bloquer les mises à jour des champs dans les champs clés.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Blocage Des Mises À Jour De Champs Provenant De Sources Non Approuvées {#blocking-field-updates-from-untrusted-sources}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Cliquez sur **[!UICONTROL Gestion des champs]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Recherchez le champ souhaité, sélectionnez-le, puis sous **[!UICONTROL Actions de champ]**, cliquez sur **[!UICONTROL Bloquer les mises à jour de champ]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Cochez **[!UICONTROL Liste Importer une source non approuvée]** et cliquez sur **[!UICONTROL Appliquer]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Vous pouvez protéger les champs de toutes les listes, qu&#39;elles soient approuvées ou non, en cochant également la case **[!UICONTROL Source approuvée d&#39;importation de liste]**.

Répétez les étapes ci-dessus pour tous les autres champs que vous souhaitez protéger des listes non approuvées.

## Exécution d’un import de liste non approuvé {#running-an-untrusted-list-import}

1. Lors de l’exécution de l’import de votre liste, veillez à sélectionner **[!UICONTROL Non approuvé]** si vous souhaitez que tous les champs configurés à l’étape précédente soient sécurisés.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Pour obtenir des instructions détaillées sur l’importation de listes, voir [Importer une liste de personnes](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Beau travail ! Vous savez maintenant comment protéger les champs clés des listes non approuvées.
