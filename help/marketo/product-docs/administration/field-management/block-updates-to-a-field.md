---
unique-page-id: 2360291
description: Bloquer les mises à jour d’un champ - Documents Marketo - Documentation du produit
title: Bloquer les mises à jour d’un champ
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 2%

---

# Bloquer les mises à jour d’un champ {#block-updates-to-a-field}

Le blocage des mises à jour d’un champ vous permet d’écrire sur le champ une seule fois, puis de conserver la valeur d’origine pendant la durée de vie du champ. Cela peut s’avérer utile pour un champ comme [!UICONTROL Source de personne].

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/block-updates-to-a-field-1.png)

1. Cliquez sur **[!UICONTROL Gestion des champs]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Recherchez le champ, sélectionnez-le, puis sous **[!UICONTROL Actions de champ]**, cliquez sur **[!UICONTROL Mises à jour du champ de bloc]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Vous pouvez bloquer les mises à jour de [Champs personnalisés des membres du programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) ainsi que .

1. Sélectionnez la **[!UICONTROL Sources d’entrée]** vous souhaitez bloquer et cliquer sur **[!UICONTROL Appliquer]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Lors d&#39;un import de liste, l&#39;état d&#39;un champ bloqué dans l&#39;aperçu de l&#39;import ne s&#39;affiche que si le champ est automatiquement reconnu par Marketo en fonction du nom du champ correspondant. _what_ (ou si des alias sont établis). Si le champ est sélectionné manuellement dans la liste déroulante Champ Marketo , l’état bloqué ne s’affiche pas dans l’ aperçu de l’importation, mais le blocage des mises à jour de ce champ est toujours implémenté.
