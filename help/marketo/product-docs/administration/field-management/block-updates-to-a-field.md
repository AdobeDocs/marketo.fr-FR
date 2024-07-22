---
unique-page-id: 2360291
description: Bloquer les mises à jour d’un champ - Documents Marketo - Documentation du produit
title: Bloquer les mises à jour d’un champ
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Bloquer les mises à jour d’un champ {#block-updates-to-a-field}

Le blocage des mises à jour d’un champ vous permet d’écrire sur le champ une seule fois, puis de conserver la valeur d’origine pendant la durée de vie du champ. Cela peut s’avérer utile pour un champ tel que [!UICONTROL Person Source].

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/block-updates-to-a-field-1.png)

1. Cliquez sur **[!UICONTROL Gestion des champs]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Recherchez le champ, sélectionnez-le, puis sous **[!UICONTROL Actions de champ]**, cliquez sur **[!UICONTROL Bloquer les mises à jour de champ]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Vous pouvez également bloquer les mises à jour des [Champs personnalisés des membres du programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Sélectionnez les **[!UICONTROL sources d&#39;entrée]** que vous souhaitez bloquer et cliquez sur **[!UICONTROL Appliquer]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Lors de l&#39;import d&#39;une liste, l&#39;état d&#39;un champ bloqué dans l&#39;aperçu de l&#39;import ne s&#39;affiche que si le champ est automatiquement reconnu par Marketo en fonction du nom du champ correspondant à _exactement_ (ou si des alias sont définis). Si le champ est sélectionné manuellement dans la liste déroulante Champ Marketo , l’état bloqué ne s’affiche pas dans l’ aperçu de l’importation, mais le blocage des mises à jour de ce champ est toujours implémenté.
