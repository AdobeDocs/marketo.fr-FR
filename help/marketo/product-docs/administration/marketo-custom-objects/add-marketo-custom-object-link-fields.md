---
unique-page-id: 10097613
description: Ajout de champs de lien d’objet personnalisé Marketo - Documents Marketo - Documentation du produit
title: Ajout de champs de lien d’objet personnalisé Marketo
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
source-git-commit: a51ee0b2b513d50febbffd7e3a72874c5ef4679c
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 1%

---

# Ajout de champs de lien d’objet personnalisé Marketo {#add-marketo-custom-object-link-fields}

Lorsque vous créez des objets personnalisés, vous devez fournir des champs de lien pour connecter l’enregistrement d’objet personnalisé à l’enregistrement parent correct.

* Pour une structure personnalisée de type &quot;un à plusieurs&quot;, utilisez le champ de lien dans l’objet personnalisé pour le connecter à une personne ou à une entreprise.
* Pour une structure multiple-à-multiple, vous utilisez deux champs de lien, connectés à un objet intermédiaire créé séparément (qui est également un type d’objet personnalisé). Un lien se connecte aux personnes ou aux entreprises de votre base de données, tandis que l’autre se connecte à l’objet personnalisé. Dans ce cas, le champ de lien ne se trouve pas dans l’objet personnalisé lui-même.

## Création d’un champ de lien pour une structure de type &quot;un à plusieurs&quot; {#create-a-link-field-for-a-one-to-many-structure}

Voici comment créer un champ de lien dans un objet personnalisé pour une structure de type &quot;un à plusieurs&quot;.

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. Cliquez sur **Objets personnalisés Marketo**.

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. Sélectionnez l’objet personnalisé dans la liste.

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. Dans le **Champs** , cliquez sur **Nouveau champ**.

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. Nommez le champ de lien et ajoutez une description facultative. Veillez à sélectionner le type de données Lien .

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >Une fois l’objet personnalisé approuvé, vous ne pourrez pas revenir en arrière pour créer, modifier ou supprimer un lien ou un champ de déduplication.

1. Indiquez si l’objet de lien est destiné à un prospect (une personne) ou une société.

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >Si vous choisissez une piste, vous verrez l’identifiant, l’adresse électronique et les champs personnalisés dans la liste.
   >
   >Si vous choisissez société, vous verrez l’identifiant et tous les champs personnalisés dans la liste.

1. Sélectionnez le champ de lien auquel vous souhaitez vous connecter en tant que parent du nouveau champ.

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >Seuls les types de champ de chaîne sont pris en charge dans le champ de lien.

1. Cliquez sur **Enregistrez.**

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## Création d’un champ de lien pour une structure multiple-à-multiple {#create-a-link-field-for-a-many-to-many-structure}

Voici comment créer un champ de lien dans un objet intermédiaire à utiliser dans une structure multiple-à-multiple.

>[!PREREQUISITES]
>
>Vous devez avoir déjà créé l’objet intermédiaire et les objets personnalisés auxquels vous souhaitez le lier.

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. Cliquez sur **Objets personnalisés Marketo**.

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. Sélectionnez l’objet intermédiaire auquel vous souhaitez ajouter le champ.

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. Dans le **Champs** , cliquez sur **Nouveau champ**.

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. Vous devez créer deux champs de lien. Créez-les un par un. Tout d’abord, nommez le champ des membres de votre liste de base de données (leadID, par exemple). Ajoutez une description facultative. Veillez à sélectionner le type de données du lien.

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >Une fois l’objet personnalisé approuvé, vous ne pourrez pas revenir en arrière pour créer, modifier ou supprimer un lien ou un champ de déduplication.

1. Sélectionnez l’objet de lien de votre base de données, dans ce cas, &quot;Lead&quot;.

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. Sélectionnez le champ du lien auquel vous souhaitez vous connecter, dans ce cas, l&#39;identifiant.

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >Seuls les types de champ de chaîne sont pris en charge dans le champ de lien.

1. Cliquez sur **Enregistrez.**

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. Répétez cette procédure pour le deuxième lien vers votre objet personnalisé, dans cet exemple, courseID. Le nom de l’objet du lien est &quot;cours&quot; et le champ de lien est &quot;coursID&quot;. Comme vous avez déjà créé et approuvé l’objet personnalisé du cours, ces sélections sont disponibles dans les menus déroulants.

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. Créez d’autres champs que vous souhaitez utiliser dans votre objet intermédiaire, tels que enrollmentID ou grade.

## Utilisation d’objets personnalisés {#using-custom-objects}

L’étape suivante consiste à utiliser ces objets personnalisés dans les filtres de vos campagnes intelligentes. Avec une relation multiple-à-multiple, vous pouvez sélectionner plusieurs personnes/entreprises et plusieurs objets personnalisés. Dans l’exemple ci-dessous, toute personne de votre base de données qui correspond à ces critères sera répertoriée. Le champ coursename provient de l’objet personnalisé de cours et la note d’inscription provient de l’objet intermédiaire.

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [Ajout de champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Modification et suppression d’un objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Modification et suppression de champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)

