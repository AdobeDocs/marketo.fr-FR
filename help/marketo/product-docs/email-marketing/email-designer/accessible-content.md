---
title: Concevoir du contenu accessible
description: Découvrez comment concevoir du contenu accessible pour vos emails dans Marketo Engage.
feature: Email Designer
role: User
level: Beginner, Intermediate
keywords: e-mail, conception, accessibilité
source-git-commit: 753455b40ead039a56c595fa61ab9a95b7936382
workflow-type: tm+mt
source-wordcount: '1367'
ht-degree: 45%

---

# Concevoir du contenu accessible {#accessible-content}

La [loi européenne sur l&#39;accessibilité](https://eur-lex.europa.eu/legal-content/FR/TXT/?uri=CELEX%3A32019L0882){target="_blank"} est une directive visant à renforcer le marché intérieur des produits et services accessibles en éliminant les obstacles dus aux différences entre les règles nationales des États membres.

Ce règlement stipule que toutes les communications numériques, y compris les e-mails, les newsletters, les fichiers PDF et le contenu téléchargeable, doivent être accessibles. Lors de la création de contenu pour vos destinataires, vous devez donc suivre des instructions spécifiques, telles que l’utilisation de polices et de formats lisibles accessibles, et fournir un texte secondaire pour les images.

Le Designer d’e-mail de Marketo Engage vous permet de vous conformer facilement à cette directive, en fonction des directives d’accessibilité du contenu web (WCAG) 2.1, niveau AA. Les bonnes pratiques pour concevoir un contenu accessible avec Marketo Engage sont répertoriées ci-dessous.

>[!NOTE]
>
>Cette page a pour but de rendre votre contenu accessible à tous vos destinataires, afin que les personnes en situation de handicap puissent lire, comprendre et interagir avec vos e-mails conçus dans Marketo Engage.

## Garantir la lisibilité du texte {#text-readability}

Utilisez l’onglet **[!UICONTROL Styles]** du composant **[!UICONTROL Texte]** pour vous assurer que votre texte est lisible, par exemple en utilisant un contraste de couleur approprié et des polices simples.

<!--![](assets/accessible-text-styles.png){width="80%"}-->

Pour les polices et le texte, suivez ces instructions :

**Sélection de la police**

* Utilisez des polices sans-serif telles qu’Arial, Verdana, Tahoma, Helvetica ou Open Sans.
* Évitez les polices en relief, cursives ou décoratives dans le contenu du corps.
* Conservez un jeu de polices limité pour garantir la cohérence et la fonctionnalité de secours (par exemple : `font-family: Arial, Helvetica, sans-serif;`).

**Taille de la police**

* Veillez à ce que la taille de police minimale du corps du texte soit de 16 pixels.
* Utilisez une hiérarchie appropriée pour les en-têtes.

**Contraste des couleurs**

* Utilisez un rapport de contraste d’au moins 4,5:1 entre le texte et l’arrière-plan.
* Pour un texte volumineux (≥24 px ou 18 px en gras), assurez-vous d’avoir un contraste d’au moins 3:1.
* Évitez le texte gris clair ou pastel sur fond blanc.
* Ne vous fiez pas uniquement à la couleur pour donner du sens. Utilisez des soulignements, des icônes, etc.

**Accessibilité du texte**

* Évitez le texte dans les images.
* N’utilisez pas de majuscules dans le corps du texte.
* Assurez-vous que le texte peut être zoomé à 200 % sans interrompre la mise en page.

## Garantir l’accessibilité visuelle {#visual-accessibility}

* Évitez d’utiliser des indicateurs de couleur uniquement pour les informations importantes.
* Utilisez des libellés de texte ou des icônes pour plus de clarté.
* Optimisez votre conception pour les mises en page mobiles et réactives en vous assurant que les boutons sont grands et suffisamment espacés.
* Effectuez des tests réguliers sur différents appareils et tailles d’écran pour garantir l’accessibilité.

Dans Marketo Engage, la taille et l’espacement des différents éléments de votre contenu peuvent être affinés à l’aide des paramètres et attributs de style du volet Designer d’e-mail **[!UICONTROL Styles]**.

Par exemple, vous pouvez mettre à jour l’arrière-plan ou modifier les marges, la marge intérieure et l’alignement pour améliorer l’accessibilité visuelle.

<!--![](assets/accessible-styles.png){width="80%"}-->

Marketo Engage Email Designer vous permet de prévisualiser et d’optimiser la conception pour différents appareils et tailles d’écran. Vous pouvez à tout moment **[!UICONTROL Basculer vers la vue en direct]** pour vérifier comment le rendu de votre contenu peut être effectué sur différentes tailles d’appareil.

<!--![](assets/accessible-live-view.png){width="80%"}-->

>[!CAUTION]
>
>L’aperçu en direct est un aperçu générique conçu pour comparer le rendu du contenu sur différentes tailles d’appareil. Le rendu final peut varier en fonction du client de messagerie de la personne destinataire.

## Utiliser un texte secondaire pour les images {#alt-text}

Utilisez le composant **[!UICONTROL Image]** pour fournir un texte secondaire pour les images.

<!--![](assets/accessible-alt-text.png){width="90%"}-->

* Décrivez l’objectif de l’image de manière concise et contextuelle.
* Évitez les expressions redondantes telles que « Image de... » et utilisez un texte secondaire vide pour les images décoratives.
* Pour les icônes significatives, fournissez des libellés significatifs. Pour les images complexes, utilisez un bref texte secondaire ainsi qu’une description plus détaillée ailleurs.

## Utiliser un format lisible {#readable-format}

Utilisez la structure et les composants de contenu pertinents du Designer d’e-mail, ainsi que les options du volet **[!UICONTROL Styles]** pour organiser votre contenu d’une manière claire, logique et concise, accessible à tous.

<!--![](assets/accessible-components.png){width="100%"}-->

* Utilisez du code HTML sémantique structuré avec des en-têtes, des paragraphes, des listes et des tableaux appropriés.
* Assurez-vous que le contenu suit un flux logique de gauche à droite, de haut en bas.
* Utilisez un langage clair et concis.
* Proposez des formats alternatifs pour les PDF et les infographies.
* Autorisez le redimensionnement et la redistribution du texte et assurez-vous que la typographie est lisible avec un contraste des couleurs adéquat dans tous les formats.

## Garantir la lisibilité du contenu {#readability}

Pour être lisible, votre contenu doit être clair, bien structuré et utilisable par tous, y compris les personnes ayant des difficultés visuelles, cognitives ou de lecture, ainsi que celles qui utilisent des technologies d’assistance. Voici quelques points à prendre en compte lors de la création de contenu accessible :

* Limitez les phrases à une vingtaine de mots ou moins.
* Modifiez votre copie pour qu’elle soit directe et concise.
* Utilisez la voix active pour simplifier la structure de la phrase.
* Évitez l&#39;argot, le jargon ou les mots régionaux que certaines personnes ne connaissent pas.

Pour évaluer la lisibilité de vos e-mails, vous pouvez utiliser le test de lisibilité [Flesch Reading Ease](https://support.microsoft.com/fr-fr/office/get-your-document-s-readability-and-level-statistics-85b4969e-e80a-4777-8dd3-f7fc3c8b3fd2){target="_blank"}, disponible dans Microsoft Word et qui calcule la facilité de lecture de votre contenu sur une échelle de 0 à 100.

## Tester votre contenu {#test}

Pour vérifier l’accessibilité de votre contenu, vous pouvez utiliser les fonctionnalités de test fournies par Marketo Engage. Elles ne sont pas spécialement conçues pour vérifier si le contenu est entièrement accessible, mais elles peuvent fournir un premier niveau de vérification.

* Prévisualisez votre contenu à l’aide de profils de test.

* Utilisez l’option [Rendu d’e-mail](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md){target="_blank"} qui tire parti de Litmus pour simuler vos conceptions sur les principaux clients de messagerie (Apple Mail, Gmail, Outlook) et vérifier si le texte, les couleurs et les images rendent votre contenu accessible. <!--Litmus includes accessibility testing-->

* Envoyez des BAT pour tester le rendu de votre contenu avant de l’envoyer à votre audience réelle.

<!--![](assets/accessible-simulate.png){width="90%"}-->

Pour vérifier de manière plus fiable si votre contenu est accessible, recherchez des outils externes spécifiques tels que :

* Le [vérificateur de contraste WebAim](https://webaim.org/resources/contrastchecker/){target="_blank"} et l’[outil d’évaluation de l’accessibilité web WAVE](https://wave.webaim.org/){target="_blank"} pour évaluer le contraste et la conformité ;

* Les technologies d’assistance comme les lecteurs d’écran (par exemple : [NVDA](https://www.nvaccess.org/download/){target="_blank"} ou [VoiceOver](https://support.apple.com/fr-fr/guide/iphone/iph3e2e415f/ios){target="_blank"} sur iPhone) pour consulter les e-mails du point de vue des utilisateurs souffrant de déficience visuelle.

## Utiliser le mode sombre {#dark-mode}

Le [mode sombre](/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md){target="_blank"} améliore l’accessibilité visuelle pour les utilisateurs et utilisatrices sensibles à la lumière ou ayant une déficience visuelle, pour une expérience de visionnage améliorée.

<!--![](assets/accessible-dark-mode.png){width="90%"}-->

Voici quelques bonnes pratiques pour concevoir du contenu en mode sombre :

* Utilisation de PNG ou de SVG transparents
* Définition des balises de métadonnées et du code CSS appropriés
* Fournir un style de secours accessible si le mode sombre n’est pas pris en charge.

Assurez-vous que vos e-mails s’affichent correctement en mode sombre en testant tout le contenu des e-mails et les éléments de l’interface utilisateur en modes clair et sombre.

## Utiliser des attributs spécifiques pour l’accessibilité {#attributes}

### Attributs de langue {#language}

Lors de la création de conceptions, incluez les attributs `lang` (langue) et `dir` (sens d’écriture) dans le corps du contenu. Ces attributs aident les technologies d’assistance (comme les lecteurs d’écran) à interpréter et présenter votre contenu d’une manière appropriée.

* L’attribut `lang` indique la langue de l’e-mail aux technologies d’assistance, afin que les mots soient prononcés correctement.

  +++Exemples

  Exemple pour l’anglais :

  ```
  <body lang="en">
  ```

  Exemple pour le français :

  ```
  <body lang="fr">
  ```

  +++

* L’attribut `dir` spécifie le sens de l’écriture. La plupart des langues, y compris l’anglais et le français, se lisent de gauche à droite (ltr), tandis que les langues telles que l’arabe et l’hébreu se lisent de droite à gauche (rtl).

  +++Exemples

  Exemple pour l’anglais (de gauche à droite) :

  ```html
  <body lang="en" dir="ltr">
  ```

  Exemple pour l’arabe (de droite à gauche) :

  ```html
  <body lang="ar" dir="rtl">
  ```

  +++

Les lecteurs d’écran se réfèrent à l’attribut `lang` pour appliquer les bonnes règles de prononciation, tandis que le sens de l’écriture assure naturellement l’agencement du contenu pour les langues écrites de gauche à droite ou de droite à gauche. Sans ces attributs, l’ordre de lecture peut être confus et des mots peuvent être mal prononcés. Encapsulez toujours le corps de votre e-mail avec les attributs de `lang` et de `dir` appropriés.

>[!TIP]
>
>Si votre e-mail contient plusieurs langues, attribuez les attributs de langue appropriés à des sections spécifiques (comme des blocs de `<table>` ou de `<td>`) pour vous assurer que chaque partie est lue correctement.

### Tableaux {#tables}

Dans le contenu HTML, les tableaux sont souvent utilisés pour la mise en page. Par défaut, les lecteurs d’écran traitent chaque `<table>` comme un tableau de données, annonçant les lignes, les colonnes et la structure. Cela peut prêter à confusion si le tableau n’est utilisé que pour la mise en forme.

Ajoutez `role="presentation"` (ou `role="none"`) aux tableaux de mise en page pour vous assurer que les technologies d’assistance ignorent leur structure et se concentrent uniquement sur le contenu.

+++Exemple - Tableau de disposition (avec `role="presentation"`)

```html
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="100%"> 
  <tr> 
    <td align="center"> 
      <h1>Hello World</h1> 
      <p>Welcome to our newsletter</p> 
    </td> 
  </tr> 
</table>
```

Les lecteurs d’écran lisent :
« Bonjour tout le monde. Bienvenue dans notre newsletter. » _(Aucune mention de lignes, colonnes ni tableau)_

+++

+++Exemple - Tableau de données (sans `role="presentation"`)

```html
<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <th scope="col">Name</th>
    <th scope="col">Score</th>
  </tr>
  <tr> 
    <td>Peter</td>
    <td>19</td>
  </tr>
  <tr>
    <td>Parker</td>
    <td>62</td>
  </tr>
</table>
```

Les lecteurs d’écran lisent :
« Tableau avec 2 colonnes et 3 lignes. »

« Nom, Peter. Score, 19. »

« Nom, Parker. Score, 62. »

+++

>[!TIP]
>
>Utilisez `role="presentation"` exclusivement pour les tableaux de mise en page. Pour les tableaux de données, conservez la structure `<table>` sémantique afin que les lecteurs d’écran puissent annoncer correctement les en-têtes et les relations.

### Texte des liens {#links}

Les lecteurs d’écran lisent les liens à l’aide de leur texte. Si le libellé d’un lien est uniquement « Cliquez ici » ou « En savoir plus », les utilisateurs et utilisatrices de technologies d’assistance ne connaîtront pas la destination. Pour garantir leur accessibilité, ils ont besoin d’un texte descriptif qui indique clairement la cible ou l’action.

Utilisez le Designer d’e-mail pour ajouter un lien à votre contenu et modifier le libellé afin de le rendre perceptible (visible) et descriptif (clarifier l’objectif). Évitez les libellés vagues tels que « ici » ou « plus ».

<!--![](assets/accessible-link.png){width="70%"}-->

+++Exemple - Bon lien (descriptif) : 

```
<p>Learn more in the  
<a href="https://adobe.com/release-notes">August release notes</a>. 
</p>
```

Les lecteurs d’écran lisent :
« Lien, notes de mise à jour d’août. »

+++

+++Exemple - Lien incorrect (non descriptif)

```
<p>Learn more about our new features.  
  <a href="https://adobe.com/release-notes">Click here</a>. 
</p>
```

Les lecteurs d’écran lisent :
« Lien, cliquez ici. » *(Ne fournit aucun contexte en dehors de l’ordre de lecture.)*

+++

<!--for Landing Pages-->

<!--## Provide keyboard navigation and focus support {#keyboard}

Providing keyboard navigation and focus support allows people who cannot use a mouse to fully access and interact with content. It also improves overall usability by giving all users a clear and consistent way to move through information.

* Focus via keyboard
    * Ensure all interactive elements (such as buttons, checkboxes, links) have `tabindex="0"` so they are included in the natural tab order. 
    * Allow navigation using the Tab and arrow keys (↑ ↓ ← →), which should visibly highlight the focused element. 
* Custom focus styling 
    * Apply clear and distinguishable styles for focusing on actionable elements: 
        +++Example (CSS)

        ```
        [tabindex="0"] : focus { 
        outline: 2px solid #00AEEF;  /* Cyan border */ 
        background-color: #20CEFF;   /* Optional background */ 
        }
        ```
        
        +++

    * Ensure that focus indicators meet the WCAG 2.2 focus appearance standards, including: 
        * Minimum area: 2 CSS pixel thick outline.
        * Contrast ratio: ≥ 3:1 between focused and unfocused state. 

* Keyboard activation support 
    * Ensure checkboxes and buttons respond to the Enter and Space keys. 
    * Validate the interaction using the keyboard alone: 
        * Enter or Space should toggle checkboxes.
        * Enter or Space should trigger the buttons.-->
