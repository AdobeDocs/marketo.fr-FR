---
unique-page-id: 10093192
description: Création D’Objets Personnalisés Marketo - Documents Marketo - Documentation Du Produit
title: Créer des objets personnalisés Marketo
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 2%

---

# Créer des objets personnalisés Marketo {#create-marketo-custom-objects}

Utilisez des objets personnalisés dans Marketo pour effectuer le suivi des mesures spécifiques à votre entreprise. Cela peut être n’importe quelle voiture, n’importe quel cours, n’importe quel modèle que vous souhaitez modéliser dans Marketo pour exécuter vos campagnes.

>[!NOTE]
>
>Vous pouvez configurer des objets personnalisés pour qu’ils fonctionnent sur une base un-à-plusieurs ou plusieurs-à-plusieurs. Vous créez l’objet initial de la même manière, mais les étapes sont différentes lorsque vous commencez à ajouter des champs à l’objet . Voir [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) pour plus d’informations.

>[!NOTE]
>
>Vous ne pouvez pas créer, modifier ou supprimer un lien ou un champ de déduplication une fois que l’objet personnalisé est approuvé.

## Créer un objet personnalisé pour une structure de type « un à plusieurs » {#create-a-custom-object-for-a-one-to-many-structure}

Cet exemple illustre un objet personnalisé Car à utiliser dans une structure de type « un à plusieurs ». Plus tard, vous allez créer un objet personnalisé de cours et un objet intermédiaire à utiliser dans une structure multiple-à-multiple.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-marketo-custom-objects-1.png)

1. Cliquez sur **[!UICONTROL Objets personnalisés Marketo]**.

   ![](assets/create-marketo-custom-objects-2.png)

1. Cliquez sur **[!UICONTROL Nouvel objet personnalisé]**.

   ![](assets/create-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >L&#39;onglet [!UICONTROL Objets personnalisés Marketo] affiche tous les objets personnalisés à droite, ainsi que les détails de tous les objets approuvés, y compris le nombre d&#39;enregistrements et de champs lors de la mise à jour la plus récente.

1. Saisissez un [!UICONTROL Nom d’affichage]. Le [!UICONTROL nom de l’API] et le [!UICONTROL nom au pluriel] sont renseignés automatiquement. Saisissez une [!UICONTROL &#x200B; Description &#x200B;] (facultatif).

   ![](assets/create-marketo-custom-objects-4.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs au moment de leur création, mais une fois enregistrés, vous ne pouvez modifier que le champ [!UICONTROL Nom au pluriel] et le curseur **[!UICONTROL Afficher dans les détails du prospect]**.

1. Faites glisser le curseur **[!UICONTROL Afficher dans les détails du prospect]** pour afficher **[!UICONTROL Afficher]** si vous souhaitez afficher des données d’objet personnalisées sur la page Base de données. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/create-marketo-custom-objects-5.png)

1. Les informations sur l’objet personnalisé affichent le contenu que vous avez saisi. Notez qu’il est à l’état **[!UICONTROL Brouillon]**.

   ![](assets/create-marketo-custom-objects-6.png)

   L’étape suivante consiste à ajouter des champs pour [créer votre objet personnalisé](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Vous pouvez uniquement remplir les objets personnalisés Marketo par le biais d’un import de liste ou de l’[API](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api).

## Création d’un objet personnalisé pour une structure multiple-à-multiple {#create-a-custom-object-for-a-many-to-many-structure}

Cet exemple montre un objet personnalisé de cours que vous utiliserez pour créer une relation multiple-à-multiple entre des personnes/sociétés et des cours. Une fois que vous avez terminé, vous allez créer un objet intermédiaire pour le connecter aux personnes ou aux sociétés de votre base de données.

>[!NOTE]
>
>Pour une relation multiple-à-multiple, il n’est pas nécessaire de créer un lien dans l’objet personnalisé. À la place, vous ajoutez deux liens à l’objet intermédiaire (voir ci-dessous).

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-marketo-custom-objects-7.png)

1. Cliquez sur **[!UICONTROL Objets personnalisés Marketo]**.

   ![](assets/create-marketo-custom-objects-8.png)

1. Cliquez sur **[!UICONTROL Nouvel objet personnalisé]**.

   ![](assets/create-marketo-custom-objects-9.png)

1. Saisissez un [!UICONTROL Nom d’affichage]. Le [!UICONTROL nom de l’API] et le [!UICONTROL nom au pluriel] sont renseignés automatiquement. Saisissez une [!UICONTROL &#x200B; Description &#x200B;] (facultatif).

   ![](assets/create-marketo-custom-objects-10.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs au moment de leur création, mais une fois enregistrés, vous ne pouvez modifier que le champ [!UICONTROL Nom au pluriel] et le curseur **[!UICONTROL Afficher dans les détails du prospect]**.

1. Faites glisser le curseur **[!UICONTROL Afficher dans les détails du prospect]** pour afficher **[!UICONTROL Afficher]** si vous souhaitez afficher des données d’objet personnalisées sur la page Base de données. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/create-marketo-custom-objects-11.png)

1. Les informations sur l’objet personnalisé affichent le contenu que vous avez saisi. Notez qu’il est à l’état **[!UICONTROL Brouillon]**.

   ![](assets/create-marketo-custom-objects-12.png)

   >[!NOTE]
   >
   >Vous pouvez uniquement remplir les objets personnalisés Marketo par le biais d’un import de liste ou de l’[API](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api).

L’étape suivante consiste à créer votre objet intermédiaire (voir ci-dessous). Mais avant cela, vous devez créer un champ auquel créer un lien.

## Créer un objet intermédiaire {#create-an-intermediary-object}

Utilisez un objet intermédiaire pour connecter un objet personnalisé à des personnes ou à des sociétés. Dans cet exemple, elle est utilisée pour connecter les cours de votre objet personnalisé de cours à des personnes ou des sociétés de votre base de données.

>[!NOTE]
>
>Vous n’avez pas besoin de créer un objet intermédiaire pour une structure d’objet personnalisée un-à-plusieurs.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-marketo-custom-objects-13.png)

1. Cliquez sur **[!UICONTROL Objets personnalisés Marketo]**.

   ![](assets/create-marketo-custom-objects-14.png)

1. Cliquez sur **[!UICONTROL Nouvel objet personnalisé]**.

   ![](assets/create-marketo-custom-objects-15.png)

1. Saisissez un [!UICONTROL Nom d’affichage]. Le [!UICONTROL nom de l’API] et le [!UICONTROL nom au pluriel] sont renseignés automatiquement. Saisissez une [!UICONTROL &#x200B; Description &#x200B;] (facultatif).

   ![](assets/create-marketo-custom-objects-16.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs au moment de leur création, mais une fois enregistrés, vous ne pouvez modifier que le champ [!UICONTROL Nom au pluriel] et le curseur [!UICONTROL Afficher dans les détails du prospect].

1. Faites glisser le curseur **[!UICONTROL Afficher dans les détails du prospect]** pour afficher **Afficher** si vous souhaitez afficher des données d’objet personnalisées sur la page Base de données. Cliquez sur **Enregistrer**

   ![](assets/create-marketo-custom-objects-17.png)

1. Les informations sur l’objet personnalisé affichent le contenu que vous avez saisi. Notez qu’il est à l’état **[!UICONTROL Brouillon]**.

   L’étape suivante consiste à [ajouter des champs de lien](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) pour connecter votre objet intermédiaire à une personne/société et à un objet personnalisé.

>[!MORELIKETHIS]
>
>* [Ajouter des champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Ajouter des champs de lien d’objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
