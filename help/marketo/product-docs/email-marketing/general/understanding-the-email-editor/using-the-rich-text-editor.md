---
unique-page-id: 2953419
description: Utilisation de l’éditeur de texte enrichi - Documents Marketo - Documentation du produit
title: Utilisation de l’éditeur de texte enrichi
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 5%

---

# Utilisation de l’éditeur de texte enrichi {#using-the-rich-text-editor}

L’éditeur de texte enrichi (RTE) s’affiche dans tout Marketo et est disponible lorsque vous souhaitez ajouter ou modifier du contenu. Une version apparaît sur les landing pages, les programmes, les emails, les formulaires et les fragments de code. Cliquez simplement sur **Modifier le brouillon** et il s’affiche pour vous servir.

## Paramètres de l’éditeur {#editor-settings}

Le paramètre d’élément de bloc racine définit les balises qui encapsulent votre contenu. Par défaut, l’élément de bloc racine d’email utilise des balises `<p>`. Vous avez la possibilité de modifier ce paramètre en suivant les étapes ci-dessous.

>[!TIP]
>
>Bien que vous ayez la possibilité de choisir votre élément de bloc racine, nous vous recommandons toujours d’utiliser les paramètres par défaut pour optimiser l’expérience utilisateur.

1. Cliquez sur **Admin**.

   ![](assets/one.png)

1. Cliquez sur **Email**.

   ![](assets/two.png)

1. Cliquez sur **Modifier les paramètres de l’éditeur de texte**.

   ![](assets/three.png)

1. Dans la liste déroulante **Email / Snippet Editor**, sélectionnez `<div>` ou None et cliquez sur **Enregistrer**. `<div>` est utilisé dans cet exemple.

   ![](assets/four.png)

   Si vous avez `<div class=“mktEditable”></div>` dans un modèle de courrier électronique, le comportement Source de l’HTML suivant s’affiche lorsque vous ouvrez la section et saisissez &quot;Texte ici&quot; dans l’éditeur :

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Aucun</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;p&gt;Texte ici&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;div&gt;Texte ici&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>Texte disponible ici<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Vous pouvez également modifier l’élément de bloc racine de l’éditeur de page d’entrée en suivant les mêmes étapes, mais en cliquant sur la liste déroulante **Éditeur de page d’entrée** de l’étape 4 au lieu de l’éditeur de courrier électronique/extrait de code.

>[!NOTE]
>
>L’élément de bloc racine est toujours `<p>` pour les jetons de programme de texte enrichi.

## Caractéristiques {#features}

Voici les fonctionnalités que vous trouverez dans un éditeur de texte enrichi.

| Icône | Nom | Fonctionnement |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | Famille de police | Choisissez votre style, nous en avons plein ! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | Taille de la police | Quelle taille en voulez-vous ? 25 choix, de 8 px à 90 px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | Styles | Choisissez Paragraphe ou six styles d&#39;en-tête (pour les landing pages). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | Espacement des lignes | Choisissez la distance entre les lignes. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | Couleur du texte | Noir, rouge ou quoi que ce soit que vous vouliez. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | Couleur de l’arrière-plan | Surlignez pour mettre l’accent. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | Gras | **Plus sombre et plus épais**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | Italique | *Angled, pour la mise en évidence ou les guillemets*. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | Souligner | Place une ligne sous votre texte. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | Alignement | Utilisez cette liste déroulante pour mettre en page votre texte et vos images. Centrez-les, choisissez l&#39;alignement gauche ou droit, ou étalez-le de haut en haut avec une justification complète. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Liste | Sélectionnez des puces ou des nombres dans la liste déroulante. Les puces sont adaptées aux listes et aux nombres avec des étapes. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | Commencer en retrait | Choisissez plus ou moins une mise en retrait. Utilisez pour les paragraphes ou tout texte que vous souhaitez mettre en évidence. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | Insérer/Modifier le lien | Insérer un lien vers un site web ou tout autre contenu ; y apporter facilement des modifications. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | Insérer/Modifier l’image | Une image vaut mille mots. Laisse-en un. Cliquez sur l’icône de la caméra pour parcourir Design Studio. Vous pouvez déposer les images côte à côte. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | Insérer le jeton | Un outil puissant, idéal pour la personnalisation des emails et le suivi des données. Veillez à saisir une valeur par défaut. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | Annuler | Oups ! Retournons un pas en arrière et réessayez. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | Rétablir | Si c&#39;est vraiment normal, revenez à l&#39;original. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | Tableau | Construisez la vôtre, comme celle-ci. Un menu déroulant vous permet de le paramétrer. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | Insérer une ancre | Déposez l&#39;ancre ! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | Ligne horizontale | Plusieurs utilisations : idéal pour la division des sections. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | Modifier l’HTML | Permet d’afficher l’éditeur Source d’HTML afin que vous puissiez ajuster votre code. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | Indice | Lettres pendantes faibles (comme dans O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | Exposant | Vous avez le pouvoir ! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | Barré | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | Caractère spécial | Vous voulez parler d&#39;euros ? Les maths ? Vous avez 243 choix. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | Rechercher et remplacer | Recherchez et modifiez les éléments beaucoup plus rapidement que chaque instance vous-même. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | Effacer la mise en forme | Revenez aux éléments standard. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | Annuler | Appuyez sur le bouton pour dire : &quot;Peu importe.&quot; |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | Sauvegarder | Appuyez sur le bouton pour dire : &quot;OK, j&#39;aime ça.&quot; |

>[!TIP]
>
>Vous modifiez l’HTML et le texte sur des écrans distincts. Veillez à cliquer sur **Copier depuis l’HTML** dans l’onglet **Texte** , puis sur **Enregistrer** afin que votre texte corresponde à votre HTML.

>[!NOTE]
>
>Vous n’êtes pas limité aux polices dans la liste déroulante. Vous pouvez en utiliser une qui n’est pas répertoriée en accédant au code de l’HTML. Toutes les polices web sont prises en charge dans Marketo, mais les polices web ne fonctionnent pas de manière universelle dans tous les clients de messagerie.

## Pages de destination {#landing-pages}

Le paramètre d’élément de bloc racine définit les balises qui encapsulent votre contenu. Par défaut, l’élément de bloc racine de page d’entrée utilise des balises `<div>`. Vous avez la possibilité de modifier ce paramètre en suivant les étapes ci-dessous.

>[!TIP]
>
>Bien que vous ayez la possibilité de choisir votre élément de bloc racine, nous vous recommandons toujours d’utiliser les paramètres par défaut pour optimiser l’expérience utilisateur.

1. Cliquez sur **Admin**.

   ![](assets/one.png)

1. Cliquez sur **Email**.

   ![](assets/two.png)

1. Cliquez sur **Modifier les paramètres de l’éditeur de texte**.

   ![](assets/three.png)

1. Dans la liste déroulante **Éditeur de page d’entrée**, sélectionnez `<p>` ou Aucun et cliquez sur **Enregistrer**. `<p>` est utilisé dans cet exemple.

   ![](assets/five.png)

   Et c&#39;est tout !
