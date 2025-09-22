---
unique-page-id: 10094188
description: Approbation d’un objet personnalisé - Documents Marketo - Documentation du produit
title: Approuver un objet personnalisé
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 3%

---

# Approuver un objet personnalisé {#approve-a-custom-object}

Vous devez approuver un objet personnalisé avant de pouvoir l’utiliser. Le processus est légèrement différent pour les nouveaux objets personnalisés et ceux que vous avez modifiés.

## Approuver un nouvel objet personnalisé {#approve-a-new-custom-object}

Vous avez créé un tout nouvel objet personnalisé. Voici comment l&#39;approuver.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/approve-a-custom-object-1.png)

1. Cliquez sur **[!UICONTROL Objets personnalisés Marketo]**.

   ![](assets/approve-a-custom-object-2.png)

1. Sélectionnez un objet dont l’état est Brouillon.

   ![](assets/approve-a-custom-object-3.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Actions sur l’objet personnalisé]** et sélectionnez **[!UICONTROL Approuver l’objet]**.

   ![](assets/approve-a-custom-object-4.png)

1. L’état devient [!UICONTROL Approuvé].

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Un objet personnalisé utilisé dans une structure _un à plusieurs_ doit avoir au moins un champ de déduplication, un champ de lien, un nom d’objet lié et un nom de champ lié à approuver.
   >
   >Un objet personnalisé utilisé dans une structure _plusieurs-à-plusieurs_ **n’a pas besoin** d’un champ de lien, d’un nom d’objet lié ou d’un nom de champ lié lorsque vous l’approuvez (car ils se trouvent dans l’objet intermédiaire).
   >
   >Un objet personnalisé utilisé comme _objet intermédiaire_ nécessite un champ de lien, un nom d’objet lié et un nom de champ lié, mais **ne nécessite pas** un champ de déduplication.
   >
   >Voir [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) pour plus d’informations.

Vous avez terminé. Vous pouvez désormais sélectionner votre objet personnalisé dans les contraintes de vos filtres et triggers à utiliser dans vos campagnes.

## Approbation d’un objet personnalisé modifié {#approve-an-edited-custom-object}

Après avoir modifié un objet personnalisé approuvé, vous devez approuver le brouillon pour rétablir l’objet personnalisé à l’état Approuvé .

1. Lorsque vous modifiez un objet personnalisé déjà approuvé, il reçoit le statut [!UICONTROL Approuvé avec brouillon].

   ![](assets/approve-a-custom-object-6.png)

1. Lorsque vous êtes prêt à approuver le brouillon, cliquez sur le menu déroulant **[!UICONTROL Actions sur l’objet personnalisé]** et sélectionnez **[!UICONTROL Approuver l’objet]**.

   ![](assets/approve-a-custom-object-7.png)

1. Un aperçu affiche les éléments qui ont été modifiés dans le brouillon. Cliquez sur **[!UICONTROL Approuver]**.

   ![](assets/approve-a-custom-object-8.png)
