---
solution: Marketo Engage
product: marketo
title: TITLE
description: Découvrez comment ajouter du code CSS personnalisé au contenu de votre e-mail directement dans le Designer d’e-mail de Marketo Engage.
level: Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
exl-id: c191b44a-47ab-41f8-aa95-9268e359e5db
source-git-commit: ca8644c43cfbdbaf7be9f21c5e440949b796cfdb
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 30%

---

# Ajouter du CSS personnalisé au contenu de votre e-mail {#email-metadata}

Ajoutez votre propre CSS personnalisé directement dans le Designer d’e-mail Marketo Engage pour un style avancé et spécifique.

## Définir un CSS personnalisé {#define-custom-css}

1. Vérifiez qu’un contenu est défini dans le Designer d’e-mail en ajoutant au moins un composant.

1. Sélectionnez **[!UICONTROL Corps]** dans l’arborescence de navigation **[!UICONTROL à gauche]** ou dans le volet de droite. **[!UICONTROL Styles CSS]** s’affiche à droite.

   CAPTURE D’ÉCRAN

   >[!NOTE]
   >
   >La section **[!UICONTROL Styles CSS]** n’est disponible que lorsque du contenu est présent dans l’éditeur.

1. Cliquez sur le bouton **[!UICONTROL + Ajouter un CSS personnalisé]** .

   >[!NOTE]
   >
   >Le bouton **[!UICONTROL Ajouter un fichier CSS personnalisé]** n’est disponible que lorsque **[!UICONTROL Corps]** est sélectionné. Cependant, vous pouvez appliquer des styles CSS personnalisés à tous les composants de votre contenu.

