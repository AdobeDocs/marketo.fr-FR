---
unique-page-id: 1146995
description: Utilisation de jetons dans les étapes de flux - Documents Marketo - Documentation du produit
title: Utiliser des jetons dans des étapes de flux
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 10%

---

# Utiliser des jetons dans des étapes de flux {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Ajouter une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Un jeton est une variable. Vous l’utilisez dans les e-mails, les landing pages et les campagnes intelligentes pour vous simplifier la vie. Vous pouvez utiliser [Mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (jetons personnalisés) dans les étapes de flux, les webhooks, les e-mails et les pages de destination. Vous pouvez utiliser des jetons pour inclure du contenu variable dans les étapes de flux suivantes :

* Modifier la valeur des données
* Modifier les données de la personne membre du programme
* Moment intéressant
* [!DNL Salesforce] étapes de la campagne (ajout, suppression, changement de statut)
* Créer une tâche
* Envoyer l’alerte (dans les campagnes de déclenchement uniquement)

1. Dans l’étape de flux, commencez à saisir `{{` pour obtenir des catégories de jeton.

   ![](assets/use-tokens-in-flow-steps-1.png)

   >[!NOTE]
   >
   >Consultez [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} pour obtenir une liste de plusieurs jetons disponibles.

1. Continuez à taper jusqu’à ce que vous trouviez le jeton souhaité, puis cliquez pour le sélectionner.

   ![](assets/use-tokens-in-flow-steps-2.png)

   >[!TIP]
   >
   >Plusieurs jetons peuvent être utilisés dans les étapes de flux Moment intéressant, Créer une tâche et Envoyer une alerte .

   >[!NOTE]
   >
   >Les jetons de champ personnalisé de membre de programme peuvent être utilisés dans les actions suivantes : Créer une tâche, Créer une tâche dans Microsoft, Moments significatifs, Modifier le flux de valeurs de données et Webhooks.

   Cool ! Les données sont extraites du jeton lors de l’exécution de la campagne intelligente.

   >[!MORELIKETHIS]
   >
   >* [Gestion de mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Présentation de mes jetons dans un programme](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
