---
unique-page-id: 11371040
description: Syntaxe du modèle de courrier électronique - Documents Marketo - Documentation du produit
title: Syntaxe du modèle de courrier électronique
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 1%

---

# Syntaxe du modèle de courrier électronique {#email-template-syntax}

Dans Marketo, les modèles de courrier électronique sont composés de n’importe quelle combinaison d’éléments, de variables, de modules ou de conteneurs. Chacun d’eux est défini en ajoutant une syntaxe spécifique à Marketo à votre HTML. Les anciens modèles de courrier électronique (v1.0) sont pris en charge dans la version 2.0 de l’éditeur de courrier électronique ; toutefois, ils n’incluront pas toutes les nouvelles fonctionnalités de l’éditeur.

La syntaxe des emails Marketo ne fonctionne que dans les modèles et les emails individuels. Elle ne fonctionne **pas** si elle est incorporée dans des fragments de code ou des jetons de texte enrichi.

>[!NOTE]
>
>La prise en charge de Marketo n’est pas configurée pour faciliter l’utilisation de CSS/HTML. Si vous ne connaissez pas CSS/HTML, consultez votre développeur.

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

Si vous définissez une région comme texte enrichi, les utilisateurs pourront modifier son contenu [à l’aide de l’éditeur de texte enrichi Marketo ](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Il existe deux manières de définir un élément Texte enrichi à l’intérieur d’un modèle d’email : mktEditable et mktoText. Gardez à l’esprit qu’un élément de texte enrichi peut toujours être converti en extrait de code depuis l’éditeur de courrier électronique.

### Option 1 - mktEditable {#option-mkteditable}

Comme l’éditeur de messagerie 2.0 est rétrocompatible, certains anciens modèles de courrier électronique peuvent spécifier des éléments de texte enrichi en ajoutant class=&quot;mktEditable&quot; sur n’importe quel élément d’HTML. Ceci est toujours pris en charge et l’identifiant de l’élément est celui qui sera utilisé comme nom d’affichage dans l’éditeur de courrier électronique.

Attributs requis

* **class** : &quot;mktEditable&quot;.
* **id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.

Attributs facultatifs

* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut

Le contenu de l’élément HTML (s’il est fourni) avec class=&quot;mktEditable&quot; sera utilisé comme valeur par défaut pour l’élément Texte enrichi.

Exemple :

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Option 2 - mktoText {#option-mktotext}

Il est recommandé de spécifier des éléments de texte enrichi en utilisant la syntaxe class=&quot;mktoText&quot;. Cela permet de s’assurer qu’il existe toujours un nom d’affichage correct pour l’élément.

Attributs requis

* **class** : &quot;mktoText&quot;
* **id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut

Le contenu de l’élément HTML (s’il est fourni) avec class=&quot;mktoText&quot; sera utilisé comme valeur par défaut pour l’élément Texte enrichi.

Exemple :

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Images {#images}

Vous disposez de deux options pour définir des éléments Image modifiables. Vous pouvez utiliser une balise `<div>`, qui spécifie un conteneur dans lequel `<img>` sera inséré, ou une balise `<img>`. Si vous envisagez que l’utilisateur final sélectionne simplement une image qui renverra l’URL de l’image (par opposition au modèle DOM), reportez-vous aux &quot;variables d’image&quot; dans la section ci-dessous. Les deux options suivantes insèrent un élément d&#39;HTML `<img>`.

### Option 1 - Utilisation d’un `<div>` {#option-use-a-div}

Attributs requis

* **class:** &quot;mktoImg&quot;.
* **id :** Chaîne d&#39;identifiant. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName : chaîne**. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoImgClass:** Chaîne. La valeur ici sera ajoutée à l’attribut class de l’élément `<img>` dans la balise div.
* **mktoImgSrc:** À utiliser comme valeur par défaut pour l’image placée dans cette balise div. Un espace réservé est utilisé s’il est omis.
* **mktoImgLink:** Indique que l’ `<img>` doit être entouré d’une balise `<a>` avec cette URL de destination. L’utilisateur peut modifier ce paramètre dans l’éditeur de courrier électronique.
* **mktoImgLinkTarget:** Indique que la balise `<a>` de l’attribut mktoImgLink doit utiliser cette cible. N’a aucun effet si mktoImgLink n’est pas également utilisé.
* **mktoImgWidth:** Utilisé comme largeur sur `<img>` inclus.
* **mktoImgHeight:** Utilisé comme hauteur sur le `<img>` inclus.
* **mktoLockImgSize:** Utilisé pour déverrouiller la propriété de hauteur et de largeur de l’élément `<img>` afin que l’utilisateur final puisse la modifier (la valeur par défaut est true si elle est omise).
* **mktoLockImgStyle:** Utilisé pour verrouiller la propriété de style de l’élément `<img>` (la valeur par défaut est false).

Valeur par défaut (facultatif)

**`<img>`** : à utiliser comme élément `<img>` dans lequel l’image sera placée. Utile si vous souhaitez ajouter un style intégré à l’image. N’oubliez pas d’inclure les balises `<a> </a>` environnantes. Par conséquent, si l’utilisateur ajoute un lien, votre style ne sera pas supprimé.

Exemple :

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Option 2 - Utilisation d’un \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Cette option ne permet pas aux utilisateurs finaux d’ajouter un lien vers leur image. Utilisez l’option 1 si cela est important pour votre modèle.

Attributs requis

* **class:** &quot;mktoImg&quot;.
* **id :** Chaîne d&#39;identifiant. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName:** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.  Valeur par défaut (facultatif)
* **src:** À utiliser comme valeur par défaut de l’image. Un espace réservé est utilisé s’il est omis.
* **mktoLockImgSize:** Utilisé pour déverrouiller la propriété de hauteur et de largeur de l’élément `<img>` afin que l’utilisateur final puisse la modifier (la valeur par défaut est true si elle est omise).
* **mktoLockImgStyle:** Utilisé pour verrouiller la propriété de style de l’élément `<img>` (la valeur par défaut est false).

Exemple :
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Extraits {#snippets}

Si vous définissez une région comme Extrait de code, les utilisateurs finaux pourront choisir quel [Extrait de code](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)approuvé ils souhaitent insérer dans cette région. Bien que les éléments de texte enrichi puissent être convertis en fragments à partir de l’éditeur de courrier électronique, il est impossible de convertir les fragments de texte enrichi lorsque vous définissez une région spécifique en extrait de code. Vous pouvez spécifier une région de fragment de code à l’aide d’un `<div>` avec class=&quot;mktoSnippet&quot;.

Attributs requis

* **id :** Chaîne d&#39;identifiant. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName:** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut (facultatif)

**mktoDefaultSnippetId** : identifiant numérique du fragment de code Marketo qui doit apparaître par défaut (ne fonctionnera que si un fragment de code avec cet identifiant existe et est approuvé dans cet espace de travail).

Exemple :

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Vidéo {#video}

Si vous définissez une région sous la forme d’une vidéo, les utilisateurs finaux pourront insérer une URL YouTube ou Vimeo qui s’affichera sous forme d’une miniature (avec le bouton &quot;lecture&quot;) à l’intérieur de l’email. Vous pouvez spécifier une région Vidéo à l’aide d’un `<div>` avec class=&quot;mktoVideo&quot;

Attributs requis

* **id :** Chaîne d&#39;identifiant. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
* **mktoName:** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoImgClass:** Chaîne. La valeur ici sera ajoutée à l’attribut de classe de la miniature vidéo `<img>` dans la balise div.

Exemple :

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variables {#variables}

Les variables sont comme des jetons. Vous devez d’abord les définir dans la section `<head>` de votre modèle d’email à l’aide de balises `<meta>`, puis les utiliser autant de fois que vous le souhaitez dans l’ensemble de votre modèle. Comme elles sont définies dans le modèle, l’utilisateur final peut modifier leurs valeurs en fonction de ses règles. Notez que vous pouvez définir une variable comme étant de portée locale ou globale. Si vous utilisez une variable dans un &quot;module&quot; (voir ci-dessous) et qu’un utilisateur final duplique ce module, les variables locales auront des valeurs indépendantes, tandis que les variables globales s’appliqueront aux deux modules.

## Chaîne {#string}

Si vous spécifiez une variable sous forme de chaîne, l’utilisateur final pourra saisir du texte dans une zone de texte de l’éditeur de courrier électronique. Vous spécifiez une variable String en utilisant `<meta>` avec class=&quot;mktoString&quot;

Attributs requis

* **id :** Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName:** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **allowHTML :** booléen. Contrôle si la valeur de la variable est placée dans une séquence d’échappement par HTML. La valeur par défaut est False si elle est omise.
* **default** : valeur par défaut de la chaîne. Vide s’il est omis.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textHeader}</pre>`

## Liste {#list}

Si vous spécifiez une variable sous la forme d&#39;une liste, l&#39;utilisateur final pourra choisir parmi un ensemble de valeurs que vous définissez dans l&#39;éditeur de courrier électronique. Vous spécifiez une variable List en utilisant `<meta>` avec class=&quot;mktoList&quot;

Attributs requis

* **id** : manière dont vous référencez la variable dans votre modèle de courrier électronique.
* **mktoName:** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.
* **values :** Liste de valeurs séparées par des virgules. Doit comporter au moins une chaîne.

Attributs facultatifs

* **default :** Valeur par défaut de la liste déroulante de sélection. Si cette valeur est omise, la première valeur de l’attribut &quot;values&quot; est utilisée.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Nombre {#number}

Si vous définissez une variable comme Nombre, l&#39;utilisateur final pourra saisir un nombre dans l&#39;éditeur d&#39;email. Vous spécifiez une variable Number en utilisant `<meta>` avec class=&quot;mktoNumber&quot;

Attributs requis

* **id** : manière dont vous référencez la variable dans votre modèle de courrier électronique.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.
* **default :** Valeur numérique par défaut pour la variable.

Attributs facultatifs

* **min :** Min valeur acceptée.
* **max :** Max valeur acceptée.
* **unit:** Unités à ajouter à la valeur numérique (ex : px, pt, em, etc.) s’affiche dans l’éditeur d’email, ainsi que dans le code résultant.
* **étape :** nombre d’unités que la variable de nombre doit augmenter/diminuer de (0,1, 1, 10, etc.). Si cette valeur est omise, la valeur par défaut est 1.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Couleur {#color}

Si vous spécifiez une variable en tant que Couleur, l’utilisateur final pourra saisir une valeur de couleur hexadécimale ou choisir une couleur dans le sélecteur de couleurs de l’éditeur de courrier électronique. Vous spécifiez une variable Color en utilisant `<meta>` avec class=&quot;mktoColor&quot;

Attributs requis

* **id** : manière dont vous référencez la variable dans votre modèle de courrier électronique.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default:** Valeur par défaut de la couleur. Code couleur hexadécimal à 6 chiffres. Ex : #ffffff.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textColor}</pre>`

## Booléenne {#boolean}

Si vous définissez une variable comme valeur booléenne, l’utilisateur final pourra activer/désactiver l’option dans l’éditeur de courrier électronique. Vous spécifiez une variable booléenne en utilisant `<meta>` avec class=&quot;mktoBoolean&quot;

Attributs requis

* **id** : manière dont vous référencez la variable dans votre modèle de courrier électronique.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default:** Valeur booléenne déterminant l’état par défaut du commutateur de basculement. False s’il est omis.
* **false_value:** Valeur à insérer lorsque le bouton bascule est en position OFF. False s’il est omis.
* **true_value:** Valeur à insérer lorsque le bouton bascule est en position ON. True s’il est omis.
* **false_value_name :** l’interface utilisateur s’affiche lors du basculement en position de désactivation. False s’il est omis.
* **true_value_name:** IU affichée en mode activé lors du basculement. True s’il est omis.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloc d’HTML {#html-block}

Si vous spécifiez une variable comme bloc d’HTML, l’utilisateur final pourra saisir l’HTML du texte dans l’éditeur de courrier électronique. Vous spécifiez une variable de bloc d’HTML à l’aide de `<meta>` avec class=&quot;mktoHTML&quot;.

Attributs requis

* **id** : manière dont vous référencez la variable dans votre modèle de courrier électronique.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default :** HTML la valeur codée pour servir de contenu par défaut du bloc.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variable d’image {#image-variable}

Si vous définissez une variable comme Image, l’utilisateur final pourra choisir une image dans le sélecteur d’image de l’éditeur de courrier électronique. L’URL d’image sélectionnée correspond à la valeur de la variable. Vous spécifiez une variable d&#39;image à l&#39;aide de `<meta>` avec class=&quot;mktoImg&quot;

Attributs requis

* **id** : manière dont vous référencez la variable dans votre modèle de courrier électronique.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default :** URL d’image par défaut pour l’élément.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Modules {#modules}

Les modules sont des sections modélisées définies au niveau du modèle qui s’afficheront pour que les utilisateurs finaux puissent les insérer dans leur email. Puisque vous avez préconfiguré ces modules, vous pouvez vous assurer qu’ils interagiront avec le reste de votre contenu d’email de manière correcte (de manière entièrement réactive). Vous pouvez uniquement placer un module dans un conteneur.

>[!IMPORTANT]
>
>Lorsqu’un email est généré à partir d’un modèle d’email qui contient des composants de module définis, toute modification apportée aux modules du modèle sera **et non** envoyée à cet email.

**Pour les conteneurs de type `<table>`, `<tbody>`, `<thead>` ou `<tfoot>` :**

Spécifié avec `<tr>` avec class=&quot;mktoModule&quot;

**Pour les conteneurs de type `<td>`:**

Spécifié avec `<table>` avec class=&quot;mktoModule&quot;

Attributs requis

* **id** : manière dont vous référencez le module dans votre modèle de courrier électronique.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de messagerie 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoActive :** détermine si ce module apparaît dans la liste des modules de l’éditeur de messagerie. La valeur par défaut est true. Si la valeur est false, le module ne peut pas être ajouté par un utilisateur final à un email.
* **mktoAddByDefault :** détermine si ce module sera dans la zone de travail d’un nouvel email qui utilise ce modèle lors de sa création. La valeur par défaut est true (si mktoActive a la valeur false, cette valeur est ignorée).

>[!NOTE]
>
>Les valeurs de classe contenant la syntaxe Marketo (c’est-à-dire mktoModule, mktoContainer, mktoText) sont sensibles à la casse. Les noms d’attribut personnalisés (c’est-à-dire mktoimgwidth, mktoname) ne le sont pas.

## Conteneurs {#containers}

Un conteneur contient des modules et définit l’emplacement où ils peuvent être placés. Lorsque les utilisateurs finaux réorganisent et insèrent des modules dans leur email, le conteneur contrôle où ils peuvent se rendre.

**Spécifié à l’aide de `<table>`, `<tbody>`, `<thead>`, `<tfoot>` ou `<td>` avec class=&quot;mktoContainer&quot;**

Attributs requis

**id** : manière dont vous référencez le module dans votre modèle de courrier électronique.

>[!CAUTION]
>
>Les conteneurs ne peuvent contenir que des modules. S’il existe autre chose, le conteneur est considéré comme non valide. Un seul conteneur est autorisé par modèle.
