---
unique-page-id: 1146974
description: Découvrez comment modifier les règles de qualification dans une campagne dynamique. Modifier le nombre de fois où les personnes peuvent exécuter la campagne.
title: Modifier les règles de qualification dans une campagne intelligente
exl-id: 8b016fe4-8caf-4266-9f8f-2b05dae78cff
feature: Smart Campaigns
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 7%

---

# Modifier les règles de qualification dans une campagne intelligente {#edit-qualification-rules-in-a-smart-campaign}

Les règles de qualification contrôlent le nombre de fois où une personne peut parcourir le flux dans une campagne dynamique. Par défaut, même si une personne déclenche plusieurs fois une campagne intelligente, elle n’est envoyée qu’une seule fois par le flux.

1. Dans votre campagne dynamique, cliquez sur l’onglet **[!UICONTROL Planning]** puis **[!UICONTROL Modifier les paramètres]**.

   ![](assets/edit-qualification-rules-in-a-smart-campaign-1.png)

   >[!TIP]
   >
   >Vous pouvez également cliquer sur **[!UICONTROL Modifier]** à droite de « Paramètres de campagne intelligente ».

1. Choisissez la fréquence à laquelle exécuter vos salariés via le flux de campagne intelligente : **[!UICONTROL une seule fois]**, **[!UICONTROL à chaque fois]** ou **une fois tous les # jours**/**semaines**/**mois**.

   ![](assets/edit-qualification-rules-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >* Lorsque vous définissez une règle pour une fois par jour, Marketo la convertit en heures. Par exemple, si vous définissez la règle pour une fois par jour et qu’une personne est éligible à 22 h un dimanche soir, elle ne peut pas être à nouveau éligible avant 22 h le lundi soir. Cette logique s’applique également lorsque vous utilisez des semaines ou des mois. Un mois compte toujours comme 30 jours.
   >
   >* Par défaut, les limites de communication ne sont pas appliquées aux campagnes intelligentes . Découvrez comment [appliquer des limites de communication à une campagne intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.md){target="_blank"}.
