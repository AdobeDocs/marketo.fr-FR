---
unique-page-id: 1146974
description: Modification des règles de qualification dans une campagne dynamique - Documents Marketo - Documentation du produit
title: Modification des règles de qualification dans une campagne dynamique
exl-id: 8b016fe4-8caf-4266-9f8f-2b05dae78cff
feature: Smart Campaigns
source-git-commit: fec5219c599c805328d77797d2636e549e489ca5
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Modification des règles de qualification dans une campagne dynamique {#edit-qualification-rules-in-a-smart-campaign}

Les règles de qualification contrôlent le nombre de fois où une personne peut exécuter le flux dans une campagne dynamique. Par défaut, même si une personne déclenche une campagne dynamique plusieurs fois, elle ne sera envoyée qu’une seule fois par le flux. Voici comment modifier ces paramètres.

1. Dans votre campagne dynamique, cliquez sur le bouton **[!UICONTROL Planification]** puis **[!UICONTROL Modifier les paramètres]**.

   ![](assets/edit-qualification-rules-in-a-smart-campaign-1.png)

   >[!TIP]
   >
   >Cliquez également sur **[!UICONTROL Modifier]** à droite de Paramètres de campagne dynamique.

1. Choisissez la fréquence d’exécution de vos personnes dans le flux de campagne dynamique : **[!UICONTROL only]**, **[!UICONTROL à chaque heure]**, ou **une fois tous les # jours**/**semaines**/**months**.

   ![](assets/edit-qualification-rules-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Lorsque vous définissez une règle pour une fois par jour, Marketo la convertit en heures. Par exemple, si vous définissez la règle pour une fois par jour et qu’une personne se qualifie à 22 h le dimanche soir, elle ne peut plus être admissible avant 22 h le lundi soir. Cette logique s’applique également lorsque vous utilisez des semaines ou des mois. Un mois est toujours compté comme 30 jours.

   >[!NOTE]
   >
   >Par défaut, les limites de communication ne sont pas appliquées aux campagnes intelligentes. Découvrez comment [appliquer des limites de communication à une campagne dynamique ;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.md){target="_blank"}.

   >[!NOTE]
   >
   >[Application de limites de communication aux campagnes dynamiques](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.md){target="_blank"}

Mission accomplie ! Vous savez maintenant comment contrôler les règles de qualification dans une campagne dynamique.
