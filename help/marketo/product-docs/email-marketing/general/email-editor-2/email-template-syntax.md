---
unique-page-id: 11371040
description: Syntaxe du modèle de courrier électronique - Documents marketing - Documentation du produit
title: Syntaxe du modèle de courriel
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 0%

---


# Syntaxe du modèle de courriel {#email-template-syntax}

Dans la nouvelle expérience d’e-mail 2.0 de Marketo, les modèles de courrier électronique sont composés de n’importe quelle combinaison d’éléments, de variables, de modules ou de Conteneurs. Chacun d’eux est défini en ajoutant une syntaxe spécifique au marketing à votre code HTML. Les anciens modèles de courrier électronique (v1.0) sont pris en charge dans la version 2.0 de l’éditeur de courrier électronique ; toutefois, elles n&#39;incluront pas toutes les fonctionnalités de la nouvelle rédaction.

La syntaxe des courriers électroniques de marketing ne fonctionne que dans les modèles et les courriers électroniques individuels ; il **ne fonctionne pas** s’il est incorporé dans des extraits de code ou des jetons de texte enrichi.

>[!NOTE]
>
>La prise en charge de Marketo n’est pas configurée pour aider à l’utilisation de CSS/HTML. Si vous ne connaissez pas CSS/HTML, consultez votre développeur.

>[!CAUTION]
>
>Les valeurs de classe contenant la syntaxe Marketo (c.-à-d. mktoModule, mktoContainer, mktoText) sont sensibles à la casse. Les noms d’attribut personnalisés (c.-à-d. mktoimgwidth, mktoname) ne le sont pas.

## Eléments {#elements}

Les éléments sont des zones de contenu que vous définissez comme modifiables dans votre modèle de courrier électronique. L’expérience de modification d’un élément est propre à son type et ses offres offrent une façon simple de travailler avec le contenu. Les éléments qui peuvent être inclus dans un modèle de courrier électronique sont les suivants :

* Texte enrichi
* Images
* Extraits de code
* Vidéos

## Texte enrichi {#rich-text}

Si vous définissez une zone de texte enrichi, les utilisateurs pourront modifier son contenu [à l’aide de l’éditeur](../../../../product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)de texte enrichi de Marketing Cloud. Il existe deux manières de définir un élément Texte enrichi dans un modèle de courrier électronique : mktEditable et mktoText. N’oubliez pas qu’un élément de texte enrichi peut toujours être converti en extrait de code à partir de l’éditeur de courrier électronique.

### Option 1 - mktEditable {#option-mkteditable}

Etant donné que la version 2.0 de l’éditeur de messagerie est rétrocompatible, certains anciens modèles de courrier électronique peuvent spécifier des éléments de texte enrichi en ajoutant class=&quot;mktEditable&quot; sur tout élément HTML. Ceci est toujours pris en charge et l’identifiant de l’élément est celui qui sera utilisé comme nom d’affichage dans l’éditeur de courrier électronique.

Attributs requis

* **classe**: &quot;mktEditable&quot;.
* **id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.

Attributs facultatifs

* **mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Valeur par défaut

Le contenu de l’élément HTML (s’il est fourni) avec class=&quot;mktEditable&quot; sera utilisé comme valeur par défaut pour l’élément Texte enrichi.

