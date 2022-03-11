---
description: Remplacement de priorité pour les campagnes de déclenchement - Documents Marketo - Documentation du produit
title: Remplacement de priorité pour les campagnes de déclenchement
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
source-git-commit: 48a49faa6a1fde1e9ac391c2bf0800123f6a5bac
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Remplacement de priorité pour les campagnes de déclenchement {#priority-override-for-trigger-campaigns}

Les administrateurs peuvent remplacer la priorité déterminée de Marketo pour déclencher des campagnes afin de définir des priorités qui s’alignent mieux sur les objectifs de l’entreprise.

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que pour les campagnes de déclenchement et pour les utilisateurs qui ont reçu l’autorisation [Autorisation &quot;Modifier la priorité de la campagne du déclencheur&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>Il est vivement conseillé d’utiliser cette fonctionnalité sur un ensemble limité de campagnes critiques de l’entreprise (25 est le maximum recommandé). L’utilisation de la fonction sur un ensemble volumineux peut avoir un impact négatif sur l’exécution globale de la campagne.

## Accorder l’accès de priorité de remplacement {#grant-priority-override-access}

>[!NOTE]
>
>Seuls les administrateurs ou les utilisateurs avec des responsabilités d’administrateur doivent disposer d’un accès de priorité de campagne de remplacement.

1. Dans le [!UICONTROL Administration] zone, cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Cliquez sur le bouton **[!UICONTROL Rôles]** , sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès, puis cliquez sur **[!UICONTROL Modifier le rôle]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. Sous [!UICONTROL Accès aux activités marketing], sélectionnez **[!UICONTROL Modifier la priorité de la campagne de déclenchement]**. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Annuler la priorité  {#override-priority}

1. Localisez votre campagne de déclenchement. Cliquez dessus avec le bouton droit et sélectionnez **[!UICONTROL Remplacer la priorité de la campagne]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Cliquez sur le bouton **[!UICONTROL Remplacer la priorité de la campagne]** curseur à activer. Sélectionnez un nouveau niveau de priorité et cliquez sur **[!UICONTROL Confirmer]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   Le nouveau niveau de priorité s’affiche dans l’onglet Planning .

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Vous pouvez afficher la priorité par défaut de votre campagne dans la [!UICONTROL File d’attente de campagne] under [!UICONTROL Activités marketing]. Pour augmenter le taux d&#39;exécution, nous vous recommandons de définir la priorité de votre campagne à un niveau supérieur à son niveau par défaut.
>* La priorité définie par l’utilisateur s’applique uniquement aux nouvelles personnes qui remplissent les critères de la campagne. les personnes déjà en file d’attente ne seront pas affectées.
>* Les remplacements de priorité sont capturés dans [Journal d’audit](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md).

