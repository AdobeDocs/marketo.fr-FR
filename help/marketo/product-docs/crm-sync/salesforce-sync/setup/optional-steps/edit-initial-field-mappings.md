---
unique-page-id: 4719287
description: Modifier les mappages de champs initiaux - Documents Marketo - Documentation du produit
title: Modifier les mappages de champs initiaux
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Modifier les mappages de champs initiaux {#edit-initial-field-mappings}

>[!NOTE]
>
>Cette fonctionnalité est accessible uniquement avant la synchronisation initiale avec Salesforce. Une fois le bouton **[!UICONTROL Synchroniser maintenant]** enfoncé, cela ne peut plus être effectué.

Lors de la synchronisation initiale avec Salesforce, Marketo Engage combine automatiquement les champs personnalisés portant le même nom dans un seul champ du côté Marketo afin de garantir que les données peuvent être échangées avec les objets Lead et Contact dans le CRM. Cet article explique comment personnaliser ces mappages.

## Mapper les champs non mappés {#map-unmapped-fields}

Lorsque vous voyez un champ dans le dossier [!UICONTROL Champs non mappés], cela signifie qu’il n’est pas mappé à un champ similaire sur le prospect ou le contact dans Salesforce. Vous pouvez réparer ça.

1. Cliquez sur **[!UICONTROL Modifier les mappages]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Ouvrez le dossier **[!UICONTROL Unmapped Custom Fields]** .

   ![](assets/two.png)

1. Faites glisser un champ personnalisé non mappé sur un autre pour les mapper ensemble.

   >[!NOTE]
   >
   >Vous pouvez uniquement modifier les mappages de champs personnalisés. Les mappages de champs standard ne peuvent pas être modifiés.

   ![](assets/three.png)

1. Cliquez sur **[!UICONTROL Terminer les mappages]** lorsque vous avez terminé.

   ![](assets/four.png)

## Rompre le mappage existant {#break-existing-mapping}

Si vous disposez de champs portant le même nom sur l’objet de piste et de contact, Marketo les mappe automatiquement. Vous pouvez les considérer comme différents et contenir des données différentes. Brisez le mappage comme cela.

1. Cliquez sur **[!UICONTROL Modifier les mappages]**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Sélectionnez un champ mappé et cliquez sur **[!UICONTROL Rompre le mappage]** pour séparer les champs.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Cliquez sur **[!UICONTROL Terminer les mappages]** lorsque vous avez terminé.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Beau ! La synchronisation initiale est presque terminée.

## Réinitialiser le schéma {#reset-schema}

1. Si vous apportez des modifications au schéma dans Salesforce lorsque vous travaillez sur les mappages, vous pouvez extraire les modifications en cliquant sur **[!UICONTROL Réinitialiser le schéma]**.

   * Toutes les modifications de mappage seront réinitialisées !
   * La réinitialisation du schéma ajoute uniquement les champs, et non les supprime (même si vous les masquez de l’utilisateur de synchronisation).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
