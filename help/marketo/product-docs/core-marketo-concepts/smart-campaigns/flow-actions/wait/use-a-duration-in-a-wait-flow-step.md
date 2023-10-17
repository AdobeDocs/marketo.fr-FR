---
unique-page-id: 1146978
description: Utiliser une durée dans une étape de flux d’attente - Documents Marketo - Documentation du produit
title: Utilisation d’une durée dans une étape de flux d’attente
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 1%

---

# Utilisation d’une durée dans une étape de flux d’attente {#use-a-duration-in-a-wait-flow-step}

Vous pouvez utiliser l’étape de flux d’attente pour suspendre le parcours d’une personne lors d’une campagne dynamique pendant une certaine durée. Vous pouvez également spécifier des critères pour le jour de la semaine et l’heure de fin.

1. Dans votre campagne dynamique **[!UICONTROL Flux]** , faites glisser sur l’onglet **[!UICONTROL Attente]** étape de flux.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Saisissez la durée de la pause.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. C&#39;est tout ! Le flux est interrompu pendant la durée que vous avez spécifiée. Pour les options avancées, cliquez sur l’icône d’engrenage à droite.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Spécifiez le jour de la semaine où l’étape d’attente doit se terminer.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Vous pouvez éventuellement spécifier l’heure. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Exemple**
   >
   >Une personne déclenche une campagne dynamique le vendredi à 17 heures. L’étape d’attente est avancée : 48 heures et doit se terminer le lundi-vendredi à 9h du matin.
   >
   >Le résultat serait que la personne continuerait dans le flux de **Lundi, 9h**. Il s’agit de la première date M-F après 48 heures.

   >[!NOTE]
   >
   >La durée, les dates, les heures et les jours utilisés dépendent du fuseau horaire de votre abonnement.

   >[!MORELIKETHIS]
   >
   >* [Utilisation d’une date spécifique dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [Utilisation d’un jeton de date dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
