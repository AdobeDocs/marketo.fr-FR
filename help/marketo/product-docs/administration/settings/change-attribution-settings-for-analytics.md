---
unique-page-id: 2360217
description: Modification des paramètres d’attribution pour Analytics - Documents Marketo - Documentation du produit
title: Modification des paramètres d’attribution pour Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Modification des paramètres d’attribution pour Analytics {#change-attribution-settings-for-analytics}

Vous pouvez modifier la manière dont Marketo lie les contacts aux opportunités pour l’attribution Première touche et multipoint, les mesures de conversion de prospect et l’indicateur d’opportunité influencé par le marketing.

Ces paramètres auront un impact sur les rapports de l’Explorateur des recettes sous [Analyse des opportunités de programme](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Analyse des opportunités](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md), et les zones Analyse des pistes . Cela aura également une incidence sur le rapport Analyseur de programme.

1. Sous , **Administration** , cliquez sur **Analyse du cycle des recettes**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Cliquez sur le bouton **Modifier** lien sous **Attribution**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >La modification de ce paramètre ne modifie aucune donnée Marketo ; cela modifie simplement la manière dont vos rapports s’exécutent. Cette opération peut être annulée à tout moment.

1. Sélectionnez une option et cliquez sur **Enregistrer**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >**Explicite**: Seuls les contacts avec des rôles (par défaut).
   >
   >**Hybride**: Contacts avec des rôles, le cas échéant. Si aucun contact n’est disponible, il utilise tous les contacts des comptes.
   >
   >**Implicite**: Tous les contacts, quel que soit leur rôle.

>[!CAUTION]
>
>Lors de l’utilisation de **Implicite**, Marketo examinera toujours tous les contacts associés au compte, quel que soit leur rôle. **Marketo recommande vivement d’utiliser le mode Explicite .**. L’utilisation d’Implicite peut créer des faux positifs ; c&#39;est-à-dire des gens qui ont le mérite d&#39;avoir une opportunité, même s&#39;ils n&#39;ont aucune réelle influence sur l&#39;opportunité. Utilisez Implicit avec précaution.
