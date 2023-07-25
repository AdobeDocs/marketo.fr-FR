---
unique-page-id: 1146995
description: Utilisation de jetons dans les étapes de flux - Documents Marketo - Documentation du produit
title: Utilisation de jetons dans les étapes de flux
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 5%

---

# Utilisation de jetons dans les étapes de flux {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

Un jeton est une variable. Vous l’utilisez dans les emails, les landing pages et les campagnes intelligentes pour faciliter votre vie. Vous pouvez utiliser [Mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (jetons personnalisés) dans les étapes de flux, webhooks, emails et landing pages. Vous pouvez utiliser des jetons pour inclure du contenu variable dans ces étapes de flux :

* Modifier valeur des données
* Modifier les données du membre du programme
* Moment significatif
* Étapes de campagne Salesforce (ajout, suppression, modification de l’état)
* Créer tâche
* Envoyer une alerte (dans les campagnes de déclenchement uniquement)

1. À l’étape du flux, commencez à saisir du texte `{{` pour obtenir des catégories de jeton.

   ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Consulter [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) pour une liste de plusieurs jetons disponibles.

1. Continuez à taper jusqu’à ce que vous trouviez le jeton de votre choix, puis cliquez pour le sélectionner.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Plusieurs jetons peuvent être utilisés dans les étapes Moment intéressant, Créer une tâche et Envoyer une alerte du flux.

   >[!NOTE]
   >
   >Les jetons de champ personnalisés de membre de programme peuvent être utilisés dans : Créer une tâche, Créer une tâche dans Microsoft, Moments intéressants, Modifier les actions de flux de valeur de données et WebHooks.

   Super ! Les données sont extraites du jeton lors de l’exécution de la campagne dynamique.

   >[!MORELIKETHIS]
   >
   >* [Gestion de mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Présentation de mes jetons dans un programme](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)