Exemple :

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Option 2 - mktoText {#option-mktotext}

Il est recommandé de spécifier des éléments de texte enrichi en utilisant la syntaxe class=&quot;mktoText&quot;. Cela permet de s’assurer qu’il existe toujours un nom d’affichage correct pour l’élément.

Attributs requis

* **classe**: &quot;mktoText&quot;
* **id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.
* **mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Valeur par défaut

Le contenu de l’élément HTML (s’il est fourni) avec class=&quot;mktoText&quot; sera utilisé comme valeur par défaut pour l’élément Texte enrichi.

Exemple :

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Images {#images}

Vous disposez de deux options pour définir des éléments d’image modifiables. Vous pouvez utiliser soit un `<div>`, qui spécifie un conteneur dans lequel la `<img>` balise sera insérée, soit une `<img>` balise. Si vous souhaitez que l’utilisateur final sélectionne simplement une image qui renverra l’URL de l’image (par opposition au modèle DOM), reportez-vous aux &quot;variables d’image&quot; dans la section ci-dessous. Les deux options suivantes vont insérer un `<img>` élément HTML.

### Option 1 - Utiliser un \&lt;div\> {#option-use-a-div}

Attributs requis

* **class :** &quot;mktoImg&quot;.
* **id:** Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Attributs facultatifs

* **mktoImgClass:** Chaîne. La valeur ici sera ajoutée à l&#39;attribut de classe de l&#39; `<img>` élément dans la balise div.
* **mktoImgSrc :** À utiliser comme valeur par défaut pour l’image placée dans cette balise div. Un espace réservé est utilisé s’il est omis.
* **mktoImgLink :** Indiquez que la balise `<img>` doit être entourée d’une `<a>` balise avec cette URL de destination. L’utilisateur peut modifier ce paramètre dans l’éditeur de messagerie.
* **mktoImgLinkTarget :** Indiquez que la `<a>` balise de l’attribut mktoImgLink doit utiliser cette cible. N&#39;a aucun effet si mktoImgLink n&#39;est pas également utilisé.
* **mktoImgWidth :** Utilisé comme largeur sur l’objet `<img>`.
* **mktoImgHeight :** Utilisée comme hauteur sur le `<img>`segment.
* **mktoLockImgSize :** Utilisé pour déverrouiller la propriété de hauteur et de largeur de l’ `<img>` élément afin que l’utilisateur final puisse le modifier (la valeur par défaut est true en cas d’omission).
* **mktoLockImgStyle :** Permet de verrouiller la propriété style de l’ `<img>` élément (false par défaut).

Valeur par défaut (facultative)

**`<img>`**: À utiliser comme `<img>` élément dans lequel l’image sera placée. Utile si vous souhaitez ajouter un style intégré à l’image. Pensez à inclure `<a> </a>` des balises environnantes. Par conséquent, si l’utilisateur ajoute un lien, votre style ne sera pas supprimé !

Exemple :

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="http://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Option 2 - Utiliser un \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Cette option ne permet pas aux utilisateurs finaux d’ajouter un lien vers leur image. Utilisez l’option 1 si cela est important pour votre modèle.

Attributs requis

* **class :** &quot;mktoImg&quot;.
* **id:** Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.  Valeur par défaut (facultative)
* **src :** A utiliser comme valeur par défaut pour l’image. Un espace réservé est utilisé s’il est omis.
* **mktoLockImgSize :** Utilisé pour déverrouiller la propriété de hauteur et de largeur de l’ `<img>` élément afin que l’utilisateur final puisse le modifier (la valeur par défaut est true en cas d’omission).
* **mktoLockImgStyle :** Permet de verrouiller la propriété style de l’ `<img>` élément (false par défaut).

Exemple :
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Extraits de code {#snippets}

Si vous définissez une région en tant qu&#39;extrait de code, les utilisateurs finaux seront en mesure de choisir quel [](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)extrait approuvé ils souhaitent insérer dans cette région. Bien que les éléments de texte enrichi puissent être convertis en extraits de code à partir de l’éditeur de messagerie, lorsque vous définissez une région spécifique en extrait de code, il ne peut pas être converti en texte enrichi. Vous pouvez spécifier une région d&#39;extrait de code à l&#39;aide d&#39;un `<div>` avec class=&quot;mktoSnippet&quot;.

Attributs requis

* **id:** Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Valeur par défaut (facultative)

**mktoDefaultSnippetId**: ID numérique du fragment de code marketing qui doit s’afficher par défaut (ne fonctionne que si un extrait de code portant cet ID existe et est approuvé dans cet espace de travail).

Exemple :

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Vidéo {#video}

Si vous définissez une région en tant que vidéo, les utilisateurs finaux peuvent insérer une URL YouTube ou Vimeo qui s’affichera sous forme de miniature (avec le bouton &quot;play&quot;) à l’intérieur du courrier électronique. Vous pouvez spécifier une région Vidéo à l’aide d’une `<div>` zone avec class=&quot;mktoVideo&quot;.

Attributs requis

* **id:** Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Attributs facultatifs

* **mktoImgClass:** Chaîne. La valeur ici sera ajoutée à l&#39;attribut de classe de la miniature vidéo `<img>` dans la balise div.

Exemple :

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variables {#variables}

Les variables sont semblables à des jetons. Vous devez d’abord les définir dans la `<head>` section de votre modèle de courrier électronique à l’aide de `<meta>` balises, puis les utiliser autant de fois que vous le souhaitez dans l’ensemble de votre modèle. Etant donné qu’ils sont définis dans le modèle, l’utilisateur final peut modifier leurs valeurs en fonction de leurs règles. Notez que vous pouvez définir une variable comme étant locale ou globale dans la portée. Si vous utilisez une variable dans un &quot;module&quot; (voir ci-dessous) et qu’un utilisateur final duplicata ce module, les variables locales auront des valeurs indépendantes, tandis que les variables globales s’appliqueront aux deux modules.

## Chaîne {#string}

Si vous spécifiez une variable sous la forme d’une chaîne, l’utilisateur final pourra saisir du texte dans une zone de texte de l’éditeur de courrier électronique. Vous spécifiez une variable String à l’aide `<meta>` de class=&quot;mktoString&quot;

Attributs requis

* **id:** Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Attributs facultatifs

* **allowHTML:** Boolean. Contrôle si la valeur de la variable est une séquence d’échappement HTML. La valeur par défaut est False si elle est omise.
* **par défaut**: Valeur par défaut de la chaîne. Vide si omis.
* **mktoModuleScope**: Boolean. Contrôle si la variable est locale (true) ou globale (false) lorsqu&#39;elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textHeader}</pre>`

## Liste {#list}

Si vous spécifiez une variable comme Liste, l’utilisateur final pourra choisir parmi un ensemble de valeurs que vous définissez dans l’éditeur de courrier électronique. Vous spécifiez une variable de Liste à l’aide `<meta>` de class=&quot;mktoList&quot;.

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName :** Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.
* **values:** Liste de valeurs séparées par des virgules. Doit contenir au moins une chaîne.

Attributs facultatifs

* **default:** Valeur par défaut de la liste déroulante de sélection. Si elle est omise, la première valeur de l’attribut &quot;valeurs&quot; est utilisée.
* **mktoModuleScope**: Boolean. Contrôle si la variable est locale (true) ou globale (false) lorsqu&#39;elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Nombre {#number}

Si vous spécifiez une variable sous la forme d’un nombre, l’utilisateur final pourra entrer un nombre dans l’éditeur de courrier électronique. Vous spécifiez une variable Number à l’aide `<meta>` de class=&quot;mktoNumber&quot;.

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.
* **default:** Valeur numérique par défaut de la variable.

Attributs facultatifs

* **min :** Valeur minimale acceptée.
* **max :** Valeur maximale acceptée.
* **unités :** Unités à ajouter à la valeur numérique (ex : px, pt, em, etc.) s’affiche dans l’éditeur de messagerie, ainsi que dans le code résultant.
* **step:** Combien d&#39;unités la variable numérique doit augmenter/diminuer de (0,1, 1, 10, etc.). Si ce paramètre est omis, la valeur par défaut est 1.
* **mktoModuleScope**: Boolean. Contrôle si la variable est locale (true) ou globale (false) lorsqu&#39;elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Couleur {#color}

Si vous spécifiez une variable en tant que Couleur, l’utilisateur final pourra saisir une valeur de couleur hexadécimale ou choisir une couleur dans le sélecteur de couleurs de l’éditeur de courrier électronique. Vous spécifiez une variable Color à l’aide `<meta>` de class=&quot;mktoColor&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Attributs facultatifs

* **default:** Valeur par défaut de la couleur. Code couleur hexadécimal à 6 chiffres. Ex : #ffffff.
* **mktoModuleScope**: Boolean. Contrôle si la variable est locale (true) ou globale (false) lorsqu&#39;elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${textColor}</pre>`

## Boolean {#boolean}

Si vous définissez une variable comme valeur booléenne, l’utilisateur final peut activer/désactiver l’option dans l’éditeur de courrier électronique. Vous spécifiez une variable booléenne à l’aide `<meta>` de class=&quot;mktoBoolean&quot;.

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Attributs facultatifs

* **default:** Valeur booléenne déterminant l’état par défaut du commutateur de bascule. False si omis.
* **false_value :** Valeur à insérer lorsque la bascule est en position OFF. False si omis.
* **true_value :** Valeur à insérer lorsque la bascule est en position ON. True si omis.
* **false_value_name :** IU affichée lors de la bascule lorsque l’utilisateur est en position OFF. False si omis.
* **true_value_name :** IU affichée lors de la bascule lorsqu&#39;elle est en position ON. True si omis.
* **mktoModuleScope**: Boolean. Contrôle si la variable est locale (true) ou globale (false) lorsqu&#39;elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloc HTML {#html-block}

Si vous spécifiez une variable en tant que bloc HTML, l’utilisateur final pourra saisir du texte HTML depuis l’éditeur de courrier électronique. Vous spécifiez une variable de bloc HTML à l’aide `<meta>` de class=&quot;mktoHTML&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Attributs facultatifs

* **default:** Valeur codée HTML à utiliser comme contenu par défaut du bloc.
* **mktoModuleScope**: Boolean. Contrôle si la variable est locale (true) ou globale (false) lorsqu&#39;elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variable Image {#image-variable}

Si vous définissez une variable comme Image, l’utilisateur final pourra choisir une image dans le sélecteur d’images de l’éditeur de courrier électronique. L’URL d’image sélectionnée correspond à la valeur de la variable. Vous spécifiez une variable Image à l’aide `<meta>` de class=&quot;mktoImg&quot;

Attributs requis

* **id**: Comment référencer la variable dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Attributs facultatifs

* **default:** URL d’image par défaut pour l’élément.
* **mktoModuleScope**: Boolean. Contrôle si la variable est locale (true) ou globale (false) lorsqu&#39;elle est utilisée dans un module. La valeur par défaut est False si elle est omise.

Exemple de déclaration :

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="http://www.company.com/image.jpg"></pre>`

Exemple d’utilisation :

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Modules {#modules}

Les modules sont des sections modélisées définies au niveau du modèle qui s’afficheront pour que les utilisateurs finaux puissent les insérer dans leur courrier électronique. Etant donné que vous avez préconstruit ces modules, vous pouvez vous assurer qu’ils interagiront avec le reste de votre contenu d’e-mail avec élégance (d’une manière entièrement réactive). Vous pouvez uniquement placer un module dans un conteneur.

**Pour les conteneurs de type `<table>`, `<tbody>`, `<thead>`ou `<tfoot>`:**

Spécifié à l’aide `<tr>` de class=&quot;mktoModule&quot;

**Pour les conteneurs de type `<td>`:**

Spécifié à l’aide `<table>` de class=&quot;mktoModule&quot;

Attributs requis

* **id**: Comment référencer le module dans votre modèle de courrier électronique.
* **mktoName**: Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’Editeur de messagerie 2.0. Il est recommandé d’utiliser un nom descriptif.

Attributs facultatifs

* **mktoActive :** Détermine si ce module apparaît dans la liste des modules de l’éditeur de messagerie. La valeur par défaut est true. Si la valeur est false, le module ne peut pas être ajouté par un utilisateur final à un courrier électronique.
* **mktoAddByDefault :** Détermine si ce module se trouve dans le canevas d’un nouveau courrier électronique qui utilise ce modèle lors de sa création. La valeur par défaut est true (si mktoActive a la valeur false, cette valeur est ignorée).

>[!NOTE]
>
>**Rappel**
>
>Les valeurs de classe contenant la syntaxe Marketo (c.-à-d. mktoModule, mktoContainer, mktoText) sont sensibles à la casse. Les noms d’attribut personnalisés (c.-à-d. mktoimgwidth, mktoname) ne le sont pas.

## Conteneurs {#containers}

Un conteneur contient des modules et définit leur emplacement. Lorsque les utilisateurs finaux réorganisent et insèrent des modules dans leur courrier électronique, le conteneur contrôle où ils peuvent se rendre.

**Spécifié à l’aide de `<table>`, `<tbody>`, `<thead>``<tfoot>` ou `<td>` avec class=&quot;mktoContainer&quot;**

Attributs requis

**id**: Comment référencer le module dans votre modèle de courrier électronique.

>[!CAUTION]
>
>Les conteneurs ne peuvent contenir que des modules. S&#39;il existe autre chose, le Conteneur est considéré comme non valide ! Un seul conteneur est autorisé par modèle.
