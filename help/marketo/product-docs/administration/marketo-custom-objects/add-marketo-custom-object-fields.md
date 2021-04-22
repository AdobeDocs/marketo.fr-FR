---
unique-page-id: 10093688
description: Ajouter les champs d’objet personnalisés Marketo - Marketo Docs - Documentation du produit
title: Ajouter les champs d’objet personnalisés Marketo
translation-type: tm+mt
source-git-commit: 65182770291dc14fbe915a40403fc09b433aae86
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# Ajouter les champs d&#39;objet personnalisé Marketo {#add-marketo-custom-object-fields}

Après avoir créé un objet personnalisé, vous devez y ajouter des champs pour répondre aux besoins de votre entreprise.

Les champs définissent les informations spécifiques utilisées par un objet personnalisé. Les champs de lien ont un travail spécial, pour connecter des objets personnalisés, et sont couverts dans un [article distinct](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Cliquez sur **Admin** et dans **Gestion de la base de données**, sélectionnez **Marketo Custom Objects**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Sélectionnez l’objet auquel vous souhaitez ajouter le champ sur la droite.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Dans l&#39;onglet **Champs**, cliquez sur **Nouveau champ**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >Les trois champs illustrés ci-dessus sont automatiquement créés par Marketo lorsque vous créez un objet personnalisé. Marketo gère ces champs automatiquement et vous ne pouvez ni les modifier ni les supprimer.

1. Saisissez un nom d’affichage et une description.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >Le nom de l&#39;API ne peut être modifié que jusqu&#39;à ce qu&#39;il soit approuvé.

1. Sélectionnez maintenant un type de données approprié dans la liste.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Faites glisser le curseur Dédupliquer si vous souhaitez utiliser le nouveau champ comme identificateur unique. Cliquez sur **Enregistrer** pour terminer.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >Les champs de déduplication peuvent être utilisés pour récupérer, mettre à jour ou supprimer des objets personnalisés. Chaque définition d’objet personnalisé doit contenir au moins un (et pas plus de trois) champs dédupliqués.

1. Ajoutez les autres champs dont vous avez besoin.

   >[!NOTE]
   >
   >Si vous créez une structure de type &quot;un à plusieurs&quot;, vous devez ajouter un champ Lien à votre objet personnalisé. Pour une structure de type &quot;plusieurs à plusieurs&quot;, vous n’avez pas besoin d’un champ de lien dans l’objet personnalisé, mais vous devez ajouter deux champs de lien dans l’objet intermédiaire. Voir [Ajouter Marketo Custom Object Link Fields](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) pour créer les champs de lien et [Comprendre les objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) pour plus d&#39;informations sur les types d&#39;objets personnalisés.

>[!MORELIKETHIS]
>
>* [Ajouter les champs de lien d’objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Modification et suppression d’un objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Modifier et supprimer des champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

