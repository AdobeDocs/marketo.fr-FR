---
unique-page-id: 2953419
description: Utilisation de l’éditeur de texte enrichi - Documents marketing - Documentation du produit
title: Utilisation de l’éditeur de texte enrichi
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---


# Utilisation de l’éditeur de texte enrichi {#using-the-rich-text-editor}

L’Editeur de texte enrichi (RTE) s’affiche dans tout le marché et est disponible chaque fois que vous souhaitez ajouter ou modifier du contenu. Vous en verrez une version sur landings page, programmes, courriels, formulaires et extraits de code. Il vous suffit de cliquer sur **Modifier le brouillon** et il apparaîtra pour vous servir.

## Paramètres de l’éditeur {#editor-settings}

Le paramètre d’élément de bloc racine définit les balises qui encapsulent votre contenu. Par défaut, l’élément de bloc racine de courrier électronique utilise <p> balises. Vous avez la possibilité de changer cela en suivant les étapes ci-dessous.

>[!TIP]
>
>Bien que vous ayez la possibilité de choisir votre élément de bloc racine, nous vous recommandons toujours d’utiliser les paramètres par défaut pour optimiser la satisfaction des utilisateurs.

1. Cliquez sur **Admin**.

   ![](assets/one.png)

1. Cliquez sur **Courriel**.

   ![](assets/two.png)

1. Cliquez sur **Modifier les paramètres de l’éditeur de texte**.

   ![](assets/three.png)

1. Dans la liste déroulante **Éditeur de courriel / extrait de code**, sélectionnez <div> ou Aucun et cliquez sur **Enregistrer**. <div> est utilisée dans cet exemple.

   ![](assets/four.png)

   Si vous avez <div class="&ldquo;mktEditable&rdquo;"></div> dans un modèle de courrier électronique, le comportement de la source HTML suivante s’affiche lorsque vous ouvrez la section et que vous tapez &quot;Texte ici&quot; dans l’éditeur :

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Aucun</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;p&gt;Le texte se trouve ici&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;div&gt;Le texte se trouve ici&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>Le texte se trouve ici<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Vous pouvez également modifier l’élément de bloc racine de l’éditeur de Landing page en suivant les mêmes étapes, mais en cliquant sur la liste déroulante **Éditeur de Landing page** à l’étape 4 au lieu de l’Éditeur de courriel/d’extrait de code.

>[!NOTE]
>
>L&#39;élément de bloc racine est toujours <p> pour les jetons de programme en texte enrichi.

## Fonctionnalités {#features}

Voici les fonctionnalités que vous trouverez dans un RTE.

| Icône | Nom | Contenu |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | Famille de polices | Choisissez votre style : nous en avons plein ! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | Taille de police | Quelle taille en voulez-vous ? 25 choix, de 8px à 90px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | Styles | Choisissez Paragraphe ou six styles d’en-tête (pour les landings page). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | Interligne | Choisissez la distance entre les lignes. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | Couleur du texte | Noir, rouge, ou quoi que ce soit que vous vouliez. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | Couleur d’arrière-plan | Mettez l’accent en évidence. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | Gras | **Plus sombre et plus épais**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | Italique | *Angled, pour l&#39;accent ou les* citations. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | Souligné | Place une ligne sous votre texte. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | Alignement | Utilisez cette liste déroulante pour mettre en forme votre texte et vos images. Centre-les, choisissez l’alignement à gauche ou à droite ou étalonnez-le d’un bord à l’autre avec une justification complète. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Liste | Choisissez des puces ou des nombres dans la liste déroulante. Les puces sont bonnes pour les listes et les nombres avec les étapes. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | Retrait | Choisissez une mise en retrait plus ou moins importante. Utilisez cette option pour les paragraphes ou tout texte à mettre en évidence. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | Insérer/modifier un lien | insérer un lien vers un site Web ou un autre contenu ; il est facile d&#39;y apporter des modifications. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | Insérer/modifier une image | Une image vaut mille mots. Lâchez-en un. Cliquez sur l’icône d’appareil photo pour parcourir votre studio de création. Vous pouvez déposer des images côte à côte. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | Insérer un jeton | Un outil puissant, idéal pour la personnalisation des courriels et le suivi des données. Veillez à entrer une valeur par défaut. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | Annuler | Oups ! Revenons en arrière et recommençons. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | Rétablir | Si c&#39;est vraiment bon, revenez à l&#39;original. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | Tableau | Construisez la vôtre, comme celle-ci. Un menu déroulant vous permet de le configurer. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | Insérer un ancrage | Déposez l&#39;ancre ! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | Ligne horizontale | Plusieurs utilisations : idéal pour diviser les sections. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | Modifier HTML | Affiche l’éditeur de source HTML afin que vous puissiez ajuster votre code. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | Indice | Lettres en attente basse (comme dans O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | Exposant | Vous avez le pouvoir ! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | Barré | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | Caractère spécial | Vous voulez parler d&#39;euros ? Les maths ? Vous avez 243 choix. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | Rechercher et remplacer | Recherchez et modifiez les éléments beaucoup plus rapidement que chaque instance vous-même. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | Effacer la mise en forme | Renvoyez les choses à la norme. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | Annuler | Appuyez sur le bouton pour dire : &quot;Peu importe.&quot; |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | Enregistrer | Appuyez sur le bouton pour dire : &quot;OK, je l&#39;aime.&quot; |

>[!TIP]
>
>Vous modifiez le code HTML et le texte sur des écrans distincts. Veillez à cliquer sur **Copier à partir du code HTML** dans l&#39;onglet **Texte**, puis sur **Enregistrer** pour que votre texte corresponde à votre code HTML.

>[!NOTE]
>
>Vous n’êtes pas limité aux polices dans la liste déroulante. Vous pouvez en utiliser un qui ne figure pas dans la liste en accédant au code HTML. Toutes les polices web sont prises en charge dans Marketing Cloud, mais les polices web ne fonctionnent pas de manière universelle dans tous les clients de messagerie.

## landings page {#landing-pages}

Le paramètre d’élément de bloc racine définit les balises qui encapsulent votre contenu. Par défaut, l’élément de bloc racine du landing page utilise <div> balises. Vous avez la possibilité de changer cela en suivant les étapes ci-dessous.

>[!TIP]
>
>Bien que vous ayez la possibilité de choisir votre élément de bloc racine, nous vous recommandons toujours d’utiliser les paramètres par défaut pour optimiser la satisfaction des utilisateurs.

1. Cliquez sur **Admin**.

   ![](assets/one.png)

1. Cliquez sur **Courriel**.

   ![](assets/two.png)

1. Cliquez sur **Modifier les paramètres de l’éditeur de texte**.

   ![](assets/three.png)

1. Dans la liste déroulante **Éditeur de Landing page**, sélectionnez <p> ou Aucun et cliquez sur **Enregistrer**. <p> est utilisée dans cet exemple.

   ![](assets/five.png)

   Et c&#39;est tout !

