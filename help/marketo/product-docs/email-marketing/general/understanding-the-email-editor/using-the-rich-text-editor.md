---
unique-page-id: 2953419
description: Utilisation de l’éditeur de texte enrichi - Documents Marketo - Documentation du produit
title: Utilisation de l’éditeur de texte enrichi
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# Utilisation de l’éditeur de texte enrichi {#using-the-rich-text-editor}

L’éditeur de texte enrichi (RTE) s’affiche dans Marketo et est disponible lorsque vous souhaitez ajouter ou modifier du contenu. Une version s’affiche sur les pages de destination, les programmes, les e-mails, les formulaires et les fragments de code. Il vous suffit de cliquer sur **[!UICONTROL Modifier le brouillon]** pour qu’il s’affiche.

## Paramètres de l’éditeur {#editor-settings}

Le paramètre d’élément de bloc racine définit les balises qui encapsulent votre contenu. Par défaut, l’élément de bloc racine d’e-mail utilise des balises `<p>`. Vous avez la possibilité de modifier ce paramètre en suivant les étapes ci-dessous.

>[!TIP]
>
>Bien que vous ayez la possibilité de choisir votre élément de bloc racine, nous vous recommandons toujours d’utiliser les paramètres par défaut pour une expérience utilisateur optimale.

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Modifier les paramètres de l’éditeur de texte]**.

   ![](assets/three.png)

1. Dans la liste déroulante **[!UICONTROL E-mail] / [!UICONTROL Éditeur de fragment de code]**, sélectionnez `<div>` ou [!UICONTROL Aucun] et cliquez sur **[!UICONTROL Enregistrer]**. `<div>` est utilisé dans cet exemple.

   ![](assets/four.png)

   Si vous avez `<div class=“mktEditable”></div>` dans un modèle d’e-mail, le comportement d’HTML Source suivant s’affiche à l’ouverture de la section et vous saisissez « Texte envoyé ici » dans l’éditeur :

<table>
 <tbody>
  <tr>
   <th>&lt;p&gt;</th>
   <th>&lt;div&gt;</th>
   <th>Aucune</th>
  </tr>
  <tr>
   <td><p>&lt;div class=« mktEditable »&gt;<br>&lt;p&gt;Le texte se trouve ici&lt;/p&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class=« mktEditable »&gt;<br>&lt;div&gt;Le texte se trouve ici&lt;/div&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class=« mktEditable »&gt;<br>Le texte est ici<br>&lt;/div&gt;</p></td>
  </tr>
 </tbody>
</table>

>[!TIP]
>
>Vous pouvez également modifier l’élément de bloc racine de l’éditeur de page de destination en suivant les mêmes étapes, mais en cliquant sur le menu déroulant **[!UICONTROL Éditeur de page de destination]** à l’étape 4 au lieu de [!UICONTROL E-mail] / [!UICONTROL Éditeur de fragment de code].

>[!NOTE]
>
>L’élément de bloc racine est toujours `<p>` pour les jetons de programme de texte enrichi.

## Fonctionnalités {#features}

Voici les fonctionnalités que vous trouverez dans un éditeur de texte enrichi.

