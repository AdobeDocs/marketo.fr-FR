---
unique-page-id: 1900554
description: Modification d’une documentation HTML de messagerie - Documents Marketo - Documentation du produit
title: Modifier la version HTML d’un e-mail
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 4%

---

# Modifier la version HTML d’un e-mail {#edit-an-emails-html}

Vous devrez parfois modifier l’HTML sous-jacente d’un e-mail. Parfois, vous pouvez utiliser un système externe pour concevoir et créer le code de votre e-mail. Dans les deux cas, vous pouvez facilement importer et modifier du code à partir de l’éditeur d’e-mail.

## Modifier l’HTML {#edit-html}

1. Sélectionnez votre e-mail et cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/teamspidey.jpg)

1. Cliquez sur **[!UICONTROL Modifier le code]**.

   ![](assets/two-4.png)

1. Apportez les modifications désirées. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Changez ce que vous voulez. Vous pouvez remplacer l’intégralité d’HTML ou effectuer des ajustements mineurs.

1. Cliquez sur le menu déroulant **[!UICONTROL Actions de code]** pour télécharger le code sous la forme d’un fichier .html, incorporer votre CSS ou valider l’HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La bonne pratique pour les e-mails consiste à rendre tous vos styles intégrés. Plusieurs clients de messagerie ne prennent pas en charge CSS dans la section `<head>`.

## Rupture d’un e-mail de son modèle {#breaking-an-email-from-its-template}

Ces modifications de code **n’** pas isolent un e-mail de son modèle :

* Modification du contenu de tout module (y compris l’ajout de nouveaux éléments dans le module)
* Ajout d’un nouveau module au conteneur
* Suppression d’un module du conteneur

* Modification des attributs spécifiques à mkto (par exemple, « mktoName » ou « mktoImgUrl ») de tout élément en dehors d’un module
* Modification du contenu d’un élément (texte enrichi, image, vidéo, etc.) en dehors d’un module

L’éditeur de code vous permet d’effectuer les opérations suivantes **** à séparer l’e-mail de son modèle :

* Modification de tout élément du code en dehors d’un élément ou d’un module
* Ajouter ou modifier des attributs non-mkto (par exemple, « id » ou « style ») de tout élément en dehors d&#39;un module
* Suppression d’un élément situé en dehors d’un module

## Rechercher le code {#search-code}

Utilisez la fonctionnalité Code de recherche pour rechercher et remplacer efficacement du contenu dans le code HTML de votre e-mail.

1. Dans le code de votre e-mail, cliquez sur **[!UICONTROL Rechercher le code]**.

   ![](assets/five-2.png)

1. Saisissez ce que vous souhaitez rechercher et cliquez sur **[!UICONTROL Rechercher suivant]** pour effectuer une recherche vers l’avant ou sur **[!UICONTROL Rechercher précédent]** pour effectuer une recherche vers l’arrière. Vous avez également la possibilité de **[!UICONTROL Remplacer]** et **[!UICONTROL Tout remplacer]**.

   ![](assets/six-1.png)

1. Cliquez sur **[!UICONTROL Fermer]** lorsque vous avez terminé.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Le code de recherche est également disponible dans l’[éditeur de modèles d’e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

Nous vous recommandons de continuer à modifier vos e-mails à l’aide de la fonctionnalité intégrée de Marketo, mais cet éditeur de code offre une certaine flexibilité si vous en avez besoin.
