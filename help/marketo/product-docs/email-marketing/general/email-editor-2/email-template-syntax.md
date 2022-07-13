---
unique-page-id: 11371040
description: Syntaxe du modèle de courrier électronique - Documents Marketo - Documentation du produit
title: Syntaxe du modèle de courrier électronique
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
source-git-commit: a59b6b2505c6e5a83c6137a1925aa4e60e56eac8
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 1%

---

# Syntaxe du modèle de courrier électronique {#email-template-syntax}

Dans Marketo, les modèles de courrier électronique sont composés de n’importe quelle combinaison d’éléments, de variables, de modules ou de conteneurs. Chacun d’eux est défini en ajoutant une syntaxe spécifique à Marketo à votre HTML. Les anciens modèles de courrier électronique (v1.0) sont pris en charge dans Email Editor 2.0 ; toutefois, elles n’incluront pas toutes les fonctions du nouvel éditeur.

La syntaxe des emails Marketo ne fonctionne que dans les modèles et les emails individuels. it **not** fonctionnent si elles sont incorporées dans des fragments de code ou des jetons de texte enrichi.

>[!NOTE]
>
>La prise en charge de Marketo n’est pas configurée pour prendre en charge CSS/HTML. Si vous ne connaissez pas le CSS/HTML, consultez votre développeur.

>[!CAUTION]
>
>Les valeurs de classe contenant la syntaxe Marketo (c’est-à-dire mktoModule, mktoContainer, mktoText) sont sensibles à la casse. Les noms d’attribut personnalisés (c’est-à-dire mktoimgwidth, mktoname) ne le sont pas.

## Éléments {#elements}

Les éléments sont des zones de contenu que vous définissez comme modifiables dans votre modèle de courrier électronique. L’expérience d’édition d’un élément est propre à son type et offre un moyen simple d’utiliser le contenu. Les éléments possibles pouvant être inclus dans un modèle d&#39;email sont les suivants :

* Texte complet
* Images
* Extraits
* Vidéos

## Texte complet {#rich-text}

