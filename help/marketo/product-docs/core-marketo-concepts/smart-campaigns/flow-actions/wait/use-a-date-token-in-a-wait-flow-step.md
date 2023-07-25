---
unique-page-id: 1146997
description: Utilisation d’un jeton de date dans une étape de flux d’attente - Documents Marketo - Documentation du produit
title: Utilisation d’un jeton de date dans une étape de flux d’attente
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Utilisation d’un jeton de date dans une étape de flux d’attente {#use-a-date-token-in-a-wait-flow-step}

Vous pouvez utiliser l’étape Flux d’attente pour suspendre le parcours d’une personne au cours d’une campagne dynamique jusqu’à une date spécifique qui utilise un jeton de date. Vous pouvez également modifier la date de fin d’un certain nombre de jours.

>[!NOTE]
>
>Cela s’applique uniquement au déclenchement de campagnes. Vous ne pouvez pas utiliser cette fonctionnalité dans les campagnes par lots.

1. Dans votre campagne dynamique **Flux** , faites glisser sur l’onglet **Attente** étape de flux.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Cliquez sur l’icône d’engrenage à droite.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Dans la **Type** menu déroulant, sélectionnez **Jeton de date**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Sélectionnez un jeton Date pour indiquer à quel moment l’étape d’attente doit se terminer :

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Cochez la case pour attendre le prochain anniversaire de la date se produisant dans l’année civile en cours ou l’année suivante.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Utilisez cette option sur les jetons de date qui font référence à des dates antérieures, telles qu’un anniversaire ou la date de début du contrat.

1. Vous pouvez éventuellement modifier la date de fin d’un nombre spécifié de jours.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Vous pouvez également spécifier le nombre de jours à l’aide d’une `{{lead.` ou `{{company.` jeton représentant un champ entier ou un `{{my.` jeton de type nombre.

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Utilisation d’une durée dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [Utilisation d’une date spécifique dans une étape de flux d’attente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
