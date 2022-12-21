---
unique-page-id: 1900554
description: Modification d’un HTML de courrier électronique - Documents Marketo - Documentation du produit
title: Modifier le HTML d’un email
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 1%

---

# Modifier le HTML d’un email {#edit-an-emails-html}

Il peut arriver que vous deviez modifier le HTML sous-jacent d&#39;un email. Parfois, vous pouvez utiliser un système externe pour concevoir et créer le code de votre email. Dans les deux cas, vous pouvez facilement importer et/ou modifier du code dans l’éditeur de courrier électronique.

## Modifier l’HTML {#edit-html}

1. Sélectionnez votre adresse électronique et cliquez sur **Modifier le brouillon**.

   ![](assets/teamspidey.jpg)

1. Cliquez sur **Modifier le code**.

   ![](assets/two-4.png)

1. Effectuez les modifications. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Change ce que tu veux. Vous pouvez remplacer l’ensemble du HTML ou effectuer des ajustements mineurs.

1. Cliquez sur le bouton **Actions de code** pour télécharger le code sous la forme d’un fichier .html, intégrer votre CSS ou valider le HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La bonne pratique pour les emails consiste à intégrer tous vos styles. Plusieurs clients de messagerie ne prennent pas en charge CSS dans la variable `<head>` .

## Rompre un email à partir de son modèle {#breaking-an-email-from-its-template}

Ces modifications de code **ne sera pas** rompez un email à partir de son modèle :

* Modification du contenu d’un module (y compris l’ajout de nouveaux éléments dans le module)
* Ajout d’un nouveau module au conteneur
* Suppression d’un module du conteneur

* Modification des attributs spécifiques à mkto (par exemple, &quot;mktoName&quot; ou &quot;mktoImgUrl&quot;) de tout élément en dehors d’un module
* Modification du contenu d’un élément (texte enrichi, image, vidéo, etc.) en dehors d’un module

Ce que vous pouvez faire dans l’éditeur de code **will** rompez l&#39;email à partir de son modèle :

* Modification de tout élément du code en dehors d’un élément ou d’un module
* Ajout ou modification d’attributs non mkto (par exemple, &quot;id&quot; ou &quot;style&quot;) de tout élément en dehors d’un module
* Suppression d’un élément situé en dehors d’un module

## Rechercher le code {#search-code}

Utilisez la fonctionnalité de code de recherche pour rechercher et remplacer efficacement du contenu dans le code de HTML de votre email.

1. Dans le code de votre email, cliquez sur **Code de recherche**.

   ![](assets/five-2.png)

1. Saisissez ce que vous souhaitez rechercher, puis cliquez sur **Rechercher suivant** pour effectuer une recherche vers l’avant ou **Rechercher précédent** pour effectuer une recherche vers l’arrière. Vous avez également la possibilité de **Remplacer** et **Tout remplacer**.

   ![](assets/six-1.png)

1. Cliquez sur **Fermer** une fois terminé.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Le code de recherche est également disponible dans la variable [Éditeur de modèle de courrier électronique](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

Nous vous recommandons de continuer à modifier vos emails à l’aide de la fonctionnalité intégrée de Marketo, mais cet éditeur de code offre une certaine flexibilité si vous en avez besoin.
