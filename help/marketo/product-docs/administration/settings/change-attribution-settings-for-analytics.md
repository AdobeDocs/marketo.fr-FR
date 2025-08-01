---
unique-page-id: 2360217
description: Modification des paramètres d’attribution pour Analytics - Documents Marketo - Documentation du produit
title: Modification des paramètres d’attribution dans Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Modification des paramètres d’attribution dans Analytics {#change-attribution-settings-for-analytics}

Vous pouvez modifier la manière dont Marketo lie les contacts aux opportunités d’attribution première touche et multitouche, aux mesures de conversion des prospects et à l’indicateur d’opportunité influencé par le marketing.

Ces paramètres auront un impact sur les rapports [!UICONTROL Explorateur de revenus] dans les zones [Analyse des opportunités du programme](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Analyse des opportunités](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) et Analyse des prospects. Cela affectera également le rapport [!UICONTROL  Analyseur de programmes ].

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Cliquez sur **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Cliquez sur le lien **[!UICONTROL Modifier]** sous **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >La modification de ce paramètre ne modifie aucune donnée Marketo ; elle modifie simplement la manière dont vos rapports s’exécutent. Cette opération peut être annulée à tout moment.

1. Sélectionnez une option et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >**[!UICONTROL Explicite]** : contacts avec des rôles uniquement (par défaut).
   >
   >**[!UICONTROL Hybride]** : contacts avec des rôles, le cas échéant. Si aucun contact n’est disponible, il utilise tous les contacts des comptes.
   >
   >**[!UICONTROL Implicite]** : tous les contacts, quel que soit leur rôle.

>[!CAUTION]
>
>Lors de l’utilisation de **[!UICONTROL Implicite]**, Marketo examine toujours tous les contacts associés au compte, quel que soit le rôle. **Marketo recommande vivement d&#39;utiliser le mode [!UICONTROL Explicit]**. L’utilisation de [!UICONTROL Implicite] peut créer des faux positifs, c’est-à-dire des personnes qui ont du crédit pour une opportunité alors qu’elles n’ont aucune influence réelle sur celle-ci. Utilisez [!UICONTROL Implicite] avec précaution.
