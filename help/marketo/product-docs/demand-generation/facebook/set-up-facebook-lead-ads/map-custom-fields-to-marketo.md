---
unique-page-id: 12983101
description: Mappage de champs personnalisés à Marketo - Documents Marketo - Documentation du produit
title: Mapper des champs personnalisés à Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 6%

---

# Mapper des champs personnalisés à Marketo {#map-custom-fields-to-marketo}

Vous pouvez collecter davantage d’informations que les informations standard stockées par défaut [!DNL Facebook], telles que la fréquence d’utilisation de votre service de diffusion en ligne. Pour ce faire, vous pouvez [créer des questions personnalisées](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) dans vos annonces de prospects [!DNL Facebook].

Cependant, **Marketo ne commencera pas automatiquement à collecter ces données**. Pour que Marketo puisse commencer à capturer des valeurs de champ personnalisées, vous **devez** mapper ces champs personnalisés à un champ dans Marketo.

Voici comment configurer ce paramètre dans la zone LaunchPoint de l’administrateur.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone Administration et cliquez sur **[!UICONTROL LaunchPoint]**. Sous Services installés, recherchez et modifiez **[!UICONTROL Publicités de leads Facebook]**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Laissez le compte autorisé tel quel, et n’apportez **de modifications**. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Comme auparavant, laissez les pages sélectionnées telles quelles (n’apportez **de modifications**. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. C’est à ce stade que vous mappez le champ [!DNL Facebook] personnalisé à votre champ Marketo. Cliquez sur **[!UICONTROL Ajouter].**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Dans la nouvelle ligne, saisissez le nom de votre champ personnalisé [!DNL Facebook].

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Seuls les champs qui ont été enregistrés dans des modèles de formulaire [!DNL Facebook] s’affichent en tant qu’options ici.

1. Cliquez dans la colonne **[!UICONTROL Champ Marketo]**. Saisissez pour rechercher le champ à mapper. Une fois le champ sélectionné, cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Si vous ne disposez pas déjà d’un champ dans Marketo auquel mapper le champ [!DNL Facebook], découvrez comment [créer des champs personnalisés](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Vous **devez** passer par ce processus pour tout nouveau champ de [!DNL Facebook] afin que Marketo puisse collecter les données.
