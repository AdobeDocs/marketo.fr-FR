---
unique-page-id: 2360335
description: Empêchez le remplacement des champs clés lors des imports de liste à partir de sources non approuvées afin de protéger les données existantes.
title: Bloquer les mises à jour des champs lors de l’import de liste à partir de sources non approuvées
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
TQID: https://experienceleague.adobe.com/cT1pOoWjR-UdHLqNJwhwgR9R12ciIa95q1xHPTf7rBY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 205
ht-degree: 10%

---

# Bloquer les mises à jour des champs lors de l’import de liste à partir de sources non approuvées {#block-field-updates-during-list-import-from-untrusted-sources}

Vous pouvez faire davantage confiance aux données de certaines listes qu’à celles d’autres. Parfois, vous disposez de données douteuses et souhaitez accepter les données si le champ est vide, mais pas s’il existe une valeur existante. Pour ce faire, vous pouvez bloquer les mises à jour des champs dans les champs clés.

>[!NOTE]
>
>**Autorisations d’administration requises**

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

Les champs clés sont désormais protégés des imports de listes non approuvés.
