---
unique-page-id: 37356429
description: Créer une tâche dans Microsoft - Documents Marketo - Documentation du produit
title: Créer une tâche dans Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 4%

---

# Créer une tâche dans Microsoft {#create-task-in-microsoft}

En tant que spécialiste marketing, vous disposez d’informations qui peuvent aider les ventes à conclure des offres. Vous pouvez créer des tâches pour leur indiquer ce qu’elles doivent faire et quand elles doivent le faire.

Créer une tâche dans Microsoft crée une tâche sous Activités liées à la personne (lead ou contact) dans [!DNL Microsoft].

>[!NOTE]
>
>Cette étape de flux _ne fonctionne qu’avec des déclencheurs_ et non des filtres, dans votre campagne intelligente.

Par défaut, l’étape de flux se présente comme suit :

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Lorsque l’utilisateur de la synchronisation Marketo crée des tâches, le champ **[!UICONTROL Échéance en cours]** est obligatoire pour que la tâche soit créée en [!DNL Microsoft]. Marketo saisit cinq jours par défaut si aucune valeur n’est saisie.

Personnalisez tous les champs pour créer la tâche comme vous le souhaitez.

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>Le champ « Statut » spécifié pour la tâche dans l’action de flux met à jour le champ « Raison du statut » dans [!DNL Microsoft].

>[!TIP]
>
>Vous pouvez utiliser `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` et `{{system.tokens}}` dans les **[!UICONTROL Objet]** et **[!UICONTROL Description]**. Voir [Jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} pour plus d’informations.
