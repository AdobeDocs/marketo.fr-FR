---
solution: Marketo Engage
product: marketo
title: Fragments personnalisables
description: Découvrez comment personnaliser des fragments en rendant certains champs modifiables. Créer des fragments réutilisables flexibles dans le Designer d’e-mail.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
TQID: https://experienceleague.adobe.com/SCmyn9QUECmvQgVltKknlvLuvL15Tz3LYorBFYB1hqI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: fdc003d7aed05d85687427d9455bb806eb33d0b2
workflow-type: tm+mt
source-wordcount: 1403
ht-degree: 12%

---

# Fragments personnalisables {#customizable-fragments}

Lorsque des fragments sont utilisés dans un e-mail ou un modèle d’e-mail, ils sont verrouillés par défaut en raison de l’héritage, ce qui signifie que toutes les modifications apportées à un fragment sont automatiquement propagées à toutes les ressources où il est utilisé. Grâce aux fragments personnalisables, les champs spécifiques d’un fragment peuvent être définis comme modifiables lorsque le fragment est ajouté à un e-mail ou à un modèle d’e-mail. Par exemple, si vous disposez d’un fragment avec une bannière, du texte et un bouton, vous pouvez désigner certains champs, tels que l’image ou l’URL cible du bouton, comme modifiables.

Les fragments personnalisables vous permettent de gérer et de personnaliser le contenu sans créer de blocs de contenu entièrement nouveaux ou interrompre l’héritage des fragments. Les modifications apportées au niveau du fragment sont toujours propagées, tout en permettant la personnalisation au niveau de l’e-mail ou du modèle d’e-mail.

Les fragments visuels et d’expression peuvent être marqués comme personnalisables.

## Ajouter des champs modifiables dans des fragments visuels {#visual}

Pour rendre des parties d’un fragment visuel modifiables, procédez comme suit :

