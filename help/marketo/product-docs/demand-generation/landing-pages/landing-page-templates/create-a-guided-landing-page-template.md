---
unique-page-id: 7515401
description: Création d’un modèle de Landing page guidé - Documents marketing - Documentation du produit
title: Création d’un modèle de Landing page guidé
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# Créer un modèle de Landing page guidé {#create-a-guided-landing-page-template}

>[!NOTE]
>
>Fatigué de la lecture ? [Regardez cette ](https://youtu.be/3O7e4GdZKsM) vidéo sympa avec des instructions détaillées.

Les modèles de landing page guidé ont une syntaxe spéciale. Utilisez cette syntaxe pour spécifier ce qui est personnalisable et où le contenu finira sur chaque landing page généré à partir de votre modèle. Seules les régions ou variables que vous spécifiez comme modifiables seront disponibles pour la personnalisation dans l’éditeur de landing page &quot;Guided&quot;.

>[!TIP]
>
>Utilisez de bonnes conventions d&#39;attribution de noms et votre équipe marketing vous séduira.

Il existe deux façons de déclarer qu’un élément de votre page doit être modifiable :

* Déclarez un objet comme &quot;élément&quot;. Le créateur de landing page pourra ajouter des images, du texte ou des ressources marketing dans ces régions spécifiées.
* Déclarez une chaîne en tant que &quot;variable&quot;. Le créateur de landing page pourra remplacer cette variable par une chaîne, une couleur ou un état booléen à partir d’un levier vrai/faux.

## Éléments modifiables {#editable-elements}

Les éléments sont déclarés en ajoutant un élément DOM normal au modèle, puis en décorant l’élément avec un nom de classe spécifique au marketing.

## Texte {#text}

Si vous définissez une région sous la forme de texte enrichi, les utilisateurs peuvent modifier son contenu [à l’aide de l’éditeur de texte enrichi de Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Attributs requis :\
**classe** : &quot;mktoText&quot;\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Facultatif :\
Le contenu d’un élément avec la classe mktoText (s’il est fourni) sera utilisé comme valeur par défaut pour la région modifiable.

Exemple :

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div></pre>`

### Image {#image}

Vous disposez de deux options pour définir des éléments d’image modifiables. Vous pouvez utiliser soit une balise `<div>`, qui spécifie un conteneur dans lequel l&#39;image sera insérée, soit une balise `<img>`.

## Option 1 - Utiliser un `<div>` {#option-use-a-div}

Attributs requis :

class : &quot;mktoImg&quot;\
id: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
mktoName : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Facultatif :\
mktoImgClass: Chaîne. La valeur ici sera ajoutée à l&#39;attribut de classe de l&#39;élément `<img>` dans la balise div.

Exemple :

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Option 2 - Utiliser un `<img>` {#option-use-a-img}

Attributs requis :\
class : &quot;mktoImg&quot;\
id: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
mktoName : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Facultatif :\
src : URL de chaîne. Elle sera utilisée comme valeur par défaut pour l’image.

Exemple :

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>Lors de l’utilisation de la version `<img>`, le code HTML rendu contient un wrapper div généré autour de la balise `<img>`. Il sera défini sur class.&quot;mktoImg.mktoGen&quot; et sera display:inline-block.

## Formulaire {#form}

Exemple : attributs obligatoires :\
**classe** : &quot;mktoForm&quot;\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Extrait {#snippet}

Attributs requis :\
**classe** : &quot;mktoSnippet&quot;\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Exemple :

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Bouton Partager {#share-button}

Attributs requis :\
**classe** : &quot;mktoShareButton&quot;\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Exemple :

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Vidéo {#video}

>[!NOTE]
>
>Lors de l’utilisation de l’élément vidéo dans un landing page, Marketo ne prend en charge que les vidéos de YouTube. Si vous utilisez un autre service, nous vous recommandons d’utiliser une zone de texte enrichi et de coller le code intégré de la vidéo.

Attributs requis :
**class**: &quot;mktoVideo&quot;
**id**: Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Exemple :

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Sondage {#poll}

Attributs requis :\
**classe** : &quot;mktoPoll&quot;\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Exemple :

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Référent {#referral}

Attributs requis :\
**classe** : &quot;mktoReferral&quot;\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Exemple :

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Tirage {#sweepstakes}

Attributs requis :\
**classe** : &quot;mktoSweepstakes&quot;\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Exemple :

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Variables modifiables {#editable-variables}

Tous les types de variable sont utilisés en référençant la valeur de leur attribut id encapsulé dans une séquence de caractères ${ }. Ils peuvent être utilisés n’importe où dans le document, sauf dans d’autres déclarations de variable.

Exemple :

`<pre data-theme="Confluence">${var1}</pre>`

**Déclaration :**

Les variables sont déclarées en tant que balises meta dans l’élément `<head>` du modèle. Trois types de variables sont disponibles pour l’utilisation : Chaîne, Couleur et Valeur booléenne.

## Chaîne {#string}

Attributs requis :\
**classe**  : &quot;mktoString&quot;,\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Facultatif :\
**par défaut** : Valeur de chaîne pour l’attribut. Vide si aucun n&#39;a été fourni.\
**allowHtml** : &quot;true&quot; ou &quot;false&quot;. Contrôle si la valeur doit être imprimée sans avoir d’échappement HTML. La valeur par défaut est &quot;false&quot; si elle est désactivée.

Exemple de base :

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Exemple avec tous les attributs :

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Couleur {#color}

Attributs requis :\
**classe**  : &quot;mktoColor&quot;,\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Facultatif :\
**par défaut** : Code couleur de caractère HEX à 7 chiffres. Par exemple : &quot;#336699&quot;

Exemple de base :

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Exemple avec tous les attributs :

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Booléen {#boolean}

Attributs requis :\
**classe**  : &quot;mktoBoolean&quot;,\
**id** : Chaîne d’ID. Contient uniquement des lettres, des chiffres, un tiret &quot;-&quot; et un trait de soulignement &quot;_&quot;. Aucun espace autorisé. Doit être unique.\
**mktoName**  : Chaîne. Il s’agit du nom d’affichage qui s’affichera dans l’éditeur de landing page. Il est recommandé d’utiliser un nom descriptif.

Facultatif :\
**par défaut** : Chaîne booléenne. &quot;true&quot; ou &quot;false&quot; contrôlent si la valeur se début en position Activé ou Désactivé. &quot;false&quot; si non fourni.\
**false_value** : Chaîne. Valeur à insérer pour la variable lorsqu’elle est en position OFF. &quot;false&quot; si non fourni.\
**true_value** : Chaîne. Valeur à insérer pour la variable lorsqu’elle se trouve en position ON. &quot;true&quot; si non fourni.\
**false_value_name** : Chaîne. Nom d’affichage à afficher dans l’éditeur de landings page lorsque la valeur est en position OFF. &quot;OFF&quot; s’il n’est pas fourni.\
**true_value_name** : Chaîne. Nom d’affichage à afficher dans l’éditeur de landings page lorsque la valeur est en position ON. &quot;ON&quot; s’il n’est pas fourni.

Exemple de base :

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Exemple avec tous les attributs :

Cet exemple montre un cas d&#39;utilisation courant où une variable booléenne contrôle la visibilité d&#39;un élément css en définissant la valeur de la propriété d&#39;affichage css sur &quot;block&quot; ou &quot;none&quot; pour afficher/masquer un élément par id avec CSS. L’éditeur de landing page utilise le nom d’affichage Afficher/Masquer plutôt que Désactivé/Activé.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>Les jetons de programme (my.token) peuvent également être utilisés n’importe où dans les landings page de forme libre ou guidé.
