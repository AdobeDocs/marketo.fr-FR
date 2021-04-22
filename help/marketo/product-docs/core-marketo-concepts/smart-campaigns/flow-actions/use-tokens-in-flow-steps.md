---
unique-page-id: 1146995
description: Utiliser des jetons dans les étapes de flux - Documents Marketo - Documentation du produit
title: Utiliser des jetons dans les étapes de flux
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 8%

---

# Utiliser des jetons dans les étapes de flux {#use-tokens-in-flow-steps}

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus d&#39;informations.

>[!PREREQUISITES]
>
>[Ajouter une étape de flux à un Campaign dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

Un jeton est une variable. Vous l’utilisez dans les courriels, les landings page et les campagnes intelligentes pour faciliter votre vie. Vous pouvez utiliser [Mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (jetons personnalisés) dans les étapes de flux, les crochets Web, les courriers électroniques et les landings page. Vous pouvez utiliser des jetons pour inclure du contenu variable dans ces étapes de flux :

* Modifier valeur des données
* Modifier les données du membre du programme
* Moment significatif
* Etapes Campaign de Salesforce (ajouter, supprimer, modifier l’état)
* Créer tâche
* Envoyer une alerte (dans les campagnes de déclenchement uniquement)

1. À l’étape du flux, saisissez `{{` début pour obtenir des catégories de jeton. ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Consultez [Présentation des jetons](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) pour obtenir la liste de plusieurs jetons disponibles.

1. Continuez à taper jusqu’à ce que vous trouviez le jeton que vous souhaitez utiliser et cliquez pour le sélectionner.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Plusieurs jetons peuvent être utilisés dans les étapes de flux Moment intéressant, Création de Tâche et Envoyer une alerte.

   >[!NOTE]
   >
   >Les jetons de champ personnalisés de membre de programme peuvent être utilisés dans : Créez des Tâches, créez des Tâches dans Microsoft, des moments intéressants, des actions Modifier le flux de valeurs de données et des hameçons Web.

   Cool ! Les données sont extraites du jeton lors de l’exécution de la campagne dynamique.

   >[!MORELIKETHIS]
   >
   >* [Gestion de mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Présentation de mes jetons dans un Programme](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)

