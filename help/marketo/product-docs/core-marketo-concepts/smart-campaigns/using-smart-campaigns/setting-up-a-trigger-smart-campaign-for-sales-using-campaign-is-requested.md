---
unique-page-id: 7514898
description: Configuration d’une campagne dynamique de déclenchement pour les ventes à l’aide de "Campaign is Requested" - Documents Marketo - Documentation du produit
title: Configuration d’une campagne dynamique de déclenchement pour les ventes à l’aide de "Campaign is Requested" (Campaign demandé)
exl-id: ed6d7c27-d54b-48e3-af67-19503da4ef56
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Configuration d’une campagne dynamique de déclenchement pour les ventes à l’aide de &quot;Campaign is Requested&quot; (Campaign demandé) {#setting-up-a-trigger-smart-campaign-for-sales-using-campaign-is-requested}

L’une des fonctionnalités les plus intéressantes de Marketo est la possibilité de laisser les vendeurs participer à l’effort marketing. Ils sont en première ligne, interagissant avec les gens. Les représentants commerciaux devraient avoir la capacité d’orienter le marketing dans la bonne direction.

>[!NOTE]
>
>Exemples de campagnes dynamiques à demander :
>
>1. **Préparation à long terme** : lorsqu’ils n’ont pas de budget cette année et que vous voulez simplement rester sur le radar
>1. **Cycle de vente actif** : lorsque le vendeur ne souhaite envoyer aucun message à la personne sauf le sien. (utilisez l’indicateur marketing suspendu pour le désabonner temporairement)
>
>Soyez créatifs ! Qu&#39;est-ce que le vendeur aimerait automatiser ? Demandez-leur et branchez-le !

1. Créez une campagne dynamique.

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-1.png)

1. Recherchez et faites glisser le déclencheur **[!UICONTROL Campaign is Requested]** sur la zone de travail.

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-2.png)

1. Les choix de la source indiquent le type de demande qui sera satisfaite. Pour la fonctionnalité Salesforce, veillez à choisir **[!UICONTROL Sales Insight]**.

   >[!TIP]
   >
   >Les opérateurs sources sont pour la sécurité. Vous pouvez limiter la campagne aux requêtes effectuées uniquement par des sources spécifiques, comme d’autres campagnes dynamiques ou des développeurs. Sélectionnez **[!UICONTROL Is Any]** dans la première zone si vous souhaitez autoriser les requêtes provenant de toutes les sources.
   >
   >_Mémoriser_ : en choisissant Sales Insight, il apparaît comme par magie dans la boîte pour les ventes. Ne le fais pas trop ! Trop d&#39;entre eux seront ignorés.

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-3.png)

C’est un excellent moyen d’étendre votre portée marketing à d’autres départements. Configurez toutes sortes de campagnes pour les automatiser.

>[!TIP]
>
>N’oubliez pas de nommer clairement vos campagnes intelligentes. Ils apparaîtront dans Sales Insight exactement comme vous les nommez.
