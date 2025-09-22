---
unique-page-id: 11371040
description: Syntaxe Du Modèle D’E-Mail - Documents Marketo - Documentation Du Produit
title: Syntaxe du modèle d’e-mail
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 2%

---

# Syntaxe du modèle d’e-mail {#email-template-syntax}

Dans la nouvelle expérience Marketo Email 2.0, les modèles d’e-mail sont composés de n’importe quelle combinaison d’éléments, de variables, de modules ou de conteneurs. Chaque est défini en ajoutant une syntaxe spécifique à Marketo à votre HTML. Les anciens modèles d’e-mail (v1.0) sont pris en charge dans l’éditeur d’e-mail 2.0. Cependant, ils n’incluront pas toutes les fonctionnalités du nouvel éditeur.

La syntaxe d’e-mail Marketo ne fonctionne que dans les modèles et les e-mails individuels ; elle ne fonctionne **pas** si elle est incorporée dans des fragments de code ou des jetons de texte enrichi.

>[!NOTE]
>
>La prise en charge de Marketo n’est pas configurée pour aider avec CSS/HTML. Si vous ne connaissez pas bien CSS/HTML, consultez votre développeur ou développeuse.

>[!CAUTION]
>
>Les valeurs de classe contenant la syntaxe Marketo (c’est-à-dire mktoModule, mktoContainer, mktoText) respectent la casse. Les noms d’attributs personnalisés (c’est-à-dire mktoimgwidth, mktoname) ne le sont pas.

## éléments ; {#elements}

Les éléments sont des régions de contenu que vous définissez comme modifiables dans votre modèle d’e-mail. L’expérience de modification d’un élément est propre à son type et offre un moyen simple d’utiliser le contenu. Les éléments possibles qui peuvent être inclus dans un modèle d’e-mail sont les suivants :

* Texte complet
* Images
* Extraits
* Vidéos

## Texte complet {#rich-text}

