---
description: Remplacement de priorité pour les campagnes de déclenchement - Documents Marketo - Documentation du produit
title: Remplacement de priorité pour les campagnes de déclenchement
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Remplacement de priorité pour les campagnes de déclenchement {#priority-override-for-trigger-campaigns}

Les administrateurs peuvent remplacer la priorité déterminée par le Marketo Engage pour les campagnes de déclenchement afin de définir des priorités qui s’alignent mieux sur les objectifs de l’entreprise.

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement pour les campagnes de déclenchement et pour les utilisateurs qui ont reçu l’autorisation [&quot;Modifier la priorité de la campagne de déclenchement&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>Il est vivement conseillé d’utiliser cette fonctionnalité sur un ensemble limité de campagnes critiques de l’entreprise (25 est le maximum recommandé). L’utilisation de la fonction sur un ensemble volumineux peut avoir un impact négatif sur l’exécution globale de la campagne.

## Accorder l’accès de priorité de remplacement {#grant-priority-override-access}

>[!NOTE]
>
>Seuls les administrateurs ou les utilisateurs avec des responsabilités d’administrateur doivent disposer d’un accès de priorité de campagne de remplacement.

1. Dans la zone [!UICONTROL Admin], cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Cliquez sur l’onglet **[!UICONTROL Rôles]** , sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès, puis cliquez sur **[!UICONTROL Modifier le rôle]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. Sous [!UICONTROL Accéder aux activités marketing], sélectionnez **[!UICONTROL Modifier la priorité de la campagne de déclenchement]**. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Annuler la priorité  {#override-priority}

1. Localisez votre campagne de déclenchement. Cliquez dessus avec le bouton droit de la souris et sélectionnez **[!UICONTROL Remplacer la priorité de la campagne]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Cliquez sur le curseur **[!UICONTROL Remplacer la priorité de la campagne]** pour l’activer. Choisissez un nouveau niveau de priorité et cliquez sur **[!UICONTROL Confirmer]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   Le nouveau niveau de priorité s’affiche dans l’onglet Planning .

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Vous pouvez afficher la priorité par défaut de votre campagne dans la [!UICONTROL file d’attente de campagne] sous [!UICONTROL Activités marketing]. Pour augmenter le taux d&#39;exécution, nous vous recommandons de définir la priorité de votre campagne à un niveau supérieur à son niveau par défaut.
>* La priorité définie par l’utilisateur s’applique uniquement aux nouvelles personnes qui remplissent les critères de la campagne ; les personnes déjà en file d’attente ne seront pas affectées.
>* Les remplacements de priorité sont capturés dans le [journal d’audit](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md){target="_blank"}.
