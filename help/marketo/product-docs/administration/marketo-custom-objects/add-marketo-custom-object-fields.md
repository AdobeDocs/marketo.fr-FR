---
unique-page-id: 10093688
description: Ajout de champs d’objet personnalisés Marketo - Documents Marketo - Documentation du produit
title: Ajout de champs d’objet personnalisés Marketo
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Ajout de champs d’objet personnalisés Marketo {#add-marketo-custom-object-fields}

Après avoir créé un objet personnalisé, vous devez y ajouter des champs pour répondre aux besoins de votre entreprise.

Les champs définissent les informations spécifiques utilisées par un objet personnalisé. Les champs de lien ont une tâche spéciale, permettant de connecter des objets personnalisés, et sont couverts par une [article distinct](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Cliquez sur **Administration** et dans **Gestion de base de données**, sélectionnez **Objets personnalisés Marketo**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Sélectionnez l’objet auquel vous souhaitez ajouter le champ à droite.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Dans le **Champs** , cliquez sur **Nouveau champ**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >Les trois champs affichés ci-dessus sont créés automatiquement par Marketo lorsque vous créez un objet personnalisé. Marketo gère ces champs automatiquement et vous ne pouvez pas les modifier ni les supprimer.

1. Saisissez un nom d’affichage et une description.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >Le nom de l’API ne peut être modifié que lorsqu’il a été approuvé.

1. Sélectionnez maintenant un type de données approprié dans la liste.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Survolez le curseur Déduplication si vous souhaitez utiliser le nouveau champ comme identifiant unique. Cliquez sur **Enregistrer** à la fin.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >Les champs de déduplication peuvent être utilisés pour récupérer, mettre à jour ou supprimer des objets personnalisés. Chaque définition d’objet personnalisé doit contenir au moins un (et pas plus de trois) champ de déduplication.

1. Ajoutez les autres champs dont vous avez besoin.

   >[!NOTE]
   >
   >Si vous créez une structure de type &quot;un à plusieurs&quot;, vous devez ajouter un champ Lien à votre objet personnalisé. Pour une structure de type &quot;plusieurs à plusieurs&quot;, vous n’avez pas besoin d’un champ de lien dans l’objet personnalisé, mais vous devez ajouter deux champs de lien dans l’objet intermédiaire. Voir [Ajout de champs de lien d’objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) pour créer les champs de lien, et [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) pour plus d’informations sur les types d’objets personnalisés.

>[!MORELIKETHIS]
>
>* [Ajout de champs de lien d’objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Modification et suppression d’un objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Modification et suppression de champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

