---
unique-page-id: 1146995
description: Utiliser des jetons dans les étapes de flux - Documents marketing - Documentation du produit
title: Utiliser des jetons dans les étapes de flux
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Utiliser des jetons dans les étapes de flux {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>* [Ajouter une étape de flux à un Campaign dynamique](add-a-flow-step-to-a-smart-campaign.md)


Un jeton est une variable. Vous l’utilisez dans les [courriels](https://docs.marketo.com/pages/viewpage.action?pageId=557076), les [landings page](https://docs.marketo.com/pages/viewpage.action?pageId=2359689)et les campagnes [](https://docs.marketo.com/display/DOCS/Smart+Lists+and+Lists) intelligentes pour faciliter votre vie. Vous pouvez utiliser [Mes jetons](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (jetons personnalisés) dans les étapes de flux, les crochets Web, les courriers électroniques et les landings page.  Vous pouvez utiliser des jetons pour inclure du contenu variable dans ces étapes de flux :

* Modifier la valeur des données
* Moment intéressant
* Etapes Campaign de Salesforce (ajouter, supprimer, modifier l’état)
* Créer une Tâche
* Envoyer une alerte (dans les campagnes de déclenchement uniquement)

>[!NOTE]
>
>**Disponibilité**
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus de détails.

1. Dans l’étape de flux, saisissez le début `{{` pour obtenir des catégories de jeton. ![](assets/image2014-9-22-14-3a3-3a17.png)>

   >[!NOTE]
   >
   >**Plongée profonde**
   >
   >Consultez la présentation [des](../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) jetons pour obtenir une liste de plusieurs jetons disponibles.

1. Continuez à taper jusqu’à ce que vous trouviez le jeton que vous souhaitez utiliser et cliquez pour le sélectionner.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Plusieurs jetons peuvent être utilisés dans les étapes de flux Moment intéressant, Création de Tâche et Envoyer une alerte.

   >[!NOTE]
   >
   >**Articles connexes**
   >
   >* [Gestion de mes jetons](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Présentation de mes jetons dans un Programme](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)


Cool ! Les données sont extraites du jeton lors de l’exécution de la campagne dynamique.