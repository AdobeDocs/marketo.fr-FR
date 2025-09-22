---
unique-page-id: 1147017
description: Créer Une Tâche - Documents Marketo - Documentation Du Produit
title: Créer une tâche
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Créer une tâche {#create-task}

En tant que spécialiste marketing, vous disposez d’informations qui peuvent aider les ventes à conclure des offres. Vous pouvez créer des tâches pour leur indiquer ce qu’elles doivent faire et quand elles doivent le faire.

![](assets/create-task-1.png)

>[!NOTE]
>
>Lorsque l’utilisateur de la synchronisation Marketo crée des tâches, le champ **[!UICONTROL Échéance en cours]** est obligatoire pour que la tâche soit créée dans Salesforce. Marketo saisit cinq jours par défaut s’il n’existe aucune valeur.

Par défaut, l’étape de flux se présente comme suit :

![](assets/create-task-2.png)

Personnalisez tous les champs pour créer la tâche comme vous le souhaitez.

![](assets/create-task-3.png)

>[!TIP]
>
>Vous pouvez utiliser `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` et `{{system.tokens}}` dans les **[!UICONTROL Objet]** et **[!UICONTROL Description]**. Voir [Jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} pour plus d’informations.