Si vous définissez une région en tant que Texte enrichi, les utilisateurs pourront modifier son contenu [à l’aide de l’éditeur de texte enrichi Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Il existe deux manières de définir un élément de texte enrichi dans un modèle d’e-mail : mktEditable et mktoText. Gardez à l’esprit qu’un élément de texte enrichi peut toujours être converti en extrait de code dans l’éditeur d’e-mail.

### Option 1 - mktEditable {#option-mkteditable}

Comme Email Editor 2.0 est rétrocompatible, certains anciens modèles d’e-mail peuvent spécifier des éléments de texte enrichi en ajoutant class=« mktEditable » sur n’importe quel élément HTML. Cela est toujours pris en charge, et l’identifiant de l’élément est ce qui sera utilisé comme nom d’affichage dans l’éditeur d’e-mail.

Attributs requis

* **class** : « mktEditable ».
* **id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.

Attributs facultatifs

* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut

Le contenu dans l’élément HTML (s’il est fourni) avec class=« mktEditable » sera utilisé comme valeur par défaut pour l’élément Rich Text.

Exemple :

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Option 2 - mktoText {#option-mktotext}

Il est recommandé de spécifier des éléments de texte enrichi à l’aide de la syntaxe class=« mktoText ». Cela permet de s’assurer qu’il existe toujours un nom d’affichage correct pour l’élément.

Attributs requis

* **class** : « mktoText »
* **id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut

Le contenu dans l’élément HTML (s’il est fourni) avec class=« mktoText » sera utilisé comme valeur par défaut pour l’élément Rich Text.

Exemple :

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Images {#images}

Vous disposez de deux options pour définir des éléments d’image modifiables. Vous pouvez utiliser une `<div>`, qui spécifie un conteneur dans lequel le `<img>` sera inséré, ou une balise `<img>`. Si vous souhaitez que l’utilisateur final sélectionne simplement une image qui renverra l’URL de l’image (par opposition au DOM), reportez-vous à « variables d’image » dans la section ci-dessous. Les deux options suivantes insèrent un élément HTML `<img>`.

### Option 1 - Utiliser un `<div>` {#option-use-a-div}

Attributs requis

* **class:** « mktoImg ».
* **id:** chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
* **mktoName :** chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoImgClass:** String. La valeur ici sera ajoutée à l’attribut class de l’élément `<img>` dans la balise div.
* **mktoImgSrc:** à utiliser comme valeur par défaut pour l’image placée dans ce div. Un espace réservé est utilisé si cet élément est omis.
* **mktoImgLink :** indiquer que la `<img>` doit être entourée d’une balise `<a>` avec cette URL de destination. L’utilisateur peut modifier ce paramètre dans l’éditeur d’e-mail.
* **mktoImgLinkTarget :** indiquez que la balise `<a>` de l’attribut mktoImgLink doit utiliser cette cible. N’a aucun effet si mktoImgLink n’est pas également utilisé.
* **mktoImgWidth :** utilisé comme largeur sur le `<img>` entre crochets.
* **mktoImgHeight :** utilisé comme hauteur sur le `<img>` entre crochets.
* **mktoLockImgSize :** permet de déverrouiller les propriétés height et width de l&#39;élément `<img>` afin que l&#39;utilisateur final puisse les modifier (la valeur par défaut est true si cet élément est omis).
* **mktoLockImgStyle :** utilisé pour verrouiller la propriété style de l’élément `<img>` (la valeur par défaut est false).

Valeur par défaut (facultatif)

**`<img>`** : à utiliser comme élément de `<img>` dans lequel l’image sera placée. Utile pour ajouter un style intégré à l’image. N’oubliez pas d’inclure les balises `<a> </a>` environnantes. Ainsi, si l’utilisateur ajoute un lien, votre style ne sera pas supprimé.

Exemple :

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### Option 2 - Utiliser un \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Cette option ne permet pas aux utilisateurs finaux d’ajouter un lien à leur image. Utilisez l’option 1 si cela est important pour votre modèle.

Attributs requis

* **class:** « mktoImg ».
* **id:** chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
* **mktoName:** String. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.  Valeur par défaut (facultatif)
* **src:** À utiliser comme valeur par défaut pour l’image. Un espace réservé est utilisé si cet élément est omis.
* **mktoLockImgSize :** permet de déverrouiller les propriétés height et width de l&#39;élément `<img>` afin que l&#39;utilisateur final puisse les modifier (la valeur par défaut est true si cet élément est omis).
* **mktoLockImgStyle :** utilisé pour verrouiller la propriété style de l’élément `<img>` (la valeur par défaut est false).

Exemple :
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Extraits {#snippets}

Si vous définissez une région en tant que fragment de code, les utilisateurs finaux pourront choisir le fragment de code approuvé [Fragment de code](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md) qu’ils souhaitent insérer dans cette région. Bien que les éléments de texte enrichi puissent être convertis en fragments de code dans l’éditeur d’e-mail, lorsque vous définissez une région spécifiquement comme fragment de code, elle ne peut pas être convertie en texte enrichi. Vous pouvez spécifier une région de fragment de code à l’aide d’un `<div>` avec class=« mktoSnippet »

Attributs requis

* **id:** chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
* **mktoName:** String. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Valeur par défaut (facultatif)

**mktoDefaultSnippetId** : identifiant numérique du fragment de code Marketo qui doit apparaître par défaut (ne fonctionne que si un fragment de code avec cet identifiant existe et est approuvé dans cet espace de travail).

Exemple :

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Vidéo {#video}

Si vous définissez une région comme une vidéo, les utilisateurs finaux pourront insérer une URL YouTube ou Vimeo qui s’affichera sous la forme d’une miniature (avec le bouton « Lire ») dans l’e-mail. Vous pouvez spécifier une région Vidéo à l’aide d’un `<div>` avec class=« mktoVideo »

Attributs requis

* **id:** chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
* **mktoName:** String. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoImgClass:** String. La valeur ici sera ajoutée à l’attribut class de la miniature vidéo `<img>` dans la balise div.

Exemple :

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variables {#variables}

Les variables sont comme des jetons. Définissez-les d’abord dans la section `<head>` de votre modèle d’e-mail à l’aide de balises `<meta>`, puis utilisez-les autant de fois que vous le souhaitez dans l’ensemble du modèle. Comme elles sont définies dans le modèle, l’utilisateur final peut modifier ses valeurs en fonction de ses règles. Notez que vous pouvez définir une variable comme locale ou globale dans la portée. Si vous utilisez une variable dans un « module » (voir ci-dessous) et qu’un utilisateur final duplique ce module, les variables locales auront des valeurs indépendantes, tandis que les variables globales s’appliqueront aux deux modules.

## Chaîne {#string}

Si vous spécifiez une variable sous la forme d’une chaîne, l’utilisateur final peut saisir du texte dans une zone de texte dans l’éditeur d’e-mail. Vous spécifiez une variable de chaîne à l’aide de `<meta>` avec class=« mktoString »

Attributs requis

* **id :** comment référencer la variable dans votre modèle d’e-mail.
* **mktoName:** String. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **allowHTML:** Boolean. Contrôle si la valeur de la variable fait l’objet d’un échappement HTML. La valeur par défaut est False si cet attribut est omis.
* **default** : valeur par défaut de la chaîne. Vide si omis.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si cet attribut est omis.

Exemple de déclaration :

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Exemple d’utilisation :

`${textHeader}`

## Liste {#list}

Si vous spécifiez une variable sous forme de liste, l’utilisateur final peut effectuer un choix parmi un ensemble de valeurs que vous définissez dans l’éditeur d’e-mail. Pour spécifier une variable de liste, utilisez `<meta>` avec class=« mktoList »

Attributs requis

* **id** : comment référencer la variable dans votre modèle d’e-mail.
* **mktoName:** String. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.
* **values:** liste de valeurs séparées par des virgules. Doit avoir au moins une chaîne.

Attributs facultatifs

* **default:** valeur par défaut de la liste déroulante de sélection. En cas d’omission, la première valeur de l’attribut « values » est utilisée.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si cet attribut est omis.

Exemple de déclaration :

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Exemple d’utilisation :

`${textFontFamily}`

## Nombre {#number}

Si vous spécifiez une variable sous la forme d’un nombre, l’utilisateur final pourra saisir un nombre dans l’éditeur d’e-mail. Vous spécifiez une variable Number à l’aide de `<meta>` avec class=« mktoNumber »

Attributs requis

* **id** : comment référencer la variable dans votre modèle d’e-mail.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.
* **default:** Valeur numérique par défaut pour la variable.

Attributs facultatifs

* **min:** Valeur acceptée min.
* **max:** Valeur acceptée max.
* **units :** unités à ajouter à la valeur numérique (px, pt, em, etc.) lorsqu’elles sont affichées dans l’éditeur d’e-mail, ainsi que dans le code qui en résulte.
* **étape :** nombre d’unités que la variable number doit augmenter/diminuer de (0,1, 1, 10, etc.). Si cet attribut est omis, la valeur par défaut est 1.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si cet attribut est omis.

Exemple de déclaration :

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1">`

Exemple d’utilisation :

`${textFontSize}`

## Couleur {#color}

Si vous spécifiez une variable en tant que Couleur, l’utilisateur final peut saisir une valeur de couleur hexadécimale ou choisir une couleur à partir du sélecteur de couleurs dans l’éditeur d’e-mail. Vous spécifiez une variable Color à l’aide de `<meta>` avec class=« mktoColor »

Attributs requis

* **id** : comment référencer la variable dans votre modèle d’e-mail.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default:** valeur par défaut de la couleur. Code couleur hexadécimal à 6 chiffres. Ex : #ffffff.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si cet attribut est omis.

Exemple de déclaration :

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Exemple d’utilisation :

`${textColor}`

## Booléen {#boolean}

Si vous spécifiez une variable sous la forme d’un booléen, l’utilisateur final peut activer/désactiver l’option dans l’éditeur d’e-mail. Pour spécifier une variable booléenne, utilisez `<meta>` avec class=« mktoBoolean »

Attributs requis

* **id** : comment référencer la variable dans votre modèle d’e-mail.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default:** valeur booléenne déterminant l&#39;état par défaut du commutateur (bascule). False si omis.
* **false_value:** Valeur à insérer lorsque le bouton (bascule) est en position OFF. False si omis.
* **true_value:** valeur à insérer lorsque le bouton (bascule) est en position ON. Vrai si omis.
* **false_value_name :** interface utilisateur affichée dans le bouton bascule en position OFF. False si omis.
* **true_value_name :** interface utilisateur affichée dans le bouton bascule en position ON. Vrai si omis.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si cet attribut est omis.

Exemple de déclaration :

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Exemple d’utilisation :

`${showFooter}`

## Bloc HTML {#html-block}

Si vous spécifiez une variable comme bloc HTML, l’utilisateur final pourra saisir mot pour mot HTML à partir de l’éditeur d’e-mail. Vous spécifiez une variable de bloc HTML à l’aide de `<meta>` avec class=« mktoHTML »

Attributs requis

* **id** : comment référencer la variable dans votre modèle d’e-mail.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default:** valeur codée par HTML pour servir de contenu par défaut du bloc.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si cet attribut est omis.

Exemple de déclaration :

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Exemple d’utilisation :

`${trackingPixel}`

## Variable d’image {#image-variable}

Si vous spécifiez une variable sous la forme d’une image, l’utilisateur final peut choisir une image dans le sélecteur d’images de l’éditeur d’e-mail. L’URL de l’image sélectionnée est la valeur de la variable . Vous spécifiez une variable Image à l’aide de `<meta>` avec class=« mktoImg »

Attributs requis

* **id** : comment référencer la variable dans votre modèle d’e-mail.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **default:** URL d&#39;image par défaut pour l&#39;élément.
* **mktoModuleScope** : booléen. Contrôle si la variable est locale (true) ou globale (false) lorsqu’elle est utilisée dans un module. La valeur par défaut est False si cet attribut est omis.

Exemple de déclaration :

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Exemple d’utilisation :

`${heroBackgroundImage}`

## Modules {#modules}

Les modules sont des sections modélisées définies au niveau du modèle qui s’afficheront pour que les utilisateurs finaux les insèrent dans leur e-mail. Comme vous avez préconfiguré ces modules, vous pouvez vous assurer qu’ils interagiront avec le reste du contenu de votre e-mail de manière élégante (et entièrement réactive). Vous pouvez uniquement placer un module dans un conteneur.

>[!IMPORTANT]
>
>Lorsqu’un e-mail est généré à partir d’un modèle d’e-mail qui contient des composants de module définis, toutes les modifications apportées aux modules du modèle ne sont **pas** transmises audit e-mail.

**Pour les conteneurs de type `<table>`, `<tbody>`, `<thead>` ou `<tfoot>`:**

Spécifié à l’aide de `<tr>` avec class=« mktoModule »

**Pour les conteneurs de type `<td>`:**

Spécifié à l’aide de `<table>` avec class=« mktoModule »

Attributs requis

* **id** : comment référencer le module dans votre modèle d’e-mail.
* **mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur d’e-mail 2.0. Il est recommandé d’utiliser un nom explicite.

Attributs facultatifs

* **mktoActive:** détermine si ce module apparaît dans la liste des modules de l’éditeur d’e-mail. La valeur par défaut est « true ». Si la valeur est false, le module ne peut pas être ajouté par un utilisateur final à un email.
* **mktoAddByDefault:** détermine si ce module sera dans la zone de travail d’un nouvel e-mail qui utilise ce modèle lors de sa création. La valeur par défaut est true (si mktoActive est false, cette valeur est ignorée).

>[!NOTE]
>
>Les valeurs de classe contenant la syntaxe Marketo (c’est-à-dire mktoModule, mktoContainer, mktoText) respectent la casse. Les noms d’attributs personnalisés (c’est-à-dire mktoimgwidth, mktoname) ne le sont pas.

## Conteneurs {#containers}

Un conteneur contient des modules et définit leur emplacement. Lorsque les utilisateurs finaux réorganisent et insèrent des modules dans leur e-mail, le conteneur détermine où ils peuvent aller.

**Spécifié en utilisant `<table>`, `<tbody>`, `<thead>`, `<tfoot>` ou `<td>` avec class=« mktoContainer »**

Attributs requis

**id** : comment référencer le module dans votre modèle d’e-mail.

>[!CAUTION]
>
>Les conteneurs ne peuvent contenir que des modules. S’il existe d’autres éléments, le conteneur est considéré comme non valide. Un seul conteneur est autorisé par modèle.
