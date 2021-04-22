---
unique-page-id: 1147074
description: Nettoyage Campaign Déclencheur Automatique - Docs Marketo - Documentation du produit
title: Nettoyage des campagnes à déclencheurs automatique
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 3%

---

# Nettoyage des campagnes à déclencheurs automatique {#automatic-trigger-campaign-cleanup}

Marketo dispose d’un service agréable/gratuit pour désactiver les campagnes dynamiques déclenchées qui ne reçoivent plus d’activité. Cela accélère les performances globales du système et vous fait gagner du temps.

## Que se passe-t-il ? {#what-happens}

Une fois par trimestre, Marketo trouvera des campagnes intelligentes qui sont restées en sommeil (pas de personnes) pendant 6 mois ou plus et les désactivera.

## Me préviendras-tu en premier ? {#will-you-notify-me-first}

Bien sûr ! Une fois par trimestre, vous recevrez une notification une semaine à l’avance, indiquant chaque campagne que nous prévoyons de désactiver.

1. Accédez à l&#39;onglet **Notifications**.

   ![](assets/notifications.png)

1. Cliquez sur **Déclenchement inactif du nettoyage Campaign planifié**. Cliquez ensuite sur le lien **Ces campagnes de déclenchement inactif seront désactivées**.

   ![](assets/image2015-4-27-20-3a48-3a35.png)

   Une liste de campagnes actives est prévue pour être désactivée.

   ![](assets/image2015-4-27-20-3a35-3a29.png)

## Quelles campagnes seront désactivées ? {#which-campaigns-will-be-deactivated}

Nous ne désactiverons que les campagnes déclencheurs qui ont été principales depuis plus de 6 mois mais qui n&#39;ont pas eu de critères pour 0 personne au cours de cette période.

## Attendez ! Pas cette campagne ! {#wait-not-this-campaign}

Ne vous inquiétez pas : l&#39;horloge d&#39;une campagne intelligente peut être réinitialisée par :

* Personne remplissant les conditions requises pour la campagne.
* Désactivation et réactivation manuelles de la campagne.

Le compteur de 6 mois est réinitialisé.

## Me direz-vous quelles campagnes ont été désactivées ? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolument : une semaine après la notification initiale, nous désactiverons les campagnes répertoriées (moins celles qui ont qualifié au moins une personne ou ont été désactivées/réactivées) et publierons une notification de confirmation.

1. Sélectionnez la **notification de nettoyage de Campaign Idle Trigger Scheduled**. Cliquez sur le lien **Ces campagnes de déclenchement inactif**.

   ![](assets/image2015-4-27-20-3a56-3a41.png)

1. Une liste de campagnes désactivées s’affiche.

   ![](assets/image2015-4-27-20-3a58-3a38.png)
