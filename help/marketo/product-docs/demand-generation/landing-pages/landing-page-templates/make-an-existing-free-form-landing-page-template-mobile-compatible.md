---
unique-page-id: 5472348
description: Rendre un modèle de page de destination de forme libre existant compatible avec les appareils mobiles - Documents Marketo - Documentation du produit
title: Rendre un modèle de page de destination de forme libre existant compatible avec les appareils mobiles
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Rendre un modèle de page de destination de forme libre existant [!UICONTROL compatible avec Mobile] {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Vous pouvez le faire à deux endroits : l’éditeur de modèles et l’éditeur de pages de destination.

## Mise à niveau à partir de l’éditeur de modèles {#upgrade-from-the-template-editor}

1. Accédez au **[!UICONTROL Design Studio]**.

   ![](assets/designstudio-1.png)

1. Sélectionnez **[!UICONTROL Modèles]**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Sélectionnez un modèle dans lequel **[!UICONTROL Compatible mobile]** est **[!UICONTROL Non]**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Cliquez sur **[!UICONTROL Rendre mobile compatible]**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Cliquez sur **[!UICONTROL Mettre à niveau]**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Votre modèle de landing page est désormais compatible avec les appareils mobiles.

   >[!NOTE]
   >
   >La mise à niveau doit être sans danger, mais veillez à vérifier les pages en cas d’incohérence. La mise à niveau créera des brouillons de toutes les pages de destination utilisant ce modèle.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Qu’est-ce qui rend un modèle [!UICONTROL compatible mobile] ? {#what-makes-a-template-mobile-compatible}

De bonnes questions ! Votre modèle doit comporter les balises suivantes :

`Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV>`

Si tout semble correct, ce message s’affiche.

![](assets/image2015-1-22-20-3a41-3a31.png)

Si un problème se produit, un message d’erreur s’affiche. Cliquez sur Réparer pour résoudre le problème et répétez le processus de validation.

![](assets/image2015-1-22-20-3a43-3a20.png)

Si vous apportez des modifications au modèle, cliquez sur [!UICONTROL Actions du modèle] et sélectionnez [!UICONTROL Valider la compatibilité mobile].

## Mise à niveau d’un modèle à partir de l’éditeur de page de destination à structure libre {#upgrading-a-template-from-the-free-form-landing-page-editor}

Lorsque vous modifiez une page de destination et que vous cliquez sur l’onglet mobile , vous remarquerez parfois que le modèle n’a pas été mis à niveau. N&#39;aie pas peur ! Vous pouvez le mettre à niveau ici.

1. Cliquez sur l’onglet **[!UICONTROL Mobile]**.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Cochez la case et cliquez sur **[!UICONTROL Activer]**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >L’activation de la version mobile d’un modèle crée des brouillons de toutes les pages de destination qui l’utilisent.

Génial ! Vous pouvez désormais [personnaliser la vue mobile](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) de toutes vos pages de destination qui utilisent ce modèle.
