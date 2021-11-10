---
unique-page-id: 7515401
description: Création d’un modèle de page d’entrée guidée - Documents Marketo - Documentation du produit
title: Création d’un modèle de page d’entrée guidée
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
source-git-commit: c309b69198c6f61d7475c6d3a6b1672e045b9b4a
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 2%

---

# Création d’un modèle de page d’entrée guidée {#create-a-guided-landing-page-template}

Les modèles de landing page guidés ont une syntaxe spéciale. Utilisez cette syntaxe pour spécifier ce qui est personnalisable et où le contenu finira sur chaque landing page créée à partir de votre modèle. Seules les régions ou variables que vous spécifiez comme modifiables pourront être personnalisées dans l’éditeur de page d’entrée &quot;guidée&quot;.

>[!TIP]
>
>Utilisez de bonnes conventions d’attribution de noms et votre équipe marketing vous aimera.

Il existe deux manières de déclarer qu’un élément de votre page doit être modifiable :

* Déclarez un objet comme &quot;élément&quot;. Le créateur de la landing page pourra ajouter des images, du texte ou des ressources Marketo dans ces régions spécifiées.
* Déclarez une chaîne comme &quot;variable&quot;. Le créateur de la page d’entrée pourra remplacer cette variable par un état de chaîne, de couleur ou de booléen à partir d’un levier vrai/faux.

## Éléments modifiables {#editable-elements}

Les éléments sont déclarés en ajoutant un élément DOM normal au modèle, puis en décorant l’élément avec un nom de classe spécifique à Marketo.

## Texte {#text}

Si vous définissez une région comme Texte enrichi, les utilisateurs pourront modifier son contenu. [Utilisation de l’éditeur de texte enrichi Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Attributs requis :\
**class**: &quot;mktoText&quot;\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

En option:\
Le contenu d’un élément avec la classe mktoText (s’il est fourni) sera utilisé comme valeur par défaut pour la région modifiable.

Exemple :

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div></pre>`

## Image {#image}

Vous disposez de deux options pour définir les éléments d’image modifiables. Vous pouvez utiliser une `<div>`, qui spécifie un conteneur dans lequel l’image sera insérée, ou un `<img>` balise .

## Option 1 - Utilisez une `<div>` {#option-use-a-div}

Attributs requis :

Classe : &quot;mktoImg&quot;\
id: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
mktoName : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

En option:\
mktoImgClass: Chaîne. La valeur ici sera ajoutée à l’attribut de classe de la propriété `<img>` élément dans la balise div.

Exemple :

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Option 2 - Utilisez une `<img>` {#option-use-a-img}

Attributs requis :\
Classe : &quot;mktoImg&quot;\
id: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
mktoName : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

En option:\
src : URL de chaîne. Cette valeur sera utilisée comme valeur par défaut de l’image.

Exemple :

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>Lors de l’utilisation de la variable `<img>` version, le HTML rendu contient un wrapper div généré autour de la balise `<img>` balise . Il sera défini sur class .&quot;mktoImg.mktoGen&quot; et sera display:inline-block.

## Formulaire {#form}

Exemple : attributs obligatoires :\
**class**: &quot;mktoForm&quot;\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Extrait {#snippet}

Attributs requis :\
**class**: &quot;mktoSnippet&quot;\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Bouton de partage {#share-button}

Attributs requis :\
**class**: &quot;mktoShareButton&quot;\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Vidéo {#video}

>[!NOTE]
>
>Lors de l’utilisation de l’élément vidéo dans une landing page, Marketo ne prend en charge que les vidéos issues de YouTube. Si vous utilisez un autre service, nous vous recommandons d’utiliser une zone de texte enrichi et de coller dans le code intégré de la vidéo.

Attributs requis :
**class**: &quot;mktoVideo&quot;
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Sondage {#poll}

Attributs requis :\
**class**: &quot;mktoPoll&quot;\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Référencement {#referral}

Attributs requis :\
**class**: &quot;mktoReferral&quot;\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Loteries {#sweepstakes}

Attributs requis :\
**class**: &quot;mktoSweepstakes&quot;\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

Exemple :

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Variables modifiables {#editable-variables}

Tous les types de variable sont utilisés en référençant la valeur de leur attribut id encapsulé dans une séquence de caractères ${ }. Ils peuvent être utilisés n’importe où dans le document, sauf dans d’autres déclarations de variable.

Exemple :

`<pre data-theme="Confluence">${var1}</pre>`

**Déclaration :**

Les variables sont déclarées en tant que balises META dans la variable `<head>` du modèle. Trois types de variables sont disponibles : Chaîne, Couleur et Valeur booléenne.

## Chaîne {#string}

Attributs requis :\
**class** : &quot;mktoString&quot;,\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

En option:\
**default**: Valeur de chaîne pour l’attribut . Vide si aucun n’est fourni.\
**allowHtml**: &quot;true&quot; ou &quot;false&quot;. Contrôle si la valeur est imprimée sans séquence d’échappement par HTML. La valeur par défaut est &quot;false&quot; si elle n’est pas définie.

Exemple de base :

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Exemple avec tous les attributs :

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Couleur {#color}

Attributs requis :\
**class** : &quot;mktoColor&quot;,\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

En option:\
**default**: Code couleur de caractère HEX à 7 chiffres. Par exemple : &quot;#336699&quot;

Exemple de base :

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Exemple avec tous les attributs :

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Booléenne {#boolean}

Attributs requis :\
**class** : &quot;mktoBoolean&quot;,\
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Les espaces ne sont pas autorisés. Doit être unique.\
**mktoName** : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom explicite.

En option:\
**default**: Chaîne booléenne. &quot;true&quot; ou &quot;false&quot; contrôle si la valeur commence à la position ON ou OFF. &quot;false&quot; s’il n’est pas fourni.\
**false_value**: Chaîne. La valeur à insérer pour la variable lorsqu’elle est en position OFF. &quot;false&quot; s’il n’est pas fourni.\
**true_value**: Chaîne. La valeur à insérer pour la variable lorsqu’elle est en position ON. &quot;true&quot; s’il n’est pas fourni.\
**false_value_name**: Chaîne. Nom d’affichage à afficher dans l’éditeur de landing page lorsque la valeur est en position OFF. &quot;OFF&quot; s’il n’est pas fourni.\
**true_value_name**: Chaîne. Nom d’affichage à afficher dans l’éditeur de landing page lorsque la valeur est en position ON. &quot;ON&quot; s’il n’est pas fourni.

Exemple de base :

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Exemple avec tous les attributs :

Cet exemple illustre un cas d’utilisation courant où une variable booléenne contrôle la visibilité d’un élément CSS en définissant la valeur de la propriété d’affichage CSS sur &quot;block&quot; ou &quot;none&quot; pour afficher/masquer un élément par identifiant avec CSS. L’éditeur de page d’entrée utilise le nom d’affichage Afficher/Masquer au lieu de OFF/ON.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>Les jetons de programme (my.token) peuvent également être utilisés n’importe où dans les pages d’entrée de forme libre ou guidée.