| Icône | Nom | Ce qu&#39;il fait |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | [!UICONTROL Famille de polices] | Choisissez votre style, nous en avons plein ! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | [!UICONTROL Taille de police] | Combien en voulez-vous ? 25 choix, de 8px à 90px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | [!UICONTROL  Styles ] | Choisissez les styles Paragraphe ou Six styles Titre (pour les pages de destination). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | [!UICONTROL Interligne] | Choisissez la distance entre les lignes. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | [!UICONTROL Couleur du texte] | Noir, rouge, ou ce que vous voulez. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | [!UICONTROL  Couleur d’arrière-plan ] | Mettez en surbrillance pour mettre l’accent. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | [!UICONTROL Gras] | **Plus sombre et plus épais**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | [!UICONTROL Italique] | *Angle, pour mettre en évidence ou citer* s. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | [!UICONTROL Souligné] | Insère une ligne sous votre texte. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | [!UICONTROL Alignement] | Utilisez cette liste déroulante pour mettre en page votre texte et vos images. Centrez-les, choisissez un alignement à gauche ou à droite, ou répartissez-les bord à bord avec une justification complète. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Liste | Sélectionnez des puces ou des nombres dans la liste déroulante. Les puces sont adaptées aux listes et les nombres aux étapes. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | [!UICONTROL Retrait] | Choisissez une mise en retrait plus ou moins importante. Utilisez pour les paragraphes ou tout texte que vous souhaitez mettre en évidence. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | [!UICONTROL Insérer/Modifier le lien] | Insérez un lien vers un site web ou un autre contenu ; modifiez-le facilement. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | [!UICONTROL Insérer/Modifier l’image] | Une image vaut mille mots. Déposez-en un. Cliquez sur l&#39;icône de caméra pour parcourir votre Design Studio. Vous pouvez déposer des images côte à côte. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | [!UICONTROL Insérer un jeton] | Un outil puissant, idéal pour la personnalisation des e-mails et le suivi des données. Veillez à saisir une valeur par défaut. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | [!UICONTROL  Annuler ] | Oups ! Revenons un peu en arrière et réessayons. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | [!UICONTROL Rétablir] | Si tout va bien comme ça, retournez à l&#39;original. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | [!UICONTROL Tableau] | Construisez le vôtre, comme celui-ci. Un menu déroulant vous permet de le configurer. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | [!UICONTROL Insérer une ancre] | Jetez l&#39;ancre ! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | [!UICONTROL Ligne horizontale] | Plusieurs utilisations - Idéal pour diviser les sections. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | [!UICONTROL Modifier HTML] | Affiche l’éditeur Source d’HTML afin que vous puissiez ajuster votre code. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | [!UICONTROL Indice] | Lettres courantes (comme dans O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | [!UICONTROL Exposant] | Tu as le pouvoir ! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | [!UICONTROL Barré ] | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | [!UICONTROL Caractère spécial] | Tu veux parler d&#39;euros ? Les maths ? Tu as 243 choix. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | [!UICONTROL Rechercher et remplacer] | Recherchez et modifiez des éléments beaucoup plus rapidement que de rechercher vous-même chaque instance. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | [!UICONTROL Effacer la mise en forme] | Rétablissez les normes. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | [!UICONTROL Annuler] | Appuyez sur le bouton pour dire, « Peu importe. » |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | [!UICONTROL Enregistrer ] | Appuyez sur le bouton pour dire : « OK, ça me plaît. » |

>[!TIP]
>
>Vous pouvez modifier votre HTML et votre texte sur des écrans distincts. Veillez à cliquer sur **[!UICONTROL Copier à partir d’HTML]** dans l’onglet **[!UICONTROL Texte]**, puis sur **[!UICONTROL Enregistrer]** afin que votre texte corresponde à votre HTML.

>[!NOTE]
>
>Vous n’êtes pas limité aux polices dans la liste déroulante. Vous pouvez en utiliser un qui n’est pas répertorié en accédant au code HTML. Toutes les polices web sont prises en charge dans Marketo, mais elles ne fonctionnent pas universellement dans tous les clients de messagerie.

## Pages de destination {#landing-pages}

Le paramètre d’élément de bloc racine définit les balises qui encapsulent votre contenu. Par défaut, l’élément de bloc racine de la page de destination utilise des balises `<div>`. Vous avez la possibilité de modifier ce paramètre en suivant les étapes ci-dessous.

>[!TIP]
>
>Bien que vous ayez la possibilité de choisir votre élément de bloc racine, nous vous recommandons toujours d’utiliser les paramètres par défaut pour une expérience utilisateur optimale.

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Modifier les paramètres de l’éditeur de texte]**.

   ![](assets/three.png)

1. Dans la liste déroulante **[!UICONTROL Éditeur de page de destination]**, sélectionnez `<p>` ou [!UICONTROL Aucun], puis cliquez sur **[!UICONTROL Enregistrer]**. `<p>` est utilisé dans cet exemple.

   ![](assets/five.png)

   Et c&#39;est tout !
