---
unique-page-id: 10094188
description: Approuver un objet personnalisé - Documents marketing - Documentation du produit
title: Approuver un objet personnalisé
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Approuver un objet personnalisé {#approve-a-custom-object}

Vous devez approuver un objet personnalisé avant de pouvoir l’utiliser. Le processus est légèrement différent pour les nouveaux objets personnalisés et ceux que vous avez modifiés.

## Approuver un nouvel objet personnalisé {#approve-a-new-custom-object}

Vous avez créé un nouvel objet personnalisé. Voici comment l&#39;approuver.

1. Dans Admin, cliquez sur **Marketo Custom Objects** et sélectionnez un objet à l’état Brouillon.

   ![](assets/one.png)

1. Cliquez sur la liste déroulante **Actions d’objet personnalisé** et sélectionnez **Approuver l’objet**.

   ![](assets/two.png)

1. L&#39;état devient Approuvé.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Un objet personnalisé utilisé dans une structure _de type &quot;un à plusieurs&quot;_ doit comporter au moins un champ de déduplication, un champ de lien, un nom d’objet lié et un nom de champ lié à approuver.
   >
   >Un objet personnalisé utilisé dans une structure _plusieurs à plusieurs_ **n&#39;a pas besoin** d&#39;un champ de lien, d&#39;un nom d&#39;objet lié ou d&#39;un nom de champ lié lorsque vous l&#39;approuvez (car il réside dans l&#39;objet intermédiaire).
   >
   >Un objet personnalisé utilisé en tant qu&#39;objet _intermédiaire_ nécessite un champ de lien, un nom d&#39;objet lié et un nom de champ lié, mais **ne nécessite pas** un champ de déduplication.
   >
   >Voir [Présentation des objets personnalisés du marketing](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) pour plus d’informations.

C&#39;est tout ! Désormais, vous pouvez sélectionner votre objet personnalisé dans les contraintes de vos filtres et déclencheurs à utiliser dans vos campagnes.

## Approuver un objet personnalisé modifié {#approve-an-edited-custom-object}

Après avoir modifié un objet personnalisé approuvé, vous devez approuver le brouillon pour que l’objet personnalisé soit renvoyé à un état Approuvé.

1. Lorsque vous modifiez un objet personnalisé déjà approuvé, il reçoit un état Approuvé avec brouillon.

   ![](assets/four.png)

1. Lorsque vous êtes prêt à approuver le brouillon, cliquez sur la liste déroulante **Actions d’objet personnalisé** et sélectionnez **Approuver l’objet**.

   ![](assets/five-1.png)

1. Une prévisualisation affiche les éléments qui ont été modifiés dans le brouillon. Cliquez sur **Approuver**.

   ![](assets/six-1.png)
