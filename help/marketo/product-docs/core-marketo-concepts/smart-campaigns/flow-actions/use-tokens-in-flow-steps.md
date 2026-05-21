---
unique-page-id: 1146995
description: Découvrez comment utiliser des jetons dans les étapes de flux. Insérez des valeurs dynamiques dans le contenu de l’étape de flux et les e-mails.
title: Utiliser des jetons dans des étapes de flux
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/0b1iseuF-rKtBcS2qPRdwnPPRYJxUNG9hzlJQxNJQdI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 10%

---

# Utiliser des jetons dans des étapes de flux {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Ajouter une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Un jeton est une variable. Vous l’utilisez dans les e-mails, les landing pages et les campagnes intelligentes pour vous simplifier la vie. Vous pouvez utiliser [Mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (jetons personnalisés) dans les étapes de flux, les webhooks, les e-mails et les pages de destination. Vous pouvez utiliser des jetons pour inclure du contenu variable dans les étapes de flux suivantes :

* Modification de la valeur des données
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

   Les données sont extraites du jeton lors de l’exécution de la campagne intelligente.

   >[!MORELIKETHIS]
   >
   >* [Gestion de mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Présentation de mes jetons dans un programme](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
