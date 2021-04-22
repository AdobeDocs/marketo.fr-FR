---
unique-page-id: 2360217
description: Modifier les paramètres d’attribution pour Analytics - Documents Marketo - Documentation du produit
title: Modification des paramètres d’attribution pour Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Modifier les paramètres d’attribution pour Analytics {#change-attribution-settings-for-analytics}

Vous pouvez modifier la manière dont Marketo associe les contacts aux opportunités d’attribution Première touche et Multipoint, aux mesures de conversion des pistes et à l’indicateur d’opportunité influencé par le marketing.

Ces paramètres auront un impact sur les rapports de l&#39;Explorateur de recettes sous [Analyse d&#39;opportunité de Programme](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Analyse d&#39;opportunité](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) et les zones d&#39;Analyse de piste. Cela aura également une incidence sur le rapport Analyseur de Programme.

1. Sous la section **Admin**, cliquez sur **Analyses du cycle des recettes**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Cliquez sur le lien **Modifier** sous **Attribution**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >La modification de ce paramètre ne modifie aucune donnée Marketo ; cela change simplement la façon dont vos rapports s&#39;exécutent. Cela peut être annulé à tout moment.

1. Sélectionnez une option et cliquez sur **Enregistrer**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >**Explicite** : Seuls les contacts avec des rôles (par défaut).
   >
   >**Hybride** : Contacts avec des rôles si disponibles. Si aucun n&#39;est disponible, il utilise tous les contacts dans les comptes.
   >
   >**Implicite** : Tous les contacts, quel que soit leur rôle.

>[!CAUTION]
>
>Lorsque vous utilisez **Implicit**, Marketo examine toujours tous les contacts associés au compte, quel que soit le rôle. **Marketo recommande vivement d’utiliser le mode** explicite. L&#39;utilisation d&#39;Implicite peut créer des faux positifs ; c&#39;est-à-dire les gens qui ont le mérite d&#39;avoir une opportunité, même s&#39;ils n&#39;ont aucune réelle influence sur cette opportunité. Utilisez Implicit avec précaution.
