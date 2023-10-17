---
unique-page-id: 37356429
description: Créer une tâche dans Microsoft - Documents Marketo - Documentation du produit
title: Créer une tâche dans Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Créer une tâche dans Microsoft {#create-task-in-microsoft}

En tant que marketeur, vous disposez d’informations qui peuvent vous aider à conclure des transactions. Vous pouvez créer des tâches pour leur indiquer ce qu’ils doivent faire et quand ils doivent le faire.

Créer une tâche dans Microsoft crée une tâche sous Activités liées à la personne (prospect ou contact) dans [!DNL Microsoft].

>[!NOTE]
>
>Cette étape de flux va _fonctionne uniquement lorsqu’il est utilisé avec des déclencheurs_, et non les filtres, dans votre campagne dynamique.

Par défaut, l’étape de flux se présente comme suit :

![](assets/msd1.png)

>[!NOTE]
>
>Lorsque l’utilisateur de synchronisation Marketo crée des tâches, **[!UICONTROL Échéance dans]** est un champ obligatoire pour la tâche à créer dans [!DNL Microsoft]. Marketo saisit cinq jours par défaut si aucune valeur n’est saisie.

Personnalisez tous les champs pour créer la tâche comme vous le souhaitez.

![](assets/msd2.png)

>[!NOTE]
>
>Le champ &quot;État&quot; spécifié pour la tâche dans l’action de flux met à jour le champ : &quot;Raison de l’état&quot; dans [!DNL Microsoft].

>[!TIP]
>
>Vous pouvez utiliser `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` et `{{system.tokens}}` dans le **[!UICONTROL Objet]** et **[!UICONTROL Description]**. Voir [Jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} pour plus d’informations.