1. Saisissez votre code CSS dans la zone de texte dédiée qui s’affiche. Assurez-vous que le code CSS personnalisé est valide et suit la syntaxe appropriée. [En savoir plus](#use-valid-css)

   CAPTURE D’ÉCRAN

   >[!NOTE]
   >
   >Vous ne pouvez pas ajouter de CSS personnalisé à votre contenu lors de l’utilisation d’un [modèle avec du contenu verrouillé](/help/marketo/product-docs/email-marketing/email-designer/content-locking.md). Le libellé du bouton se transforme en **[!UICONTROL Affichage du code CSS personnalisé]** et tout code CSS personnalisé affiché est en lecture seule.

1. Enregistrez votre CSS personnalisé et assurez-vous qu’il s’applique à votre contenu. Dans le cas contraire, consultez la section [Dépannage](#troubleshooting).

   CAPTURE D’ÉCRAN

   >[!NOTE]
   >
   >Si vous supprimez tout le contenu, la section disparaît et le CSS personnalisé défini précédemment n’est plus appliqué. Ajoutez à nouveau du contenu pour que la section **[!UICONTROL styles CSS]** réapparaisse. Le CSS personnalisé s’applique à nouveau.

## Utilisation d’un CSS valide {#using-valid-css}

Vous pouvez saisir n’importe quelle chaîne CSS valide dans la zone de texte **[!UICONTROL Ajouter un fichier CSS personnalisé]**. Si le fichier CSS est correctement formaté, il s’applique immédiatement au contenu.

>[!CAUTION]
>
>Vous êtes responsable de la sécurité de votre CSS personnalisé. Assurez-vous que votre CSS n’introduit pas de vulnérabilités ou de conflits avec le contenu existant.
>
>Évitez d’utiliser une page CSS qui pourrait altérer involontairement la disposition ou la fonctionnalité du contenu.

+++ Exemples de CSS valide

Vous trouverez ci-dessous des exemples de CSS valide.

```css
.acr-component[data-component-id="form"] {
  display: flex;
  justify-content: center;
  background: none;
}

.acr-Form {
  width: 100%;
  padding: 20px 100px;
  border-spacing: 0px 8px;
  box-sizing: border-box;
  margin: 0;
}

.acr-Form .spectrum-FieldLabel {
  width: 20%;
}

.acr-Form.spectrum-Form--labelsAbove .spectrum-FieldLabel,
.acr-Form [data-form-item="checkbox"] .spectrum-FieldLabel {
  width: auto;
}

.acr-Form .spectrum-Textfield {
  width: 100%;
}

#acr-form-error,
#acr-form-confirmation {
  width: 100%;
  padding: var(--spectrum-global-dimension-static-size-500);
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  gap: var(--spectrum-global-dimension-static-size-200);
}

.spectrum-Form-item.is-required .spectrum-FieldLabel:after{
  content: '*';
  font-size: 1.25rem;
  margin-left: 5px;
  position: absolute;
}

/* Error field placeholder */
.spectrum-HelpText {
  display: none !important;
}

.spectrum-HelpText.is-invalid,
.is-invalid ~ .spectrum-HelpText {
  display: flex !important;
}
```

```css
@media only screen and (min-width: 600px) {
  .acr-paragraph-1 {
    width: 100% !important;
  }
}
```

+++


+++ Exemples de CSS non valides

Si une page CSS non valide est saisie, un message d’erreur s’affiche, indiquant que la page CSS ne peut pas être enregistrée. Vous trouverez ci-dessous des exemples de CSS non valides.

L’utilisation de balises `<style>` n’est pas acceptée :

```html
<style type="text/css">
  .acr-Form {
    width: 100%;
    padding: 20px 100px;
    border-spacing: 0px 8px;
    box-sizing: border-box;
    margin: 0;
  }
</style>
```

Une syntaxe non valide, comme l’omission des accolades, n’est pas acceptée :

```css
body {
  background: red;
```

+++

## Implémentation technique {#implementation}

Votre CSS personnalisé est ajouté à la fin de la section `<head>` dans le cadre d’une balise `<style>` avec l’attribut `data-name="global-custom"`, comme dans l’exemple ci-dessous. Cela permet de s’assurer que les styles personnalisés sont appliqués globalement au contenu.

+++ Voir l’exemple

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="content-version" content="3.3.31">
    <meta name="x-apple-disable-message-reformatting">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <style data-name="default" type="text/css">
      td { padding: 0; }
      th { font-weight: normal; }
    </style>
    <style data-name="grid" type="text/css">
      .acr-grid-table { width: 100%; }
    </style>
    <style data-name="acr-theme" type="text/css" data-theme="default" data-variant="0">
      body { margin: 0; font-family: Arial; }
    </style>
    <style data-name="media-default-max-width-500px" type="text/css">
      @media screen and (max-width: 500px) {
        body { width: 100% !important; }
      }
    </style>
    <style data-name="global-custom" type="text/css">
      /* Add you custom CSS here */
    </style>
  </head>
  <body>
    <!-- Minimal content -->
  </body>
</html>
```

+++


Le CSS personnalisé n’est pas interprété ni validé par le volet **[!UICONTROL Paramètres]** du concepteur d’e-mail. Il est entièrement indépendant et ne peut être modifié que par l’intermédiaire de l’option **[!UICONTROL Ajouter un fichier CSS personnalisé]**.

### Mécanismes de sécurisation - Contenu importé {#guardrails}

Si vous souhaitez utiliser un CSS personnalisé avec du contenu importé dans le concepteur d’e-mail, tenez compte des points suivants :

* Si vous [importez du contenu HTML externe](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) y compris du contenu CSS, à moins de convertir ce contenu, il se trouvera en **[!UICONTROL mode de compatibilité]**, où la section **[!UICONTROL styles CSS]** n’est pas disponible.

* Si l’importation de contenu créé avec le Designer d’e-mail inclut un CSS appliqué via l’option **[!UICONTROL Ajouter un CSS personnalisé]**, le CSS précédemment appliqué sera visible et modifiable à partir de la même option.

## Dépannage {#troubleshooting}

Si votre CSS personnalisé n’est pas appliqué, essayez les suggestions ci-dessous.

* Assurez-vous que votre CSS est valide et ne comporte pas d’erreurs de syntaxe (telles que des accolades manquantes, des noms de propriété incorrects). [Voici comment procéder](#use-valid-css)

* Assurez-vous que votre CSS est ajouté à la balise `<style>` avec l’attribut `data-name="global-custom"`.

* Vérifiez si la balise de style de `global-custom` possède l’attribut `data-disabled` défini sur `true`. Si tel est le cas, le code CSS personnalisé n’est pas appliqué.

+++ Par exemple :

  ```html
  <style data-name="global-custom" type="text/css" data-disabled="true"> body: { color: red; } </style>
  ```

+++

* Assurez-vous que votre CSS n’est pas remplacée par d’autres règles CSS.

   * Utilisez les outils de développement de votre navigateur pour inspecter le contenu et vérifier que votre CSS cible les sélecteurs corrects.

   * Pensez à ajouter des `!important` à vos déclarations pour vous assurer qu’elles sont prioritaires.

+++ Par exemple :

     ```css
     .acr-Form {
       background: red !important;
     }
     ```

+++

>[!NOTE]
>
>La prise en charge de Marketo Engage n’est pas configurée pour vous aider à résoudre les problèmes liés au CSS personnalisé. Pour obtenir de l’aide sur CSS, consultez un développeur ou une développeuse web.
