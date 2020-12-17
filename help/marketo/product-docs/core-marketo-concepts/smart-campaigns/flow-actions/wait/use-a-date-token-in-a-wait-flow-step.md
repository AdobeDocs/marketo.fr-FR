---
unique-page-id: 1146997
description: Utiliser un jeton de date dans une étape de flux d'attente - Documents marketing - Documentation du produit
title: Utilisation d’un jeton de date dans une étape de flux d’attente
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Utiliser un jeton de date dans une étape de flux d&#39;attente {#use-a-date-token-in-a-wait-flow-step}

Vous pouvez utiliser l’étape de flux d’attente pour interrompre le parcours d’une personne au cours d’une campagne dynamique jusqu’à une date particulière qui utilise un jeton de date. Vous pouvez également modifier la date de fin d’un certain nombre de jours.

>[!NOTE]
>
>Cela s’applique uniquement aux campagnes déclencheuses. Vous ne pouvez pas utiliser cette fonction dans les campagnes par lots.

1. Dans l’onglet de votre campagne dynamique **Flux**, faites glisser la souris sur l’étape de flux **Attendre**.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Cliquez sur l&#39;icône d&#39;engrenage à droite.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Dans la liste déroulante **Type**, sélectionnez **Jeton de date**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Choisissez un jeton Date pour indiquer à quel moment l’étape d’attente doit se terminer :

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Pour attendre le prochain anniversaire de la date se produisant au cours de l’année civile en cours ou de l’année civile suivante, cochez la case.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Utilisez cette option sur les jetons de date qui font référence à des dates antérieures, telles qu’une date d’anniversaire ou de début du contrat.

1. Vous pouvez éventuellement modifier la date de fin selon un nombre de jours spécifié.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Vous pouvez également spécifier le nombre de jours à l’aide d’un jeton `{{lead.` ou `{{company.` qui représente un champ entier ou d’un jeton `{{my.` de type nombre.

1. Cliquez sur Enregistrer.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!NOTE]
   >
   >**Articles connexes**
   >
   >* [Utilisation d’une durée dans une étape de flux d’attente](use-a-duration-in-a-wait-flow-step.md)
   >* [Utilisation d’une date spécifique dans une étape de flux d’attente](use-a-specific-date-in-a-wait-flow-step.md)


