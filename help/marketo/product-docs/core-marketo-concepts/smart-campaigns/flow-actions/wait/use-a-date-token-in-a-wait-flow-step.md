---
unique-page-id: 1146997
description: Utilisation d’un jeton de date dans une étape de flux d’attente - Documents Marketo - Documentation du produit
title: Utilisation d’un jeton de date dans une étape de flux d’attente
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Utilisation d’un jeton de date dans une étape de flux d’attente {#use-a-date-token-in-a-wait-flow-step}

Vous pouvez utiliser l’étape Flux d’attente pour suspendre le parcours d’une personne via une campagne dynamique jusqu’à une date spécifique qui utilise un jeton de date. Vous pouvez également modifier la date de fin d’un certain nombre de jours.

>[!NOTE]
>
>Cela s’applique uniquement aux campagnes de déclenchement. Vous ne pouvez pas utiliser cette fonctionnalité dans les campagnes par lots.

1. Dans l’onglet **[!UICONTROL Flux]** de votre campagne dynamique, faites glisser le curseur sur l’étape de flux **[!UICONTROL Attente]** .

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. Cliquez sur l’icône d’engrenage.

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. Dans la liste déroulante **[!UICONTROL Type]**, sélectionnez **[!UICONTROL Jeton de date]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. Sélectionnez un jeton Date pour indiquer à quel moment l’étape d’attente doit se terminer :

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. Cochez la case pour attendre le prochain anniversaire de la date se produisant dans l’année civile en cours ou l’année suivante.

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >Utilisez cette option sur les jetons de date qui font référence à des dates antérieures, telles qu’un anniversaire ou la date de début du contrat.

1. Vous pouvez éventuellement modifier la date de fin d’un nombre spécifié de jours.

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >Vous pouvez également spécifier le nombre de jours à l’aide d’un jeton `{{lead.` ou `{{company.` qui représente un champ entier, ou d’un jeton `{{my.` de type nombre.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [Utiliser une durée dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Utiliser une date spécifique dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
