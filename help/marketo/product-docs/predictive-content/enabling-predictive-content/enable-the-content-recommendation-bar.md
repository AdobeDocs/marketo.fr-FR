---
unique-page-id: 4720108
description: Activation de la barre de recommandations de contenu - Documents Marketo - Documentation du produit
title: Activer la barre de recommandation de contenu
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
feature: Predictive Content
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 3%

---

# Activer la barre de recommandation de contenu {#enable-the-content-recommendation-bar}

Le moteur de recommandation de contenu utilise des algorithmes d’analyse prédictive et de machine learning pour fournir du contenu pertinent à chaque visiteur web. Le moteur de recommandation prédit le contenu le plus performant par visiteur. Le contenu du moteur est surveillé et contrôlé dans la page Recommendations, ce qui vous aide à optimiser le retour sur investissement de votre contenu.

>[!PREREQUISITES]
>
>Avant d’activer le contenu prédictif, vous devez :
>
>* **Préparation de votre contenu prédictif**
>
>   * [Modifier le contenu prédictif des e-mails](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) ou
>   * [Modification du contenu prédictif pour les médias riches](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) ou
>   * [Modifier le contenu prédictif de la barre de recommandations](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [Approuver un titre pour le contenu prédictif](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)

## Activation et personnalisation de la barre de recommandations de contenu {#enable-and-customize-the-content-recommendation-bar}

1. Accédez à **[!UICONTROL Paramètres de contenu]**.

   ![](assets/settings-dropdown-hand.png)

1. Cliquez sur **[!UICONTROL Barre]**.

   ![](assets/content-settings-bar-hand.png)

1. Pour activer la barre de recommandations pour une URL, cliquez simplement sur **[!UICONTROL Activé]** puis **[!UICONTROL Enregistrer]**.

   ![](assets/bar-enable.png)

1. Pour personnaliser une URL, sélectionnez les couleurs, le style, le format, les flèches de la barre de recommandation et les pages à inclure ou à exclure de la barre. Personnalisez-le pour l’adapter à l’identité graphique de votre site web. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Inclure/exclure l’URL d’affichage**
   >
   >* L’URL d’affichage doit correspondre au chemin d’accès du domaine.
   >* N’incluez pas https:// ni https://
   >* Utiliser des &#42; pour les caractères génériques
   >* Utiliser un point-virgule comme séparateur
   >* Exemple : /contact_us&#42;; &#42;action=logout&#42;
   >* Ce champ respecte la casse.

## Considérations relatives aux barres de recommandations {#recommendation-bar-considerations}

* Vous avez besoin d’au moins un élément de contenu pour que la barre de recommandation soit définie sur **[!UICONTROL Activé]** sur la page Recommandations pour que le moteur de recommandation fonctionne. Si aucun contenu n’est activé et que la barre est définie sur **[!UICONTROL Activé]**, l’effet de flèche s’affiche en bas à droite de la page web, mais aucun contenu recommandé n’apparaît.

* Plus il y a de contenu exécuté dans le moteur de recommandation, mieux l’algorithme peut tester et identifier le contenu qui fonctionne le mieux. Nous vous recommandons de commencer par 10 à 20 éléments de contenu actifs en cours d’exécution et de continuer à en ajouter de nouveaux.
* L’élément de contenu que vous activez pour recommandation doit inclure la balise JavaScript RTP. Cela permet à l’algorithme de suivre et d’optimiser le contenu recommandé.

>[!MORELIKETHIS]
>
>[Activer le contenu prédictif pour les médias riches en contenu web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
