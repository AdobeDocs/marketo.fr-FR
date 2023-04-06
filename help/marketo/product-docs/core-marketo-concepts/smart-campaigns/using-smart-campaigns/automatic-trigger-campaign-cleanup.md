---
unique-page-id: 1147074
description: Nettoyage automatique des campagnes de déclenchement - Documents Marketo - Documentation du produit
title: Nettoyage des campagnes à déclencheurs automatique
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
source-git-commit: 073a136953f1997436396cf3f2c87fdc1a3b9c1d
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 3%

---

# Nettoyage des campagnes à déclencheurs automatique {#automatic-trigger-campaign-cleanup}

Marketo dispose d’un service sympa/gratuit pour désactiver les campagnes intelligentes déclenchées qui ne reçoivent plus d’activité. Cela accélère les performances globales du système et vous permet de gagner du temps.

## Que se passe-t-il ? {#what-happens}

Une fois par trimestre, Marketo trouvera des campagnes intelligentes qui sont restées en sommeil (personne) pendant 6 mois ou plus et les désactivera.

## Me préviendras-tu en premier ? {#will-you-notify-me-first}

Bien sûr ! Une fois par trimestre, vous recevrez une notification une semaine à l’avance indiquant chaque campagne que nous prévoyons de désactiver.

1. Cliquez sur le bouton **Notifications** icône .

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. Cliquez sur **Nettoyage inactif des campagnes de déclenchement planifié**. Cliquez ensuite sur le bouton **Ces campagnes de déclenchement inactives seront désactivées.** lien.

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   Une liste des campagnes intelligentes doit être désactivée.

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## Quelles campagnes seront désactivées ? {#which-campaigns-will-be-deactivated}

Nous ne désactiverons que les campagnes de déclenchement principales depuis plus de 6 mois, mais pour lesquelles aucune personne n’est admissible pendant cette période.

## Attendez ! Pas cette campagne ! {#wait-not-this-campaign}

Ne vous inquiétez pas : l’horloge d’une campagne dynamique peut être réinitialisée en procédant comme suit :

* Personne admissible pour la campagne.
* Désactivation et réactivation manuels de la campagne.

Réinitialise le compteur de 6 mois.

## Me direz-vous quelles campagnes ont été désactivées ? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolument : une semaine après la notification d’origine, nous désactiverons les campagnes répertoriées (moins celles qui ont qualifié au moins une personne ou qui ont été désactivées/réactivées) et publierons une notification de confirmation.

1. Sélectionnez la **Nettoyage inactif des campagnes de déclenchement planifié** notification. Cliquez sur le bouton **Ces campagnes de déclenchement inactives** lien.

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. Une liste des campagnes désactivées s’affiche.

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
