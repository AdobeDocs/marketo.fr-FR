---
description: Génération de questions - Documents Marketo - Documentation du produit
title: Génération de questions
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: a711da0fe04e967bfc525be4f3df59d978021592
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Génération de questions {#question-generation}

Affichez toutes vos tâches et leurs détails pertinents, tels que le moment où elles ont été générées, le nombre total de questions, l’état d’approbation, etc.

## Générer des questions {#generate-questions}

1. Sous Generative AI, cliquez sur **[!UICONTROL Réponses assistées]**.

   ![](assets/question-generation-1.png)

1. Cliquez sur **[!UICONTROL Générer les questions]**.

   ![](assets/question-generation-2.png)

1. Donnez un nom à votre tâche et saisissez une URL source (jusqu’à 10) à partir de laquelle tout le contenu sera extrait. Saisissez les rubriques/mots-clés de votre choix, puis appuyez sur la touche Entrée de votre clavier. Une fois que vous avez terminé, cliquez sur **[!UICONTROL Générer]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Pour vous assurer que Marketo Engage peut extraire du contenu des URL fournies, vous devez d’abord placer sur la liste autorisée plusieurs adresses IP. [Voir ci-dessous pour plus de détails](#ip-addresses-to-allowlist).

   >[!NOTE]
   >
   >Les sites/pages doivent être publics (c’est-à-dire qu’ils ne doivent pas être masqués derrière une connexion) pour que leurs informations soient mises au rebut.

1. En fonction de votre contenu, la génération de questions et de réponses peut prendre jusqu’à 30 minutes. Cliquez sur **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Actualisez l’accès pour afficher le dernier état de la génération de questions.

   ![](assets/question-generation-5.png)

## Téléchargement des questions et réponses {#download-questions-and-responses}

>[!NOTE]
>
>Les questions et réponses générées sont également visibles dans la [bibliothèque de réponses](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Recherchez la tâche souhaitée et cliquez sur l’icône de téléchargement en regard de son nom.

   ![](assets/question-generation-6.png)

1. Recherchez le dossier de téléchargements dans votre navigateur et sélectionnez le fichier. Cela peut avoir un aspect différent selon le navigateur que vous utilisez.

   ![](assets/question-generation-7.png)

1. Dans le fichier Excel, **[!DNL Task details]** affiche précisément cela, divers détails sur la tâche, y compris des instructions sur la façon d&#39;ajouter/modifier des questions et/ou des réponses.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Si vous décidez d&#39;ajouter/modifier des questions et/ou des réponses en masse, [apprenez à les transférer ici](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. L’onglet **[!DNL Q&Rs]** fournit des détails supplémentaires, y compris les questions et réponses générées.

   ![](assets/question-generation-9.png)

## Adresses IP à Liste autorisée {#ip-addresses-to-allowlist}

Pour permettre l’extraction de contenu de vos URL web lors de la génération des questions et réponses, localisez votre région ci-dessous et vérifiez que l’adresse IP qui y est associée est placée sur la liste autorisée par votre équipe web.

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
