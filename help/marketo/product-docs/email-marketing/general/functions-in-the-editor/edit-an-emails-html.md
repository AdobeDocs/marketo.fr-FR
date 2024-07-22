---
unique-page-id: 1900554
description: Modification de l’HTML d’un courrier électronique - Documents Marketo - Documentation du produit
title: Modifier l’HTML d’un email
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# Modifier l’HTML d’un email {#edit-an-emails-html}

Il peut arriver que vous deviez modifier l’HTML sous-jacent d’un email. Parfois, vous pouvez utiliser un système externe pour concevoir et créer le code de votre email. Dans les deux cas, vous pouvez facilement importer et/ou modifier du code dans l’éditeur de courrier électronique.

## Modifier l’HTML {#edit-html}

1. Sélectionnez votre adresse électronique et cliquez sur **Modifier le brouillon**.

   ![](assets/teamspidey.jpg)

1. Cliquez sur **Modifier le code**.

   ![](assets/two-4.png)

1. Apportez les modifications nécessaires. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Change ce que tu veux. Vous pouvez remplacer l’HTML entier ou effectuer des ajustements mineurs.

1. Cliquez sur la liste déroulante **Actions du code** pour télécharger le code sous la forme d’un fichier .html, intégrer votre CSS ou valider l’HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La bonne pratique pour les emails consiste à intégrer tous vos styles. Plusieurs clients de messagerie ne prennent pas en charge CSS dans la section `<head>`.

## Rompre un email à partir de son modèle {#breaking-an-email-from-its-template}

Ces modifications de code **ne rompent pas** un email de son modèle :

* Modification du contenu d’un module (y compris l’ajout de nouveaux éléments dans le module)
* Ajout d’un nouveau module au conteneur
* Suppression d’un module du conteneur

* Modification des attributs spécifiques à mkto (par exemple, &quot;mktoName&quot; ou &quot;mktoImgUrl&quot;) de tout élément en dehors d’un module
* Modification du contenu d’un élément (texte enrichi, image, vidéo, etc.) en dehors d’un module

Ces actions que vous pouvez effectuer dans l’éditeur de code **vont** interrompre l’email à partir de son modèle :

* Modification de tout élément du code en dehors d’un élément ou d’un module
* Ajout ou modification d’attributs non mkto (par exemple, &quot;id&quot; ou &quot;style&quot;) de tout élément en dehors d’un module
* Suppression d’un élément situé en dehors d’un module

## Rechercher le code {#search-code}

Utilisez la fonctionnalité de code de recherche pour rechercher et remplacer efficacement du contenu dans le code d’HTML de votre email.

1. Dans le code de votre email, cliquez sur **Search Code**.

   ![](assets/five-2.png)

1. Saisissez ce que vous souhaitez rechercher et cliquez sur **Rechercher le suivant** pour effectuer une recherche vers l’avant ou sur **Rechercher le précédent** pour effectuer une recherche vers l’arrière. Vous avez également la possibilité de **Remplacer** et **Remplacer tout**.

   ![](assets/six-1.png)

1. Cliquez sur **Fermer** une fois terminé.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Le code de recherche est également disponible dans l’[ éditeur de modèles d’email](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

Nous vous recommandons de continuer à modifier vos emails à l’aide de la fonctionnalité intégrée de Marketo, mais cet éditeur de code offre une certaine flexibilité si vous en avez besoin.
