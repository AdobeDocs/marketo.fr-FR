---
unique-page-id: 7515401
description: Création d’un modèle de page de destination guidé - Documents Marketo - Documentation du produit
title: Créer un modèle de page de destination guidée
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 29c1b59c9d2598626f546554a8bdc1b26b9e1590
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 2%

---

# Créer un modèle de page de destination guidée {#create-a-guided-landing-page-template}

Les modèles de landing page guidés ont une syntaxe spéciale. Utilisez cette syntaxe pour spécifier ce qui est personnalisable et où le contenu se retrouvera sur chaque page de destination créée à partir de votre modèle. Seules les régions ou variables que vous spécifiez comme modifiables seront disponibles pour personnalisation dans l’éditeur de page de destination « Guidée ».

>[!TIP]
>
>Respectez les bonnes conventions de nommage et votre équipe marketing tombera amoureuse de vous.

Il existe deux manières de déclarer qu’un élément de votre page doit être modifiable :

* Déclarez un objet en tant qu’« élément ». Le créateur de la page de destination pourra ajouter des images, du texte ou des ressources Marketo dans ces régions spécifiées.
* Déclarez une chaîne en tant que « variable ». Le créateur de la page de destination pourra remplacer cette variable par une chaîne, une couleur ou un état booléen à partir d’un levier vrai/faux.

## Éléments modifiables {#editable-elements}

Les éléments sont déclarés en ajoutant un élément DOM normal au modèle, puis en ajoutant un nom de classe spécifique à Marketo à l’élément.

## Texte {#text}

Si vous définissez une région en tant que Texte enrichi, les utilisateurs pourront modifier son contenu [à l’aide de l’éditeur de texte enrichi Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Attributs requis :
**class** : « mktoText »
**id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
**mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Facultatif :
Le contenu d’un élément avec la classe mktoText (s’il est fourni) sera utilisé comme valeur par défaut pour la région modifiable.

Exemple :

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Image {#image}

Vous disposez de deux options pour définir des éléments d’image modifiables. Vous pouvez utiliser une `<div>`, qui spécifie un conteneur dans lequel l’image sera insérée, ou une balise `<img>`.

## Option 1 - Utiliser un `<div>` {#option-use-a-div}

Attributs requis :

classe : « mktoImg »
id : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
mktoName : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Facultatif :
mktoImgClass : chaîne. La valeur ici sera ajoutée à l’attribut class de l’élément `<img>` dans la balise div.

Exemple :

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Option 2 - Utiliser un `<img>` {#option-use-a-img}

Attributs requis :
classe : « mktoImg »
id : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
mktoName : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Facultatif :
src : URL de chaîne. Elle sera utilisée comme valeur par défaut pour l’image.

Exemple :

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Lors de l’utilisation de la version `<img>`, l’HTML rendue contiendra un wrapper div généré autour de la balise `<img>`. Il sera défini sur « classe ».mktoImg.mktoGen », et sera affiché:inline-block.

## Form {#form}

Exemple :Required attributs :
**class** : « mktoForm »
**id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
**mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Extrait {#snippet}

Attributs requis :
**class** : « mktoSnippet »
**id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
**mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Bouton de partage {#share-button}

Attributs requis :
**class** : « mktoShareButton »
**id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
**mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Vidéo {#video}

>[!NOTE]
>
>Lors de l’utilisation de l’élément vidéo dans une page de destination, Marketo ne prend en charge que les vidéos provenant de YouTube. Si vous utilisez un autre service, nous vous recommandons d’utiliser une zone de texte enrichi et de coller le code intégré de la vidéo.

Attributs requis :
**class** : « mktoVideo »
**id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
**mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Variables modifiables {#editable-variables}

Tous les types de variables sont utilisés en référençant la valeur de leur attribut d’identifiant encapsulé dans une séquence de caractères ${ }. Ils peuvent être utilisés n’importe où dans le document, à l’exception de ceux contenus dans d’autres déclarations de variables.

Exemple :

`${var1}`

**Déclaration:**

Les variables sont déclarées en tant que balises meta dans l’élément `<head>` du modèle. Trois types de variables sont disponibles : chaîne, couleur et valeur booléenne.

## Chaîne {#string}

Attributs requis :
**class** : « mktoString »,
**id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
**mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Facultatif :
**default** : valeur de chaîne pour l&#39;attribut. Vide si aucun n’est fourni.
**allowHtml** : « true » ou « false ». Contrôle si la valeur sera imprimée sans être placée dans une séquence d’échappement HTML. La valeur par défaut est « false » si elle n’est pas définie.

Exemple de base :

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Exemple avec tous les attributs :

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Couleur {#color}

Attributs requis :
**class** : « mktoColor »,
**id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
**mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Facultatif :
**default** : code couleur à 7 chiffres pour les caractères HEX. Par Ex. : « #336699 »

Exemple de base :

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Exemple avec tous les attributs :

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Booléen {#boolean}

Attributs requis :
**class** : « mktoBoolean »,
**id** : chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret « - » et un trait de soulignement « _ ». Aucun espace n’est autorisé. Doit être unique.
**mktoName** : chaîne. Il s’agit du nom d’affichage qui s’affiche dans l’éditeur de page de destination. Il est recommandé d’utiliser un nom explicite.

Facultatif :
**default** : chaîne booléenne. « true » ou « false » contrôle si la valeur commence à la position ON ou OFF. « false » s’il n’est pas fourni.
**false_value** : chaîne. Valeur à insérer pour la variable lorsqu’elle est en position OFF. « false » s’il n’est pas fourni.
**true_value** : chaîne. Valeur à insérer pour la variable lorsqu’elle est en position ON. « true » si non fourni.
**false_value_name** : chaîne. Nom d’affichage à afficher dans l’éditeur de page de destination lorsque la valeur est en position OFF. « OFF » s’il n’est pas fourni.
**true_value_name** : chaîne. Nom d’affichage à afficher dans l’éditeur de page de destination lorsque la valeur est en position ON. « ON » s’il n’est pas fourni.

Exemple de base :

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Exemple avec tous les attributs :

Cet exemple illustre un cas d’utilisation courant où une variable booléenne contrôle la visibilité d’un élément css en définissant la valeur de la propriété d’affichage css sur « block » ou « none » pour afficher/masquer un élément par identifiant avec CSS. L’éditeur de page de destination utilise le nom d’affichage Afficher/Masquer au lieu de Désactiver/Activer.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Les jetons de programme (my.token) peuvent également être utilisés n’importe où dans les pages de destination guidées ou à structure libre.
