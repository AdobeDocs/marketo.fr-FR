---
unique-page-id: 1147017
description: Découvrez comment créer une tâche Salesforce dans une étape de flux. Créez une tâche pour le propriétaire du prospect lorsqu’un utilisateur accède au flux.
title: Créer une tâche
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/RJ5nZrVvURtgXEWWZwL2xXzlYOhWjKGSbX-MFTWCwzg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 130
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
