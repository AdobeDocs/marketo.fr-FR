---
unique-page-id: 1147017
description: Créer une tâche - Documents Marketo - Documentation du produit
title: Créer une tâche
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Créer une tâche {#create-task}

En tant que marketeur, vous disposez d’informations qui peuvent vous aider à conclure des transactions. Vous pouvez créer des tâches pour leur indiquer ce qu’ils doivent faire et quand ils doivent le faire.

![](assets/image2014-9-22-14-3a54-3a46.png)

>[!NOTE]
>
>Lorsque l’utilisateur de synchronisation Marketo crée des tâches, **[!UICONTROL Échéance dans]** est un champ obligatoire pour que la tâche soit créée dans Salesforce. Marketo saisit cinq jours par défaut s’il n’y a aucune valeur.

Par défaut, l’étape de flux se présente comme suit :

![](assets/image2014-9-22-14-3a54-3a49.png)

Personnalisez tous les champs pour créer la tâche comme vous le souhaitez.

![](assets/image2014-9-22-14-3a54-3a52.png)

>[!TIP]
>
>Vous pouvez utiliser `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` et `{{system.tokens}}` dans le **[!UICONTROL Objet]** et **[!UICONTROL Description]**. Voir [Jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} pour plus d’informations.
