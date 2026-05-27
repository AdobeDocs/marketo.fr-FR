---
unique-page-id: 1147074
description: En savoir plus sur le nettoyage automatique des campagnes de déclenchement. Découvrez comment Marketo nettoie les anciennes exécutions de campagnes de déclenchement.
title: Nettoyage automatique des campagnes à déclencheur
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/KygJNZIAwzO7OzNBHiVwXAylH7mRg31v-bPII53SFD8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 3%

---

# Nettoyage automatique des campagnes à déclencheur {#automatic-trigger-campaign-cleanup}

Marketo propose un service gratuit permettant de désactiver les campagnes intelligentes déclenchées qui n’obtiennent plus d’activité. Cela permet d’accélérer les performances globales du système et de gagner du temps.

## Que se passe-t-il ? {#what-happens}

Une fois par trimestre, Marketo trouve les campagnes intelligentes qui sont restées inactives (aucune personne) pendant 6 mois ou plus et les désactive.

## Me préviendrez-vous d&#39;abord ? {#will-you-notify-me-first}

Bien sûr ! Une fois par trimestre, vous recevrez une notification une semaine à l’avance indiquant chaque campagne que nous prévoyons de désactiver.

1. Cliquez sur l’icône **[!UICONTROL Notifications]**.

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. Cliquez sur **[!UICONTROL Nettoyage de la campagne du déclencheur inactif planifié]**. Cliquez ensuite sur le lien **[!UICONTROL Ces campagnes de déclenchement inactives seront désactivées]**.

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   Une liste des campagnes intelligentes planifiées pour être désactivées s’affiche.

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## Quelles campagnes seront désactivées ? {#which-campaigns-will-be-deactivated}

Nous désactiverons uniquement les campagnes de déclenchement qui sont actives depuis plus de 6 mois, mais pour lesquelles 0 personne est éligible au cours de cette période.

## Attendez ! Pas cette campagne ! {#wait-not-this-campaign}

Ne vous inquiétez pas : l’horloge d’une campagne intelligente peut être réinitialisée en procédant comme suit :

* Personne éligible à la campagne.
* Désactivation et réactivation manuelle de la campagne.

Les deux réinitialiseront le compteur de 6 mois.

## Me ferez-vous savoir quelles campagnes ont été désactivées ? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolument : une semaine après la notification d’origine, nous désactiverons les campagnes répertoriées (moins celles qui remplissent les critères d’au moins une personne ou qui ont été désactivées/réactivées) et publierons une notification de confirmation.

1. Sélectionnez la notification **[!UICONTROL Nettoyage de la campagne du déclencheur inactif planifié]** . Cliquez sur le lien **[!UICONTROL Ces campagnes de déclenchement inactives]**.

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. Une liste des campagnes désactivées s’affiche.

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
