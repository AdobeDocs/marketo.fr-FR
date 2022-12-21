---
unique-page-id: 4720108
description: Activation de la barre de recommandation de contenu - Documents Marketo - Documentation du produit
title: Activation de la barre de recommandation de contenu
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Activation de la barre de recommandation de contenu {#enable-the-content-recommendation-bar}

Le moteur de recommandation de contenu utilise des algorithmes d’analyse prédictive et d’apprentissage automatique pour diffuser du contenu pertinent à chaque visiteur web. Le moteur de recommandation prédit le contenu le plus performant par visiteur. Le contenu du moteur est surveillé et contrôlé dans la page Recommendations, ce qui vous permet d’optimiser le retour sur investissement de votre contenu.

>[!PREREQUISITES]
>
>Avant d’activer le contenu prédictif, vous devez :
>
>* **Préparation de votre contenu prédictif**
   >
   >   * [Modifier le contenu prédictif pour les emails](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) ou
   >   * [Modification du contenu prédictif pour le contenu multimédia enrichi](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) ou
   >   * [Modifier le contenu prédictif pour la barre de recommandations](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [Approbation d’un titre pour le contenu prédictif](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Activation et personnalisation de la barre de recommandation de contenu {#enable-and-customize-the-content-recommendation-bar}

1. Accédez à **Paramètres Contenu**.

   ![](assets/settings-dropdown-hand.png)

1. Cliquez sur **Barre**.

   ![](assets/content-settings-bar-hand.png)

1. Pour activer la barre de recommandation pour une URL, cliquez simplement sur **Activé** puis **Enregistrer**.

   ![](assets/bar-enable.png)

1. Pour personnaliser une URL, sélectionnez les couleurs, le style, le format, les flèches de la barre de recommandations et les pages à inclure ou exclure de la barre. Personnalisez pour l’adapter à l’identité graphique de votre site web. Cliquez sur **Enregistrer**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**URL d’affichage d’inclusion/exclusion**
   >
   >* L’URL d’affichage doit être le chemin du domaine.
   >* N’incluez pas https:// ou https://
   >* Utilisation &#42; pour les caractères génériques
   >* Utilisation d’un point-virgule comme séparateur
   >* Exemple : /contact_us&#42;; &#42;action=logout&#42;
   >* Ce champ est sensible à la casse


## Observations sur la barre de recommandation {#recommendation-bar-considerations}

* Vous avez besoin d’au moins un élément de contenu pour que la barre de recommandations soit définie sur **Activé** sur la page Recommendations pour que le moteur de recommandation fonctionne. Si aucun contenu n’est activé et que la barre est définie sur **Activé**, l’effet Flèche s’affiche en bas à droite de la page web, mais aucun contenu recommandé ne s’affiche.

* Plus le contenu s’exécute dans le moteur de recommandations, mieux l’algorithme peut le tester et apprendre quel contenu fonctionne le mieux. Nous vous recommandons de commencer par 10 à 20 éléments de contenu en cours d’exécution et principaux et de continuer à en ajouter de nouveaux.
* L’élément de contenu que vous activez pour la recommandation doit inclure la balise JavaScript RTP. Cela permet à l’algorithme de suivre et d’optimiser le contenu recommandé.

>[!MORELIKETHIS]
>
>[Activation du contenu prédictif pour le contenu multimédia Web enrichi](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