Si vous définissez une région comme Texte enrichi, les utilisateurs pourront modifier son contenu. [Utilisation de l’éditeur de texte enrichi Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Il existe deux manières de définir un élément Texte enrichi à l’intérieur d’un modèle d’email : mktEditable et mktoText. Gardez à l’esprit qu’un élément de texte enrichi peut toujours être converti en extrait de code depuis l’éditeur de courrier électronique.

### Option 1 - mktEditable {#option-mkteditable}

Comme l’éditeur de messagerie 2.0 est rétrocompatible, certains anciens modèles de courrier électronique peuvent spécifier des éléments de texte enrichi en ajoutant class=&quot;mktEditable&quot; sur n’importe quel élément de HTML. Ceci est toujours pris en charge et l’identifiant de l’élément est celui qui sera utilisé comme nom d’affichage dans l’éditeur de courrier électronique.

Attributs requis

* **class**: &quot;mktEditable&quot;.
* **id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.

Attributs facultatifs

* **mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut

Le contenu de l’élément de HTML (s’il est fourni) avec class=&quot;mktEditable&quot; sera utilisé comme valeur par défaut pour l’élément Texte enrichi.

Exemple :

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Option 2 - mktoText {#option-mktotext}

Il est recommandé de spécifier des éléments de texte enrichi en utilisant la syntaxe class=&quot;mktoText&quot;. Cela garantit qu’il existe toujours un nom d’affichage correct pour l’élément.

Attributs requis

* **class**: &quot;mktoText&quot;
* **id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut

Le contenu de l’élément de HTML (s’il est fourni) avec class=&quot;mktoText&quot; sera utilisé comme valeur par défaut pour l’élément Texte enrichi.

Exemple :

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Images {#images}

Vous disposez de deux options pour définir des éléments Image modifiables. Vous pouvez utiliser une `<div>`, qui spécifie un conteneur qui `<img>` est inséré dans ou un `<img>` balise . Si vous envisagez que l’utilisateur final sélectionne simplement une image qui renverra l’URL de l’image (par opposition au modèle DOM), reportez-vous aux &quot;variables d’image&quot; dans la section ci-dessous. Les deux options suivantes insèrent un HTML : `<img>` élément .

### Option 1 - Utilisez une `<div>` {#option-use-a-div}

Attributs requis

* **Classe :** &quot;mktoImg&quot;.
* **id:** Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoImgClass:** Chaîne. La valeur ici sera ajoutée à l’attribut de classe de la propriété `<img>` élément dans la balise div.
* **mktoImgSrc :** À utiliser comme valeur par défaut de l’image placée dans cette balise div. Un espace réservé est utilisé s’il est omis.
* **mktoImgLink :** Indiquez que la variable `<img>` doit être entouré d’un `<a>` avec cette URL de destination. L’utilisateur peut modifier ce paramètre dans l’éditeur de courrier électronique.
* **mktoImgLinkTarget :** Indiquez que la variable `<a>` La balise de l’attribut mktoImgLink doit utiliser cette cible. N’a aucun effet si mktoImgLink n’est pas également utilisé.
* **mktoImgWidth :** Utilisé comme largeur sur l’objet inclus `<img>`.
* **mktoImgHeight :** Utilisé comme hauteur sur l’objet inclus `<img>`.
* **mktoLockImgSize :** Utilisé pour déverrouiller la variable `<img>` de la hauteur et de la largeur de l’élément afin que l’utilisateur final puisse la modifier (la valeur par défaut est true si elle est omise).
* **mktoLockImgStyle:** Utilisé pour verrouiller la variable `<img>` propriété de style de l’élément (la valeur par défaut est false).

Valeur par défaut (facultatif)

**`<img>`**: À utiliser comme `<img>` élément dans lequel l’image sera placée. Utile si vous souhaitez ajouter un style intégré à l’image. N’oubliez pas d’inclure les `<a> </a>` , donc si l’utilisateur ajoute un lien, votre style ne sera pas supprimé.

Exemple :

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Option 2 - Utiliser un \&lt;img> {#option-use-an-img}

>[!NOTE]
>
>Cette option ne permet pas aux utilisateurs finaux d’ajouter un lien vers leur image. Utilisez l’option 1 si cela est important pour votre modèle.

Attributs requis

* **Classe :** &quot;mktoImg&quot;.
* **id:** Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.  Valeur par défaut (facultatif)
* **src :** À utiliser comme valeur par défaut de l’image. Un espace réservé est utilisé s’il est omis.
* **mktoLockImgSize :** Utilisé pour déverrouiller la variable `<img>` de la hauteur et de la largeur de l’élément afin que l’utilisateur final puisse la modifier (la valeur par défaut est true si elle est omise).
* **mktoLockImgStyle:** Utilisé pour verrouiller la variable `<img>` propriété de style de l’élément (la valeur par défaut est false).

Exemple:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Extraits {#snippets}

Si vous définissez une région comme extrait de code, les utilisateurs finaux pourront choisir la région approuvée. [Fragment de code](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)ils souhaitent insérer dans cette région. Bien que les éléments de texte enrichi puissent être convertis en fragments à partir de l’éditeur de courrier électronique, il est impossible de convertir les fragments de texte enrichi lorsque vous définissez une région spécifique en extrait de code. Vous pouvez spécifier une région de fragment de code à l’aide d’une `<div>` with class=&quot;mktoSnippet&quot;

Attributs requis

* **id:** Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut (facultatif)

**mktoDefaultFragmentId**: L’identifiant numérique du fragment de code Marketo qui doit apparaître par défaut (ne fonctionne que si un fragment de code avec cet identifiant existe et est approuvé dans cet espace de travail).

Exemple :

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Vidéo {#video}

Si vous définissez une région sous la forme d’une vidéo, les utilisateurs finaux pourront insérer une URL YouTube ou Vimeo qui s’affichera sous forme d’une miniature (avec le bouton &quot;lecture&quot;) à l’intérieur de l’email. Vous pouvez spécifier une région Vidéo à l’aide d’une `<div>` with class=&quot;mktoVideo&quot;

Attributs requis

* **id:** Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoImgClass:** Chaîne. La valeur ici sera ajoutée à l’attribut de classe de la miniature vidéo. `<img>` dans la balise div.

Exemple :

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variables {#variables}

Les variables sont comme des jetons. Vous devez d’abord les définir dans la variable `<head>` section de votre modèle d’email utilisant `<meta>` puis les utiliser autant de fois que vous le souhaitez dans votre modèle. Comme elles sont définies dans le modèle, l’utilisateur final peut modifier leurs valeurs en fonction de ses règles. Notez que vous pouvez définir une variable comme étant de portée locale ou globale. Si vous utilisez une variable dans un &quot;module&quot; (voir ci-dessous) et qu’un utilisateur final duplique ce module, les variables locales auront des valeurs indépendantes, tandis que les variables globales s’appliqueront aux deux modules.

## Chaîne {#string}

Si vous spécifiez une variable sous la forme d’une chaîne, l’utilisateur final pourra saisir du texte dans une zone de texte de l’éditeur de courrier électronique. Vous spécifiez une variable String à l’aide de `<meta>` with class=&quot;mktoString&quot;

Attributs requis

* **id:** Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **allowHTML :** Booléen. Contrôle si la valeur de la variable est placée dans une séquence d’échappement par HTML. La valeur par défaut est False si elle est omise.
* **default**: Valeur par défaut de la chaîne. Vide s’il est omis.
* **mktoModuleScope**: Booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textHeader}</pre>`

## Liste {#list}

Si vous spécifiez une variable sous la forme d&#39;une liste, l&#39;utilisateur final pourra choisir parmi un ensemble de valeurs que vous définissez dans l&#39;éditeur de courrier électronique. Vous spécifiez une variable de liste à l’aide de la variable `<meta>` with class=&quot;mktoList&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.
* **values :** Liste de valeurs séparées par des virgules. Doit comporter au moins une chaîne.

Attributs facultatifs

* **default :** Valeur par défaut de la liste déroulante de sélection. Si cette valeur est omise, la première valeur de l’attribut &quot;values&quot; est utilisée.
* **mktoModuleScope**: Booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Nombre {#number}

Si vous définissez une variable comme Nombre, l&#39;utilisateur final pourra saisir un nombre dans l&#39;éditeur d&#39;email. Vous spécifiez une variable Number à l’aide de `<meta>` with class=&quot;mktoNumber&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.
* **default :** Valeur numérique par défaut de la variable.

Attributs facultatifs

* **min :** Min valeur acceptée.
* **max :** Max. valeur acceptée.
* **unit :** Unités à ajouter à la valeur numérique (ex : px, pt, em, etc.) s’affiche dans l’éditeur d’email, ainsi que dans le code résultant.
* **étape :** Nombre d’unités que la variable de nombre doit augmenter/diminuer de (0,1, 1, 10, etc.). Si cette valeur est omise, la valeur par défaut est 1.
* **mktoModuleScope**: Booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Couleur {#color}

Si vous spécifiez une variable en tant que Couleur, l’utilisateur final pourra saisir une valeur de couleur hexadécimale ou choisir une couleur dans le sélecteur de couleurs de l’éditeur de courrier électronique. Vous spécifiez une variable Color à l’aide de `<meta>` with class=&quot;mktoColor&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default :** Valeur par défaut de la couleur. Code couleur hexadécimal à 6 chiffres. Ex : #ffffff.
* **mktoModuleScope**: Booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textColor}</pre>`

## Booléenne {#boolean}

Si vous définissez une variable comme valeur booléenne, l’utilisateur final pourra activer/désactiver l’option dans l’éditeur de courrier électronique. Vous spécifiez une variable booléenne à l’aide de la variable `<meta>` with class=&quot;mktoBoolean&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default :** Valeur booléenne déterminant l’état par défaut du bouton bascule. False si omis.
* **false_value:** Valeur à insérer lorsque le bouton bascule est en position OFF. False si omis.
* **true_value:** Valeur à insérer lorsque le bouton bascule est en position ON. True s’il est omis.
* **false_value_name:** IU affichée dans le bouton d’activation/désactivation en position OFF. False si omis.
* **true_value_name:** IU affichée dans le bouton bascule en position ON. True s’il est omis.
* **mktoModuleScope**: Booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloc de HTML {#html-block}

Si vous spécifiez une variable comme bloc de HTML, l’utilisateur final pourra saisir le HTML textuel depuis l’éditeur de courrier électronique. Vous spécifiez une variable de bloc de HTML à l’aide de `<meta>` with class=&quot;mktoHTML&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default :** Valeur codée en HTML qui sert de contenu par défaut au bloc.
* **mktoModuleScope**: Booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variable d’image {#image-variable}

Si vous définissez une variable comme Image, l’utilisateur final pourra choisir une image dans le sélecteur d’image de l’éditeur de courrier électronique. L’URL d’image sélectionnée correspond à la valeur de la variable. Vous spécifiez une variable d’image à l’aide de `<meta>` with class=&quot;mktoImg&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default :** URL de l’image par défaut pour l’élément.
* **mktoModuleScope**: Booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Modules {#modules}

Les modules sont des sections modélisées définies au niveau du modèle qui s’afficheront pour que les utilisateurs finaux puissent les insérer dans leur email. Puisque vous avez préconfiguré ces modules, vous pouvez vous assurer qu’ils interagiront avec le reste de votre contenu d’email de manière correcte (de manière entièrement réactive). Vous pouvez uniquement placer un module dans un conteneur.

>[!IMPORTANT]
>
>Lorsqu’un email est généré à partir d’un modèle de courrier électronique qui contient des composants de module définis, toute modification apportée aux modules du modèle est **not** être poussé vers cet e-mail.

**Pour les conteneurs de type `<table>`, `<tbody>`, `<thead>`ou `<tfoot>`:**

Spécifié à l’aide de `<tr>` with class=&quot;mktoModule&quot;

**Pour les conteneurs de type `<td>`:**

Spécifié à l’aide de `<table>` with class=&quot;mktoModule&quot;

Attributs requis

* **id**: Comment référencer le module dans votre modèle d’email.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans la version 2.0 de l’éditeur de messagerie. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoActive:** Détermine si ce module apparaît dans la liste des modules de l’éditeur de messagerie. La valeur par défaut est true. Si la valeur est false, le module ne peut pas être ajouté par un utilisateur final à un email.
* **mktoAddByDefault :** Détermine si ce module se trouve dans le canevas d’un nouvel email qui utilise ce modèle lors de sa création. La valeur par défaut est true (si mktoActive a la valeur false, cette valeur est ignorée).

>[!NOTE]
>
>Les valeurs de classe contenant la syntaxe Marketo (c’est-à-dire mktoModule, mktoContainer, mktoText) sont sensibles à la casse. Les noms d’attribut personnalisés (c’est-à-dire mktoimgwidth, mktoname) ne le sont pas.

## Conteneurs {#containers}

Un conteneur contient des modules et définit l’emplacement où ils peuvent être placés. Lorsque les utilisateurs finaux réorganisent et insèrent des modules dans leur email, le conteneur contrôle où ils peuvent se rendre.

**Spécifié à l’aide de `<table>`, `<tbody>`, `<thead>`, `<tfoot>` ou `<td>` with class=&quot;mktoContainer&quot;**

Attributs requis

**id**: Comment référencer le module dans votre modèle d’email.

>[!CAUTION]
>
>Les conteneurs ne peuvent contenir que des modules. S’il existe autre chose, le conteneur est considéré comme non valide. Un seul conteneur est autorisé par modèle.
