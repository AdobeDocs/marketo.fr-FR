---
unique-page-id: 10093192
description: Créer des objets personnalisés sur le marché - Documents marketing - Documentation du produit
title: Créer des objets personnalisés marketing
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# Créer des objets personnalisés marketing {#create-marketo-custom-objects}

Utilisez des objets personnalisés dans Marketing pour effectuer le suivi de mesures spécifiques à votre entreprise. Il peut s&#39;agir de n&#39;importe quoi, des voitures, des cours, de tout ce que vous souhaitez modéliser sur Marketo pour exécuter vos campagnes.

>[!NOTE]
>
>Vous pouvez configurer des objets personnalisés pour qu’ils fonctionnent sur la base d’un-à-plusieurs ou de plusieurs-à-plusieurs. Vous créez l’objet initial de la même manière, mais les étapes sont différentes lorsque vous débuts ajouter des champs à l’objet. Pour plus d’informations, voir [Présentation des objets](understanding-marketo-custom-objects.md) personnalisés de marketing.

>[!NOTE]
>
>Vous ne pouvez pas créer, modifier ou supprimer un lien ou un champ de déduplication une fois que l’objet personnalisé a été approuvé.

## Création d’un objet personnalisé pour une structure de type &quot;un à plusieurs&quot; {#create-a-custom-object-for-a-one-to-many-structure}

Cet exemple montre un objet personnalisé Car, à utiliser dans une structure de type &quot;un à plusieurs&quot;. Par la suite, vous allez créer un objet personnalisé de cours et un objet intermédiaire à utiliser dans une structure de type &quot;plusieurs à plusieurs&quot;.

1. Cliquez sur **Admin**, puis dans Gestion **de la** base de données, sélectionnez **Marketo Custom Objects**.

   ** ![](assets/image2016-1-18-13-3a12-3a19.png)

   **

1. Cliquez sur **Nouvel objet** personnalisé.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >L’onglet Objets personnalisés du marketing affiche tous les objets personnalisés sur la droite, ainsi que les détails de tous les objets approuvés, y compris le nombre d’enregistrements et de champs lors de la dernière mise à jour.

1. Saisissez un nom d’affichage. Le nom de l’API et le nom du pluriel sont renseignés automatiquement. Entrez une description (facultatif).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs lorsque vous les créez, mais après les avoir enregistrés, vous pouvez uniquement modifier le champ Nom du pluriel et le curseur **Afficher dans les détails** de piste.

1. Appuyez sur le **Afficher dans le détail des pistes **pour afficher **Afficher** si vous souhaitez vue des données d&#39;objet personnalisées sur la page Base de données des pistes. Cliquez sur **Enregistrer**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. Les informations sur les objets personnalisés affichent le contenu que vous avez saisi. Notez qu’il est à l’état Brouillon.

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   L’étape suivante consiste à ajouter des champs pour [créer votre objet](add-marketo-custom-object-fields.md)personnalisé.

   >[!NOTE]
   >
   >Vous ne pouvez renseigner les objets personnalisés de marketing que par le biais d’une importation de liste ou de l’ [API](http://developers.marketo.com/documentation/rest/).

## Création d’un objet personnalisé pour une structure de type &quot;plusieurs à plusieurs&quot; {#create-a-custom-object-for-a-many-to-many-structure}

Cet exemple montre un objet personnalisé de cours, que vous utiliserez pour créer une relation de type &quot;plusieurs à plusieurs&quot; entre les personnes/sociétés et les cours. Une fois terminé, vous allez créer un objet intermédiaire pour le connecter à des personnes ou des sociétés de votre base de données.

>[!NOTE]
>
>Pour une relation de type &quot;plusieurs à plusieurs&quot;, il n’est pas nécessaire de créer un lien dans l’objet personnalisé. Vous allez plutôt ajouter deux liens à l’objet intermédiaire (voir ci-dessous).

1. Cliquez sur **Admin**, puis dans Gestion **de la** base de données, sélectionnez **Marketo Custom Objects**.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Cliquez sur **Nouvel objet** personnalisé.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Saisissez un nom d’affichage. Le nom de l’API et le nom du pluriel sont renseignés automatiquement. Entrez une description (facultatif).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs lorsque vous les créez, mais après les avoir enregistrés, vous pouvez uniquement modifier le champ Nom du pluriel et le curseur **Afficher dans les détails** de piste.

1. Appuyez sur le **Afficher dans les détails de la piste **pour afficher Afficher si vous souhaitez vue des données d&#39;objet personnalisées sur la page Base de données de pistes. Cliquez sur **Enregistrer**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. Les informations sur les objets personnalisés affichent le contenu que vous avez saisi. Notez qu’il est à l’état Brouillon.

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >Vous ne pouvez renseigner les objets personnalisés de marketing que par le biais d’une importation de liste ou de l’ [API](http://developers.marketo.com/documentation/rest/).

L&#39;étape suivante consiste à créer votre objet intermédiaire (voir ci-dessous). Mais avant cela, vous devez créer un champ avec lequel créer un lien.

## Création d’un objet intermédiaire {#create-an-intermediary-object}

Utilisez un objet intermédiaire pour connecter un objet personnalisé à des personnes ou des sociétés. Dans cet exemple, il est utilisé pour connecter des cours de votre objet personnalisé de cours à des personnes ou des sociétés de votre base de données.

>[!NOTE]
>
>Il n’est pas nécessaire de créer un objet intermédiaire pour une structure d’objet personnalisé de type &quot;un à plusieurs&quot;.

1. Cliquez sur **Admin**, puis dans Gestion **de la** base de données, sélectionnez Objets **** personnalisés de marketing à.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Cliquez sur **Nouvel objet** personnalisé.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Saisissez un nom d’affichage. Le nom de l’API et le nom du pluriel sont renseignés automatiquement. Entrez une description (facultatif).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >Vous pouvez modifier ces champs lorsque vous les créez, mais une fois enregistrés, vous pouvez uniquement modifier le champ Nom du pluriel et le curseur Afficher dans les détails de piste.

1. Appuyez sur le curseur **Afficher dans les détails** de la piste pour afficher Afficher si vous souhaitez vue des données d&#39;objet personnalisées sur la page Base de données de piste. Cliquez sur **Enregistrer**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. Les informations sur les objets personnalisés affichent le contenu que vous avez saisi. Notez qu’il est à l’état Brouillon.

   L’étape suivante consiste à [ajouter des champs](add-marketo-custom-object-link-fields.md) de lien pour connecter votre objet intermédiaire à une personne/société et à un objet personnalisé.

>[!MORELIKETHIS]
>
>* [Ajouter les champs d&#39;objet personnalisé Marketo](add-marketo-custom-object-fields.md)
>* [Ajouter les champs de lien d’objet personnalisé Marketo](add-marketo-custom-object-link-fields.md)
>* [Compréhension des objets personnalisés de marketing](understanding-marketo-custom-objects.md)

>