>[!NOTE]
>
>Des champs modifiables peuvent être ajoutés aux composants **image**, **texte** et **bouton**. Pour les composants **HTML**, les champs modifiables sont ajoutés à l’aide de l’éditeur de personnalisation, comme pour les fragments d’expression. [En savoir plus sur les champs modifiables dans les composants HTML des fragments](#editable-html)

1. Ouvrez l’écran d’édition du contenu du fragment.

1. Sélectionnez le composant de votre fragment dans lequel vous souhaitez configurer des champs modifiables.

1. Le volet des propriétés du composant s’ouvre sur le côté droit. Sélectionnez l’onglet **[!UICONTROL Champs modifiables]**, puis activez l’option **[!UICONTROL Activer l’édition]**.

1. Tous les champs pouvant être modifiés pour le composant sélectionné sont répertoriés dans le volet. Les champs disponibles pour la modification dépendent du type de composant sélectionné.

   Dans l’exemple ci-dessous, l’URL du bouton « Cliquez ici » est configurée comme étant modifiable.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Cliquez sur **[!UICONTROL Aperçu]** pour vérifier tous les champs modifiables et leurs valeurs par défaut.

   Dans cet exemple, le champ URL du bouton s’affiche avec la valeur par défaut définie dans le composant. Les utilisateurs peuvent personnaliser cette valeur après avoir ajouté le fragment à leur contenu.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Enregistrez vos modifications lorsque vous avez terminé.

Après avoir ajouté le fragment à un e-mail, les utilisateurs et utilisatrices peuvent personnaliser tous les champs modifiables configurés dans le fragment.

## Composants HTML modifiables dans les fragments {#editable-html}

Dans un composant HTML, les types d’éléments suivants peuvent être rendus modifiables :

* Une partie du **contenu texte** (par exemple, un titre ou un libellé CTA).
* Une **URL** complète, utilisée comme cible du lien ou source de l’image. Les URL partielles ne sont pas prises en charge ; la variable doit représenter la valeur URL entière.
* Valeur **propriété CSS** complète (par exemple, une valeur de couleur, une valeur de remplissage complète ou une valeur de largeur totale). Les valeurs de propriété CSS partielles ne sont pas prises en charge.

Chaque valeur de propriété CSS paramétrée doit être exactement `{{{varName}}}` : aucun suffixe, aucun texte supplémentaire, aucune variable multiple et aucune concaténation dans une seule propriété.

Pour paramétrer des propriétés multifaces telles que la marge intérieure, procédez de l’une des manières suivantes :

* déclarer chaque côté comme propriété distincte _(recommandé)_ ou
* déclarez une variable unique contenant la valeur complète de la forme abrégée.

## Fonctionnement des champs modifiables dans les composants HTML {#components}

Les champs modifiables d’un composant HTML sont créés en déclarant des variables intégrées directement dans le code source du composant. Chaque variable possède un identifiant unique et une valeur par défaut. La variable est ensuite référencée là où la valeur modifiable doit apparaître dans le balisage.

Une fois le fragment enregistré et publié, chaque variable déclarée dans le composant HTML est automatiquement surfacée en tant que paramètre modifiable lorsque le fragment est ajouté à un email.

L’auteur d’e-mail peut alors remplacer la valeur par défaut de toute variable du Designer d’e-mail (par exemple, modifier une couleur d’arrière-plan, échanger une URL de CTA ou mettre à jour un titre) sans modifier l’HTML sous-jacent.

## Référence de syntaxe {#syntax}

Les champs modifiables sont définis et référencés à l’aide de deux modèles :

### Déclaration d’une variable {#declaring}

Utilisez la déclaration en ligne pour définir une variable avec un ID unique et une valeur par défaut :

```handlebars
{{#inline "variableID"}}default_value{{/inline}}
```

Remplacez `variableID` par un identifiant unique pour le champ modifiable. L’identifiant doit être unique dans le composant et ne doit pas contenir d’espaces.

Remplacez `default_value` par la valeur à utiliser si l’auteur de l’e-mail ne la remplace pas.

### Référencer une variable {#referencing}

Utilisez des accolades triples pour référencer la variable à l’endroit où sa valeur doit apparaître dans le balisage :

```handlebars
{{{variableID}}}
```

Le même ID de variable peut être référencé un certain nombre de fois dans l’HTML. Toutes les références sont résolues sur la valeur définie par l’auteur de l’e-mail (ou sur la valeur par défaut si aucun remplacement n’est fourni).

### Paramètres facultatifs {#optional}

La déclaration intégrée prend en charge des paramètres facultatifs qui modifient la manière dont le champ modifiable est présenté ou traité :

| Action | Paramètre | Exemple |
|---|---|---|
| Déclarez un champ modifiable avec une **valeur par défaut**. Lorsque le fragment est ajouté à un e-mail, cette valeur par défaut est utilisée, sauf si l’auteur la remplace. | Ajoutez la valeur par défaut entre les balises intégrées. | `{{#inline "editableFieldID"}}default_value{{/inline}}` |
| Définissez un **libellé** pour le champ modifiable. Ce libellé s’affiche dans le Designer d’e-mail lorsque l’auteur de l’e-mail modifie les champs du fragment. | `name="title"` | `{{#inline "editableFieldID" name="title"}}default_value{{/inline}}` |
| Déclarez un champ modifiable contenant une **source d’image**. | `assetType="image"` | `{{#inline "editableFieldID" assetType="image"}}default_value{{/inline}}` |
| Déclarez un champ modifiable contenant une **URL** qui doit être suivie. | `assetType="url"` | `{{#inline "editableFieldID" assetType="url"}}default_value{{/inline}}` |

## Ajout de champs modifiables à un composant HTML {#adding-editable-fields}

Pour rendre modifiables des parties d’un composant HTML dans un fragment visuel, procédez comme suit :

1. Ouvrez le fragment visuel à modifier dans le Designer d’e-mail.
1. Ajoutez un **composant** au fragment à partir du panneau Composants , ou sélectionnez un composant HTML existant.
1. Une fois le composant HTML sélectionné, cliquez sur **Afficher le code source** pour ouvrir la vue source HTML dans l’éditeur de personnalisation.
1. Dans l’éditeur de personnalisation, déclarez chaque variable modifiable à l’aide de la syntaxe de déclaration intégrée. Placez toutes les déclarations de variable en haut du composant pour plus de lisibilité et affectez un identifiant unique à chaque variable.
1. Référencez chaque variable dans le balisage HTML à l’aide de la syntaxe `{{{variableID}}}` où la valeur modifiable doit apparaître. La même variable peut être référencée plusieurs fois dans le même composant.
1. Enregistrez le composant HTML, puis enregistrez le fragment.
1. Publiez le fragment pour le rendre disponible pour une utilisation dans les e-mails.

## Utilisation du fragment dans un email {#using-fragment}

Une fois le fragment publié, toutes les variables déclarées dans ses composants HTML sont affichées en tant que paramètres modifiables dans le Designer d’e-mail.

Pour les personnaliser lors de l’utilisation du fragment dans un e-mail :

1. Ouvrez ou créez un e-mail dans le Designer d’e-mail Marketo Engage.
1. Ajoutez le fragment publié à la zone de travail de l’e-mail.
1. Sélectionnez le fragment pour ouvrir son volet Propriétés. La liste des champs modifiables s’affiche sous la section **Champs modifiables**, chaque champ étant libellé par son identifiant de variable (ou par le libellé convivial spécifié par le paramètre `name` ).
1. Mettez à jour la valeur de n’importe quel champ modifiable directement à partir du volet des propriétés. La modification s’applique uniquement à l’e-mail actuel ; le fragment publié et les autres e-mails qui y font référence ne sont pas affectés.
1. Enregistrez l’e-mail.

Le fragment s’affiche avec les valeurs personnalisées, tout en héritant des futures mises à jour structurelles apportées au fragment publié.

### Exemple : fragment simple avec texte modifiable, couleur et URL {#example}

L’exemple suivant crée une petite bannière promotionnelle avec quatre champs modifiables :

* une couleur de fond
* un texte de titre ;
* un libellé CTA ;
* une URL CTA ;

Après avoir publié le fragment, un auteur d’e-mail peut remplacer l’une de ces valeurs lors de l’ajout du fragment à un e-mail.

**Bannière modifiable simple**

```html
<!-- Define editable variables -->
{{#inline "bgColor"}}#0057FF{{/inline}}
{{#inline "headlineText"}}Example Headline{{/inline}}
{{#inline "ctaText"}}Learn More{{/inline}}
{{#inline "ctaUrl" assetType="url"}}https://www.example.com{{/inline}}

<!-- Use the variables in the HTML -->
<table width="100%" cellpadding="0" cellspacing="0"
       style="background-color:{{{bgColor}}}; border-radius:8px;" >
  <tr>
    <td style="padding:30px; text-align:center; font-family:Arial,sans-serif;">
      <h2 style="color:#ffffff; font-size:24px; margin:0;">
        {{{headlineText}}}
      </h2>
      <a href="{{{ctaUrl}}}"
         style="display:inline-block; margin-top:16px; padding:12px 28px;
                background:#ffffff; color:{{{bgColor}}};
                font-weight:bold; border-radius:4px; text-decoration:none;">
        {{{ctaText}}}
      </a>
    </td>
  </tr>
</table>
```

Dans cet exemple :

* `bgColor` est référencé deux fois : une fois pour la couleur d’arrière-plan du tableau et une fois pour la couleur du texte CTA. Les deux références se résolvent sur la même valeur, de sorte qu’une seule modification se propage aux deux emplacements.
* `ctaUrl` est déclaré avec `assetType="url"`, ce qui indique que la valeur doit être traitée en tant qu’URL suivie.

## Bonnes pratiques {#best-practices}

* Incluez des unités (`px`, `em`, `%`) à l’intérieur de la valeur par défaut de la variable afin que la variable représente une valeur CSS complète. Cela évite la concaténation, qui n’est pas prise en charge.
* Préférez les propriétés CSS à longue main côté par côté (`padding-top`, `padding-right`, `padding-bottom`, `padding-left`) aux propriétés abrégées lorsque chaque côté peut devoir être modifié indépendamment.
* Lorsqu’une URL doit être suivie, déclarez-la avec `assetType="url"`.
* Lorsqu’un champ modifiable porte une source d’image, déclarez-la avec `assetType="image"`.
* Testez le fragment en l’ajoutant à un e-mail de brouillon et en vérifiant que tous les champs modifiables apparaissent dans le volet des propriétés et sont résolus correctement lorsqu’ils sont remplacés.

## Choses à savoir {#things-to-know}

* Les champs modifiables dans les composants HTML prennent en charge le contenu de texte intégral, les URL complètes et les valeurs de propriété CSS complètes. Les URL partielles et les valeurs de propriété CSS partielles ne peuvent pas être paramétrées.
* Une seule valeur de propriété CSS ne peut pas combiner une variable avec un texte statique supplémentaire ou avec une autre variable. Chaque valeur de propriété paramétrée doit être exactement une référence de variable.
* Les identifiants de variable doivent être uniques dans un composant HTML et ne doivent pas contenir d’espaces.
* Les liens système d’usine, tels que le lien de désabonnement et l’URL de la page miroir, ne peuvent pas être transformés en champs modifiables.

<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->

>[!MORELIKETHIS]
>
>[Fragments](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
