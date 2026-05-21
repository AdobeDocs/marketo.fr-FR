---
unique-page-id: 1146978
description: Découvrez comment utiliser une durée dans une étape de flux d’attente. Mettre le flux en pause pendant un nombre défini de jours avant l’action suivante.
title: Utiliser une durée dans une étape de flux Attendre
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/4T2sVyYvhrxdvwELe0DXw0zvGCywwHDKAuDGlIiIN9Q
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 216
ht-degree: 8%

---

# Utiliser une durée dans une étape de flux Attendre {#use-a-duration-in-a-wait-flow-step}

Vous pouvez utiliser l’étape Flux d’attente pour suspendre le parcours d’une personne par le biais d’une campagne intelligente pendant une certaine durée. Vous pouvez également définir des critères pour le jour de la semaine et l’heure de fin.

1. Dans l’onglet **[!UICONTROL Flux]** de votre campagne dynamique, faites glisser sur l’étape de flux **[!UICONTROL Attente]**.

   ![](assets/use-a-duration-in-a-wait-flow-step-1.png)

1. Saisissez la durée de la pause.

   ![](assets/use-a-duration-in-a-wait-flow-step-2.png)

1. Le flux se met en pause pendant la durée que vous avez spécifiée. Pour les options avancées, cliquez sur l’icône en forme d’engrenage à droite.

   ![](assets/use-a-duration-in-a-wait-flow-step-3.png)

1. Indiquez le jour de la semaine où l’étape d’attente doit se terminer.

   ![](assets/use-a-duration-in-a-wait-flow-step-4.png)

1. Vous pouvez éventuellement spécifier l’heure. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/use-a-duration-in-a-wait-flow-step-5.png)

   >[!NOTE]
   >
   >**Exemple**
   >
   >Une personne déclenche une campagne intelligente le vendredi à 17 h. L’étape d’attente est avancée : 48 heures et doit se terminer le lundi-vendredi à 9 h.
   >
   >Le résultat serait que la personne continuerait dans le flux le **lundi, 9 heures**. Il s’agit de la première date M-F après 48 heures.

   >[!NOTE]
   >
   >La durée, les dates, les heures et les jours utilisés dépendent tous du fuseau horaire de votre abonnement.

   >[!MORELIKETHIS]
   >
   >* [Utiliser une date spécifique dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [Utiliser un jeton de date dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
