---
unique-page-id: 37356429
description: Créer une tâche dans Microsoft - Documents Marketo - Documentation du produit
title: Créer une tâche dans Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Créer une tâche dans Microsoft {#create-task-in-microsoft}

En tant que marketeur, vous disposez d’informations qui peuvent vous aider à conclure des transactions. Vous pouvez créer des tâches pour leur indiquer ce qu’ils doivent faire et quand ils doivent le faire.

Créer une tâche dans Microsoft crée une tâche sous Activités liées à la personne (prospect ou contact) dans [!DNL Microsoft].

>[!NOTE]
>
>Cette étape de flux _ne fonctionne que lorsqu’elle est utilisée avec des déclencheurs_, et non des filtres, dans votre campagne dynamique.

Par défaut, l’étape de flux se présente comme suit :

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Lorsque l’utilisateur de synchronisation Marketo crée des tâches, **[!UICONTROL Échéance dans]** est un champ obligatoire pour que la tâche soit créée dans [!DNL Microsoft]. Marketo saisit cinq jours par défaut si aucune valeur n’est saisie.

Personnalisez tous les champs pour créer la tâche comme vous le souhaitez.

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>Le champ &quot;Status&quot; spécifié pour la tâche dans l’action de flux met à jour le champ : &quot;Status Reason&quot; dans [!DNL Microsoft].

>[!TIP]
>
>Vous pouvez utiliser `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` et `{{system.tokens}}` dans les **[!UICONTROL Sujet]** et **[!UICONTROL Description]**. Pour plus d’informations, voir [Jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} .
