---
unique-page-id: 10093192
description: Création d’objets personnalisés Marketo - Documents Marketo - Documentation du produit
title: Créer des objets personnalisés Marketo
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Créer des objets personnalisés Marketo {#create-marketo-custom-objects}

Utilisez des objets personnalisés dans Marketo pour effectuer le suivi de mesures propres à votre entreprise. Il peut s’agir de voitures, de cours, de tout ce que vous souhaitez modéliser dans Marketo pour exécuter vos campagnes.

>[!NOTE]
>
>Vous pouvez configurer des objets personnalisés pour qu’ils fonctionnent de un à plusieurs ou de plusieurs à plusieurs. Vous créez l’objet initial de la même manière, mais les étapes sont différentes lorsque vous commencez à ajouter des champs à l’objet. Voir  [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) pour plus d’informations.

>[!NOTE]
>
>Une fois l’objet personnalisé approuvé, vous ne pouvez pas créer, modifier ou supprimer un lien ou un champ de déduplication.

## Création d’un objet personnalisé pour une structure de type &quot;un à plusieurs&quot; {#create-a-custom-object-for-a-one-to-many-structure}

Cet exemple présente un objet personnalisé Car, à utiliser dans une structure de type &quot;un à plusieurs&quot;. Vous allez ensuite créer un objet personnalisé de cours et un objet intermédiaire à utiliser dans une structure de type &quot;plusieurs à plusieurs&quot;.

1. Cliquez sur **Administration** et dans **Gestion de base de données** select **Objets personnalisés Marketo**.

   ![](assets/image2016-1-18-13-3a12-3a19.png)

1. Cliquez sur **Nouvel objet personnalisé**.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >L’onglet Objets personnalisés Marketo affiche tous les objets personnalisés à droite, ainsi que les détails de tous les objets approuvés, y compris le nombre d’enregistrements et de champs lors de la mise à jour la plus récente.

1. Saisissez un nom d’affichage. Le nom de l’API et le nom du pluriel sont renseignés automatiquement. Saisissez une description (facultatif).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs lorsque vous les créez, mais une fois qu’ils ont été enregistrés, vous ne pouvez modifier que le champ Nom du pluriel et le champ **Afficher dans les détails de piste** curseur.

1. Extrayez le **Afficher dans les détails de piste** curseur sur lequel afficher **Afficher** si vous souhaitez afficher des données d’objet personnalisées sur la page Base de données de piste . Cliquez sur **Enregistrer**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. Les informations d’objet personnalisé affichent le contenu que vous avez saisi. Notez qu’il est à l’état En création .

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   L’étape suivante consiste à ajouter des champs à [créer votre objet personnalisé ;](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Vous ne pouvez renseigner les objets personnalisés Marketo que par le biais d’une importation de liste ou de la variable [API](https://developers.marketo.com/documentation/rest/).

## Création d’un objet personnalisé pour une structure multiple-à-multiple {#create-a-custom-object-for-a-many-to-many-structure}

Cet exemple illustre un objet personnalisé de cours que vous utiliserez pour créer une relation de type &quot;plusieurs à plusieurs&quot; entre les personnes/entreprises et les cours. Lorsque vous aurez terminé, vous allez créer un objet intermédiaire pour le connecter aux personnes ou aux entreprises de votre base de données.

>[!NOTE]
>
>Dans le cas d’une relation multiple-à-multiple, il n’est pas nécessaire de créer un lien dans l’objet personnalisé. Vous allez ajouter deux liens à l’objet intermédiaire (voir ci-dessous).

1. Cliquez sur **Administration** et dans **Gestion de base de données** select **Objets personnalisés Marketo**.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Cliquez sur **Nouvel objet personnalisé**.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Saisissez un nom d’affichage. Le nom de l’API et le nom du pluriel sont renseignés automatiquement. Saisissez une description (facultatif).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs lorsque vous les créez, mais une fois qu’ils ont été enregistrés, vous ne pouvez modifier que le champ Nom du pluriel et le champ **Afficher dans les détails de piste** curseur.

1. Extrayez le **Afficher dans les détails de piste** curseur sur lequel afficher **Afficher** si vous souhaitez afficher des données d’objet personnalisées sur la page Base de données de piste . Cliquez sur **Enregistrer**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. Les informations d’objet personnalisé affichent le contenu que vous avez saisi. Notez qu’il est à l’état En création .

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >Vous ne pouvez renseigner les objets personnalisés Marketo que par le biais d’une importation de liste ou de la variable [API](https://developers.marketo.com/documentation/rest/).

L’étape suivante permet de créer l’objet intermédiaire (voir ci-dessous). Avant cela, vous devez créer un champ vers lequel vous souhaitez établir un lien.

## Création d’un objet intermédiaire {#create-an-intermediary-object}

Utilisez un objet intermédiaire pour connecter un objet personnalisé à des personnes ou à des entreprises. Dans cet exemple, il est utilisé pour connecter des cours dans votre objet personnalisé de cours à des personnes ou des entreprises de votre base de données.

>[!NOTE]
>
>Vous n’avez pas besoin de créer un objet intermédiaire pour une structure d’objet personnalisé de type &quot;un à plusieurs&quot;.

1. Cliquez sur **Administration** et dans **Gestion de base de données**, sélectionnez **Objets personnalisés Marketo**.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Cliquez sur **Nouvel objet personnalisé**.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Saisissez un nom d’affichage. Le nom de l’API et le nom du pluriel sont renseignés automatiquement. Saisissez une description (facultatif).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs lorsque vous les créez, mais une fois qu’ils ont été enregistrés, vous pouvez uniquement modifier le champ Nom du pluriel et le curseur Afficher dans les détails de la piste .

1. Extrayez le **Afficher dans les détails de piste** curseur sur lequel afficher **Afficher** si vous souhaitez afficher des données d’objet personnalisées sur la page Base de données de piste . Cliquez sur **Enregistrer**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. Les informations d’objet personnalisé affichent le contenu que vous avez saisi. Notez qu’il est à l’état En création .

   L’étape suivante permet d’effectuer les opérations suivantes : [ajouter des champs de lien](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) pour connecter l’objet intermédiaire à une personne/société et à un objet personnalisé.

>[!MORELIKETHIS]
>
>* [Ajout de champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Ajout de champs de lien d’objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

