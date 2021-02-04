---
unique-page-id: 5472348
description: Rendre un modèle de Landing page de formulaire libre existant compatible avec les dispositifs portables - Documents marketing - Documentation du produit
title: Rendre un modèle de Landing page de formulaire libre existant compatible avec les dispositifs portables
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# Compatibilité d’un modèle de Landing page de formulaire libre existant {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Vous pouvez effectuer cette opération à deux endroits : l’éditeur de modèle et l’éditeur de Landing page.

## Mise à niveau à partir de l’éditeur de modèles {#upgrade-from-the-template-editor}

1. Accédez à **Design Studio**.

   ![](assets/designstudio-1.png)

1. Sélectionnez **Modèles**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Sélectionnez un modèle où **Mobile Compatible** est **Non**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Cliquez sur **Modifier le brouillon**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Cliquez sur **Rendre Mobile Compatible**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Cliquez sur **Mettre à niveau**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Votre modèle de landing page est désormais compatible avec les mobiles.

   >[!NOTE]
   >
   >La mise à niveau doit être inoffensive, mais assurez-vous de vérifier les différences entre les pages. La mise à niveau crée des brouillons de n’importe quel landing page utilisant ce modèle.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Qu’est-ce qui rend un modèle compatible avec les dispositifs portables ? {#what-makes-a-template-mobile-compatible}

De bonnes questions ! Votre modèle doit comporter les balises suivantes :

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

Si tout semble bien, vous verrez ce message.

![](assets/image2015-1-22-20-3a41-3a31.png)

Si un problème se produit, un message d’erreur s’affiche, cliquez sur réparer pour corriger le problème et recommencez le processus de validation.

![](assets/image2015-1-22-20-3a43-3a20.png)

Si vous apportez des modifications au modèle, cliquez sur Actions de modèle et sélectionnez Valider la compatibilité mobile.

## Mise à niveau d’un modèle à partir de l’éditeur de Landing page de forme libre {#upgrading-a-template-from-the-free-form-landing-page-editor}

Lorsque vous modifiez un landing page et que vous cliquez sur l’onglet mobile, vous constaterez parfois que le modèle n’a pas été mis à niveau. Peur non ! Vous pouvez le mettre à niveau juste ici.

1. Cliquez sur l&#39;onglet **Mobile**.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Cochez la case et cliquez sur **Activer**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >L&#39;activation de la version mobile d&#39;un modèle crée des brouillons de tous les landings page qui l&#39;utilisent.

Super ! Vous pouvez désormais [personnaliser la vue mobile](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) de tous les landings page qui utilisent ce modèle.
