---
unique-page-id: 2360217
description: Modification des paramètres d’attribution pour Analytics - Documents Marketo - Documentation du produit
title: Modification des paramètres d’attribution pour Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 3%

---

# Modification des paramètres d’attribution pour Analytics {#change-attribution-settings-for-analytics}

Vous pouvez modifier la manière dont Marketo lie les contacts aux opportunités pour l’attribution Première touche et multipoint, les mesures de conversion de prospect et l’indicateur d’opportunité influencé par le marketing.

Ces paramètres auront un impact [!UICONTROL Explorateur de recettes] rapports sous [Analyse des opportunités de programme](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Analyse des opportunités](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md), et les zones Analyse des pistes . Cela aura également une incidence sur la variable [!UICONTROL Analyseur de programme] rapport.

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Cliquez sur **[!UICONTROL Analyse du cycle des recettes]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Cliquez sur le bouton **[!UICONTROL Modifier]** lien sous **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >La modification de ce paramètre ne modifie aucune donnée Marketo ; cela modifie simplement la manière dont vos rapports s’exécutent. Cette opération peut être annulée à tout moment.

1. Sélectionnez une option et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >**[!UICONTROL Explicite]**: Seuls les contacts avec des rôles (par défaut).
   >
   >**[!UICONTROL Hybride]**: Contacts avec des rôles, le cas échéant. Si aucun contact n’est disponible, il utilise tous les contacts des comptes.
   >
   >**[!UICONTROL Implicite]**: Tous les contacts, quel que soit leur rôle.

>[!CAUTION]
>
>Lors de l’utilisation de **[!UICONTROL Implicite]**, Marketo examinera toujours tous les contacts associés au compte, quel que soit leur rôle. **Marketo recommande vivement d’utiliser [!UICONTROL Explicite] mode**. Utilisation [!UICONTROL Implicite] peut créer des faux positifs ; c&#39;est-à-dire des gens qui ont le mérite d&#39;avoir une opportunité, même s&#39;ils n&#39;ont aucune réelle influence sur l&#39;opportunité. Utilisation [!UICONTROL Implicite] avec prudence.
