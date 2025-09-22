---
description: Génération de questions - Documents Marketo - Documentation du produit
title: Génération de questions
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 3%

---

# Génération de questions {#question-generation}

Affichez toutes vos tâches et leurs détails pertinents, tels que la date de génération, le nombre total de questions, le statut d’approbation, etc.

## Générer des questions {#generate-questions}

1. Sous IA générative, cliquez sur **[!UICONTROL Réponses assistées]**.

   ![](assets/question-generation-1.png)

1. Cliquez sur **[!UICONTROL Générer des questions]**.

   ![](assets/question-generation-2.png)

1. Donnez un nom à votre tâche et saisissez une URL source (jusqu’à 10) à partir de laquelle tout le contenu sera extrait. Saisissez les rubriques/mots-clés souhaités et appuyez sur Entrée sur votre clavier. Lorsque vous avez terminé, cliquez sur **[!UICONTROL Générer]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Pour que Marketo Engage puisse récupérer du contenu à partir des URL fournies, vous devez d’abord placer sur la liste autorisée plusieurs adresses IP. [Voir ci-dessous pour plus de détails](#ip-addresses-to-allowlist).

   >[!NOTE]
   >
   >Les sites/pages doivent être publics (c’est-à-dire non masqués derrière une connexion) pour que leurs informations soient supprimées.

1. Selon votre contenu, la génération de la question et de la réponse peut prendre jusqu’à 30 minutes. Cliquez sur **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Appuyez sur Actualiser pour afficher le dernier statut de la génération de votre question.

   ![](assets/question-generation-5.png)

## Télécharger les questions et réponses {#download-questions-and-responses}

>[!NOTE]
>
>Les questions et réponses générées sont également visibles dans la [bibliothèque de réponses](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Recherchez la tâche souhaitée et cliquez sur l’icône de téléchargement en regard de son nom.

   ![](assets/question-generation-6.png)

1. Recherchez le dossier de téléchargements dans votre navigateur et sélectionnez le fichier . Cela peut varier en fonction du navigateur que vous utilisez.

   ![](assets/question-generation-7.png)

1. Dans le fichier Excel, **[!DNL Task details]** affiche uniquement ce détail, ainsi que divers détails sur la tâche, y compris des instructions sur la manière d’ajouter ou de modifier des questions et/ou des réponses.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Si vous décidez d’ajouter/modifier en bloc des questions et/ou des réponses, [découvrez comment les charger à nouveau ici](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. L’onglet **[!DNL Q&Rs]** fournit des détails supplémentaires, y compris les questions et réponses générées.

   ![](assets/question-generation-9.png)

## Adresses IP à Placer sur la liste autorisée {#ip-addresses-to-allowlist}

Afin de permettre l&#39;extraction du contenu de vos URL web pendant la génération des questions et réponses, localisez votre région ci-dessous et assurez-vous que l&#39;adresse IP qui lui est associée est bien placée sur la liste autorisée par votre équipe web.

<table width="450">
<thead>
  <tr>
    <th>Amérique du Nord</th>
    <th>Europe</th>
    <th>APAC</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>13.68.17.252</td>
    <td>20.105.150.224</td>
    <td>20.213.91.77</td>
  </tr>
</tbody>
</table>
