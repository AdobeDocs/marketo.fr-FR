---
unique-page-id: 4720108
description: Activer la barre de recommandation du contenu - Documents marketing - Documentation du produit
title: Activation de la barre de recommandation de contenu
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---


# Activation de la barre de recommandation de contenu {#enable-the-content-recommendation-bar}

Le moteur de recommandation de contenu utilise des analyses prédictives et des algorithmes d’apprentissage automatique pour diffuser du contenu pertinent à chaque visiteur Web. Le moteur de recommandation prédit le contenu le plus performant par visiteur. Le contenu du moteur est surveillé et contrôlé sous la page Recommendations, ce qui vous permet d’optimiser le RSI de votre contenu.

>[!NOTE]
>
>**Conditions préalables**
>
>Avant d’activer le contenu prédictif, vous devez :
>
>* [Préparation du contenu prédictif](http://docs.marketo.com/display/docs/edit+predictive+content)
>* [Approbation d’un titre pour le contenu prédictif](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Activation et personnalisation de la barre de recommandation de contenu {#enable-and-customize-the-content-recommendation-bar}

1. Accédez à Paramètres **** de contenu.

   ![](assets/settings-dropdown-hand.png)

1. Cliquez sur **Barre**.

   ![](assets/content-settings-bar-hand.png)

1. Pour activer la barre de recommandation pour une URL, il vous suffit de cliquer sur **Activé** , puis **Enregistrer**.

   ![](assets/bar-enable.png)

1. Pour personnaliser une URL, sélectionnez les couleurs, le style, le format, les flèches de la barre de recommandation et les pages à inclure ou exclure la barre. Personnalisez votre site Web pour l’adapter à l’image de marque. Cliquez sur **Enregistrer**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Inclure / Exclure l’URL d’affichage**
   >
   >    * L’URL d’affichage doit être le chemin d’accès du domaine.
   >    * N’incluez pas http:// ou https://.
   >    * Utiliser * pour les caractères génériques
   * Utiliser un point-virgule comme séparateur
   * Exemple : /contact_us*; *action=déconnexion*
   * Ce champ est sensible à la casse


## Considérations relatives à la barre des recommandations {#recommendation-bar-considerations}

* Pour que le moteur de recommandation fonctionne, vous devez disposer d’au moins un élément de contenu pour que la barre de recommandations soit définie sur **Activé** sur la page Recommendations. Si aucun contenu n’est activé et que la barre est définie sur **Activé**, l’effet Flèche s’affiche en bas à droite de la page Web, mais aucun contenu recommandé n’apparaît.

* Plus le contenu s’exécute dans le moteur de recommandation, mieux l’algorithme peut le tester et savoir quel contenu fonctionne le mieux. Nous vous recommandons de commencer par 10 à 20 éléments de contenu en cours d&#39;exécution et principal et de continuer à en ajouter de nouveaux.
* L’élément de contenu que vous activez pour la recommandation doit inclure la balise JavaScript RTP. Cela permet à l’algorithme de suivre et d’optimiser le contenu recommandé.

>[!NOTE]
**Articles connexes**
* [Activer le contenu prédictif pour les médias enrichis en ligne](enable-predictive-content-for-web-rich-media.md)

