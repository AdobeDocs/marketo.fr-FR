---
unique-page-id: 1900554
description: Modification d’un courrier électronique HTML - Documents marketing - Documentation du produit
title: Modification du code HTML d’un courrier électronique
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Modification du code HTML d’un courrier électronique {#edit-an-emails-html}

Il peut être nécessaire de modifier le code HTML sous-jacent d’un courrier électronique. Vous pouvez parfois utiliser un système externe pour concevoir et créer le code de votre messagerie. Dans les deux cas, vous pouvez facilement importer et/ou modifier du code dans l’éditeur de courrier électronique.

## Modifier HTML {#edit-html}

1. Sélectionnez votre adresse électronique et cliquez sur **Modifier le brouillon**.

   ![](assets/teamspidey.jpg)

1. Cliquez sur **Modifier le code**.

   ![](assets/two-4.png)

1. Effectuez toutes les modifications. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Change ce que tu veux. Vous pouvez remplacer l’intégralité du code HTML ou effectuer des ajustements mineurs.

1. Cliquez sur la liste déroulante Actions **** de code pour télécharger le code sous la forme d’un fichier .html, d’une page CSS intégrée ou de la validation du code HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La meilleure pratique pour les courriels est de mettre tous vos styles en ligne. Plusieurs clients de messagerie ne prennent pas en charge les pages CSS dans la `<head>` section.

## Rompre un courrier électronique à partir de son modèle {#breaking-an-email-from-its-template}

Ces modifications de code **ne rompent pas** un courrier électronique de son modèle :

* Modification du contenu d’un module (y compris l’ajout de nouveaux éléments dans le module)
* Ajouter un nouveau module au Conteneur
* Suppression d&#39;un module du Conteneur

* Modification des attributs spécifiques à mkto (par exemple, &quot;mktoName&quot; ou &quot;mktoImgUrl&quot;) de tout élément en dehors d’un module
* Modification du contenu d’un élément (texte enrichi, image, vidéo, etc.) en dehors d’un module

Les actions que vous pouvez effectuer dans l’éditeur de code **vont** rompre le courrier électronique à partir de son modèle :

* Modification de tout élément du code en dehors d’un élément ou d’un module
* Ajouter ou modifier des attributs non mkto (par exemple, &quot;id&quot; ou &quot;style&quot;) de tout élément en dehors d’un module
* Suppression d’un élément en dehors d’un module

## Code de recherche {#search-code}

Utilisez la fonctionnalité Code de recherche pour rechercher et remplacer efficacement du contenu dans le code HTML de votre courrier électronique.

1. Dans le code de votre courrier électronique, cliquez sur Code **de** recherche.

   ![](assets/five-2.png)

1. Saisissez ce que vous souhaitez rechercher, puis cliquez sur **Rechercher suivant** pour effectuer une recherche vers l’avant ou **Rechercher précédent** pour effectuer une recherche vers l’arrière. Vous avez également la possibilité de **Remplacer** et **Remplacer tout**.

   ![](assets/six-1.png)

1. Cliquez sur **Fermer** lorsque vous avez terminé.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Le code de recherche est également disponible dans l’éditeur [Modèle de](http://docs.marketo.com/display/DOCS/Create+a+New+Email+Template)courriel.

Nous vous recommandons de continuer à modifier vos courriels à l’aide de la fonctionnalité intégrée de Marketo, mais cet éditeur de code offre une certaine souplesse si vous en avez besoin.
