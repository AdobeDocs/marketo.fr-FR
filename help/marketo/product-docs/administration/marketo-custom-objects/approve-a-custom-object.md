---
unique-page-id: 10094188
description: Approuver un objet personnalisé - Documents Marketo - Documentation du produit
title: Approbation d’un objet personnalisé
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Approbation d’un objet personnalisé {#approve-a-custom-object}

Vous devez approuver un objet personnalisé avant de pouvoir l’utiliser. Le processus est légèrement différent pour les nouveaux objets personnalisés et ceux que vous avez modifiés.

## Approbation d’un nouvel objet personnalisé {#approve-a-new-custom-object}

Vous avez créé un nouvel objet personnalisé. Voici comment l&#39;approuver.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/approve-a-custom-object-1.png)

1. Cliquez sur **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/approve-a-custom-object-2.png)

1. Sélectionnez un objet dont l’état est En création.

   ![](assets/approve-a-custom-object-3.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Actions d’objet personnalisé]** et sélectionnez **[!UICONTROL Approuver l’objet]**.

   ![](assets/approve-a-custom-object-4.png)

1. L’état devient [!UICONTROL Approuvé].

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Un objet personnalisé utilisé dans une _structure un-à-multiple_ doit comporter au moins un champ de déduplication, un champ de lien, un nom d’objet lié et un nom de champ lié à approuver.
   >
   >Un objet personnalisé utilisé dans une _structure multiple-à-multiple_ **n’a pas besoin d’un champ de lien, d’un nom d’objet lié ou d’un nom de champ lié lorsque vous l’approuvez (car il se trouve dans l’objet intermédiaire).**
   >
   >Un objet personnalisé utilisé comme _objet intermédiaire_ nécessite un champ de lien, un nom d’objet lié et un nom de champ lié, mais **ne nécessite pas** de champ de déduplication.
   >
   >Pour plus d’informations, voir [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) .

C&#39;est tout ! Désormais, vous pouvez sélectionner votre objet personnalisé dans les contraintes de vos filtres et déclencheurs à utiliser dans vos campagnes.

## Approbation d’un objet personnalisé modifié {#approve-an-edited-custom-object}

Après avoir modifié un objet personnalisé approuvé, vous devez approuver le brouillon pour renvoyer l’objet personnalisé à un état Approuvé.

1. Lorsque vous modifiez un objet personnalisé déjà approuvé, il reçoit l’état [!UICONTROL Approuvé avec brouillon].

   ![](assets/approve-a-custom-object-6.png)

1. Lorsque vous êtes prêt à approuver le brouillon, cliquez sur la liste déroulante **[!UICONTROL Actions d’objet personnalisé]** et sélectionnez **[!UICONTROL Approuver l’objet]**.

   ![](assets/approve-a-custom-object-7.png)

1. Un aperçu affiche les éléments modifiés dans le brouillon. Cliquez sur **[!UICONTROL Approve]**.

   ![](assets/approve-a-custom-object-8.png)
