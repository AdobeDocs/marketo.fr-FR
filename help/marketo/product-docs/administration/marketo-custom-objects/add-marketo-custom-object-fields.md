---
unique-page-id: 10093688
description: Ajouter des champs d’objet personnalisés Marketo - Documents Marketo - Documentation du produit
title: Ajouter des champs d’objet personnalisés Marketo
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Ajouter des champs d’objet personnalisés Marketo {#add-marketo-custom-object-fields}

Après avoir créé un objet personnalisé, vous devez y ajouter des champs pour répondre aux besoins de votre entreprise.

Les champs définissent les informations spécifiques utilisées par un objet personnalisé. Les champs de lien comportent une tâche spéciale permettant de connecter des objets personnalisés et sont traités dans un [article distinct](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Cliquez sur **[!UICONTROL Objets personnalisés Marketo]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Sélectionnez l’objet auquel vous souhaitez ajouter le champ à droite.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. Cliquez sur l&#39;onglet **[!UICONTROL Champs]**, puis **[!UICONTROL Nouveau champ]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >Les trois champs présentés ci-dessus sont créés automatiquement par Marketo lors de la création d’un objet personnalisé. Marketo gère automatiquement ces champs. Vous ne pouvez pas les modifier ni les supprimer.

1. Saisissez un [!UICONTROL Nom d’affichage] et (facultatif) un [!UICONTROL Description].

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >Le [!UICONTROL nom de l’API] ne peut être modifié que jusqu’à ce qu’il soit approuvé.

1. Sélectionnez à présent un [!UICONTROL type de données] approprié dans la liste.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Déplacez le curseur [!UICONTROL Déduplication] si vous souhaitez utiliser le nouveau champ comme identifiant unique. Cliquez sur **[!UICONTROL Enregistrer]** pour terminer.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >Les champs Dédupliquer peuvent être utilisés pour récupérer, mettre à jour ou supprimer des objets personnalisés. Chaque définition d’objet personnalisé doit contenir au moins un champ de déduplication (et pas plus de trois).

1. Ajoutez les autres champs dont vous avez besoin.

   >[!NOTE]
   >
   >Si vous créez une structure de type « un à plusieurs », vous devez ajouter un champ Lien à votre objet personnalisé. Pour une structure multiple-à-multiple, vous n’avez pas besoin d’un champ de lien dans l’objet personnalisé, mais vous devez ajouter deux champs de lien dans l’objet intermédiaire. Voir [Ajouter des champs de lien d’objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) pour créer les champs de lien, et [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) pour plus d’informations sur les types d’objets personnalisés.

>[!MORELIKETHIS]
>
>* [Ajouter des champs de lien d’objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Modifier et supprimer un objet personnalisé Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Modifier et supprimer des champs d’objet personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
