---
unique-page-id: 10094188
description: Approbation d’un objet personnalisé - Documents Marketo - Documentation du produit
title: Approbation d’un objet personnalisé
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Approbation d’un objet personnalisé {#approve-a-custom-object}

Vous devez approuver un objet personnalisé avant de pouvoir l’utiliser. Le processus est légèrement différent pour les nouveaux objets personnalisés et ceux que vous avez modifiés.

## Approbation d’un nouvel objet personnalisé {#approve-a-new-custom-object}

Vous avez créé un nouvel objet personnalisé. Voici comment l&#39;approuver.

1. Dans Admin, cliquez sur **Objets personnalisés Marketo** et sélectionnez un objet dont l’état est En création.

   ![](assets/one.png)

1. Cliquez sur le bouton **Actions d’objet personnalisées** et sélectionnez **Approuver l’objet**.

   ![](assets/two.png)

1. L’état devient Approuvé.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Un objet personnalisé utilisé dans une _structure un-à-multiple_ doit comporter au moins un champ de déduplication, un champ de lien, un nom d’objet lié et un nom de champ lié à valider.
   >
   >Un objet personnalisé utilisé dans une _structure multiple-à-multiple_ **ne** vous avez besoin d’un champ de lien, d’un nom d’objet lié ou d’un nom de champ lié lorsque vous le validez (car ils se trouvent dans l’objet intermédiaire).
   >
   >Objet personnalisé utilisé comme _objet intermédiaire_ nécessite un champ de lien, un nom d’objet lié et un nom de champ lié, mais **ne** nécessitent un champ de déduplication.
   >
   >Voir [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) pour plus d’informations.

C&#39;est tout ! Désormais, vous pouvez sélectionner votre objet personnalisé dans les contraintes de vos filtres et déclencheurs à utiliser dans vos campagnes.

## Approbation d’un objet personnalisé modifié {#approve-an-edited-custom-object}

Après avoir modifié un objet personnalisé approuvé, vous devez approuver le brouillon pour renvoyer l’objet personnalisé à un état Approuvé.

1. Lorsque vous modifiez un objet personnalisé déjà approuvé, il reçoit l’état Approuvé avec brouillon .

   ![](assets/four.png)

1. Lorsque vous êtes prêt à approuver le brouillon, cliquez sur le **Actions d’objet personnalisées** et sélectionnez **Approuver l’objet**.

   ![](assets/five-1.png)

1. Un aperçu affiche les éléments qui ont été modifiés dans le brouillon. Cliquez sur **Approuver**.

   ![](assets/six-1.png)
