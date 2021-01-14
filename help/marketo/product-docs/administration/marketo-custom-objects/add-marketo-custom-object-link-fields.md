---
unique-page-id: 10097613
description: Champs de lien d'objet personnalisé Ajouter Marketo - Documents marketing - Documentation du produit
title: Ajouter les champs de lien d’objet personnalisé Marketo
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---


# Champs de lien d&#39;objet personnalisé du marketing d&#39;Ajoute {#add-marketo-custom-object-link-fields}

Lorsque vous créez des objets personnalisés, vous devez fournir des champs de lien pour connecter l’enregistrement d’objet personnalisé à l’enregistrement parent correct.

* Pour une structure personnalisée de type &quot;un à plusieurs&quot;, utilisez le champ de lien de l’objet personnalisé pour la connecter à une personne ou une société.
* Pour une structure de type &quot;plusieurs à plusieurs&quot;, vous utilisez deux champs de lien, connectés à partir d’un objet intermédiaire créé séparément (qui est également un type d’objet personnalisé). Un lien se connecte aux personnes ou aux sociétés de votre base de données et l’autre à l’objet personnalisé. Dans ce cas, le champ de lien n’est pas situé dans l’objet personnalisé lui-même.

## Créer un champ de lien pour une structure de type &quot;un à plusieurs&quot; {#create-a-link-field-for-a-one-to-many-structure}

Voici comment créer un champ de lien dans un objet personnalisé pour une structure de type &quot;un à plusieurs&quot;.

1. Cliquez sur **Admin**, puis dans **Gestion de la base de données**, sélectionnez **Objets personnalisés marketing**.

   ![](assets/image2016-1-18-13-3a25-3a11.png)

1. Sélectionnez l’objet personnalisé dans la liste.

   ![](assets/image2016-1-14-15-3a6-3a2.png)

1. Dans l&#39;onglet **Champs**, cliquez sur **Nouveau champ**.

   ![](assets/image2015-9-17-14-3a9-3a19.png)

1. Attribuez un nom au champ de lien et ajoutez une description facultative. Veillez à sélectionner le type de données Lien.

   ![](assets/image2015-10-5-13-3a24-3a57.png)

   >[!CAUTION]
   >
   >Vous ne pourrez pas revenir en arrière et créer, modifier ou supprimer un lien ou un champ de déduplication une fois l’objet personnalisé approuvé.

1. Indiquez si l&#39;objet de lien est destiné à une piste (personne) ou à une société.

   ![](assets/image2015-10-5-13-3a28-3a1.png)

   >[!NOTE]
   >
   >Si vous choisissez une piste, vous verrez l’ID, l’adresse électronique et les champs personnalisés dans la liste.
   >
   >Si vous choisissez société, vous verrez l’ID et les champs personnalisés dans la liste.

1. Sélectionnez le champ de lien auquel vous souhaitez vous connecter en tant que parent du nouveau champ.

   ![](assets/image2015-10-5-13-3a30-3a6.png)

   >[!NOTE]
   >
   >Seuls les types de champ de chaîne sont pris en charge dans le champ de lien.

1. Cliquez sur **Enregistrer.**

   ![](assets/image2015-10-5-13-3a34-3a0.png)

## Créer un champ de lien pour une structure de type &quot;plusieurs à plusieurs&quot; {#create-a-link-field-for-a-many-to-many-structure}

Voici comment créer un champ de lien dans un objet intermédiaire pour une utilisation dans une structure de type &quot;plusieurs à plusieurs&quot;.

>[!PREREQUISITES]
>
>Vous devez avoir déjà créé l’objet intermédiaire et les objets personnalisés vers lesquels vous souhaitez le lier.

1. Cliquez sur **Admin**, puis dans **Gestion de la base de données**, sélectionnez **Objets personnalisés marketing**.

   ![](assets/image2016-1-18-9-3a8-3a14.png)

1. Sélectionnez l’objet intermédiaire auquel vous souhaitez ajouter le champ.

   ![](assets/image2016-1-18-9-3a10-3a29.png)

1. Dans l&#39;onglet **Champs**, cliquez sur **Nouveau champ**.

   ![](assets/image2016-1-18-9-3a31-3a43.png)

1. Vous devez créer deux champs de lien. Créez-les un par un. Tout d&#39;abord, nommez le champ des membres de votre liste de base de données (prospectID, par exemple). Ajoutez une description facultative. Veillez à sélectionner le type de données du lien.

   ![](assets/image2016-1-18-9-3a38-3a59.png)

   >[!CAUTION]
   >
   >Vous ne pourrez pas revenir en arrière et créer, modifier ou supprimer un lien ou un champ de déduplication une fois l’objet personnalisé approuvé.

1. Sélectionnez l&#39;objet de lien de votre base de données, dans ce cas, Piste.

   ![](assets/image2016-1-18-9-3a50-3a48.png)

1. Sélectionnez le champ de lien auquel vous souhaitez vous connecter, dans ce cas, l’identifiant.

   ![](assets/image2016-1-18-9-3a53-3a54.png)

   >[!NOTE]
   >
   >Seuls les types de champ de chaîne sont pris en charge dans le champ de lien.

1. Cliquez sur **Enregistrer.**

   ![](assets/image2016-1-18-9-3a55-3a18.png)

1. Répétez cette procédure pour le deuxième lien vers votre objet personnalisé, dans cet exemple, courseID. Le nom de l’objet de lien sera course et le champ de lien sera courseID. Puisque vous avez déjà créé et approuvé l’objet personnalisé du cours, ces sélections sont disponibles dans les menus déroulants.

   ![](assets/image2016-1-18-9-3a57-3a46.png)

1. Créez d’autres champs à utiliser dans votre objet intermédiaire, tels que enrollmentID ou grade.

## Utilisation d&#39;objets personnalisés {#using-custom-objects}

L’étape suivante consiste à utiliser ces objets personnalisés dans les filtres de vos campagnes actives. Avec une relation de type &quot;plusieurs à plusieurs&quot;, vous pouvez sélectionner plusieurs personnes/sociétés et plusieurs objets personnalisés. Dans l’exemple ci-dessous, toute personne de votre base de données qui correspond à ces critères est répertoriée. Le champ coursename provient de l’objet personnalisé course et le grade d’inscription provient de l’objet intermédiaire.

![](assets/image2016-1-14-15-3a57-3a59.png)

>[!MORELIKETHIS]
>
>* [Ajouter les champs d&#39;objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Modifier et supprimer un objet personnalisé marketing](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Compréhension des objets personnalisés de marketing](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Modifier et supprimer des champs d&#39;objet personnalisé du marketing](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)

