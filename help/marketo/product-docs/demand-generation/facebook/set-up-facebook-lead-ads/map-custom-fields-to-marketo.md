---
unique-page-id: 12983101
description: Mappage de champs personnalisés à Marketo - Documents Marketo - Documentation du produit
title: Mappage de champs personnalisés à Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Mappage de champs personnalisés à Marketo {#map-custom-fields-to-marketo}

Par défaut, vous pouvez collecter plus que les informations standard stockées par Facebook, comme la fréquence à laquelle une personne utilise votre service de diffusion en ligne. Pour ce faire, [créez des questions personnalisées](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) dans vos annonces publicitaires Facebook.

Cependant, **Marketo ne commencera pas automatiquement à collecter ces données**. Pour que Marketo commence à capturer des valeurs de champ personnalisées, vous **devez** les mapper à un champ dans Marketo.

Voici comment le configurer dans la zone LaunchPoint d’administration.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone Admin et cliquez sur **LaunchPoint**. Sous Services installés, recherchez et modifiez **Facebook Lead Ads**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Cliquez sur **Suivant**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Laissez le compte autorisé tel quel : **not** effectuez des modifications. Cliquez sur **Suivant**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Comme auparavant, laissez les pages sélectionnées telles quelles : **ne pas** apporter de modifications. Cliquez sur **Suivant**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. C’est là que vous mappez le champ Facebook personnalisé à votre champ Marketo. Cliquez sur **Ajouter.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Dans la nouvelle ligne, saisissez le nom de votre champ personnalisé Facebook.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Seuls les champs qui ont été enregistrés dans des modèles de formulaire Facebook s’affichent sous la forme d’options.

1. Cliquez dans la colonne **Champ Marketo** . Saisissez pour rechercher le champ à mapper. Une fois que vous avez sélectionné un champ, cliquez sur **Enregistrer**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Si vous ne disposez pas déjà d’un champ dans Marketo pour mapper le champ Facebook à, découvrez comment [créer des champs personnalisés](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Vous **devez** passer par ce processus pour tout nouveau champ Facebook afin que Marketo puisse rassembler les données.
