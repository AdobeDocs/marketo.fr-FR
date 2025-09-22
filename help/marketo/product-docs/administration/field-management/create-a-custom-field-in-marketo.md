---
unique-page-id: 2360287
description: Création d’un champ personnalisé dans Marketo - Documents Marketo - Documentation du produit
title: Créer un champ personnalisé dans Marketo
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 6%

---

# Créer un champ personnalisé dans Marketo {#create-a-custom-field-in-marketo}

Si vous avez besoin d’un nouveau champ personnalisé dans Marketo Engage pour stocker/capturer des données, voici comment en créer un.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. Cliquez sur **[!UICONTROL Gestion des champs]**.

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >Si vous souhaitez que les champs soient synchronisés avec votre CRM, créez-les dans le CRM et elles seront automatiquement créées dans Marketo.

1. Cliquez sur **[!UICONTROL Nouveau champ personnalisé]**.

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. Choisissez l’_[!UICONTROL Objet]_.

   ![](assets/create-a-custom-field-in-marketo-4.png)

   >[!NOTE]
   >
   >Bien que vous ne puissiez pas sélectionner vous-même l’objet _Company_, vous pouvez en faire la demande en contactant le support technique de [Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

1. Choisissez le champ _[!UICONTROL Type]_. Cela modifiera son rendu dans les listes dynamiques et les formulaires dans Marketo.

   >[!TIP]
   >
   >Consultez le [Glossaire des types de champs personnalisés](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

   ![](assets/create-a-custom-field-in-marketo-5.png)

1. Saisissez le _[!UICONTROL Nom]_ tel que vous souhaitez qu’il apparaisse dans Marketo (le _[!UICONTROL Nom de l’API]_ est généré automatiquement). Choisissez avec soin, car il ne peut pas être renommé après avoir été enregistré. Cliquez sur **[!UICONTROL Créer]** lorsque vous avez terminé.

>[!CAUTION]
>
>Les noms de champ ne peuvent pas commencer par les caractères suivants : **. &amp; +[]**

![](assets/create-a-custom-field-in-marketo-6.png)

>[!NOTE]
>
>Le nom de l’API est utilisé par l’API SOAP et d’autres processus principaux.

Vous pouvez désormais utiliser ce champ personnalisé dans les formulaires, les étapes de flux et les listes dynamiques.
