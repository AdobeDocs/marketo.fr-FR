---
unique-page-id: 2360291
description: Bloquer les mises à jour d’un champ - Documents Marketo - Documentation du produit
title: Bloquer les mises à jour d’un champ
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Bloquer les mises à jour d&#39;un champ {#block-updates-to-a-field}

Le blocage des mises à jour d’un champ vous permet d’écrire une seule fois dans le champ, puis de conserver la valeur d’origine pour la durée de vie du champ. Cela peut s’avérer utile pour un champ comme Source de personne.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à **Admin** et cliquez sur **Gestion des champs**.

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. Recherchez le champ, sélectionnez-le, puis sous **Actions de champ**, cliquez sur **Bloquer les mises à jour de champ**.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Vous pouvez également bloquer les mises à jour des [champs personnalisés des membres du Programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Sélectionnez les **Sources d&#39;entrée** que vous souhaitez bloquer et cliquez sur **Appliquer**.

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >Lors d’une importation de liste, l’état d’un champ bloqué dans la Prévisualisation d’importation ne s’affiche que si le champ est automatiquement reconnu par Marketo en fonction du nom du champ correspondant exactement à __ (ou si des alias sont établis). Si le champ est sélectionné manuellement dans la liste déroulante Champ Marketo, l’état bloqué ne s’affiche pas dans la Prévisualisation d’importation, mais le blocage des mises à jour de ce champ est toujours implémenté.
