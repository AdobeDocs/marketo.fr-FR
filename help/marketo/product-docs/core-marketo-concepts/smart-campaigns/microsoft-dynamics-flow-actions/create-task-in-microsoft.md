---
unique-page-id: 37356429
description: Découvrez comment créer une tâche dans Microsoft Dynamics à partir d’une étape de flux. Créez une tâche pour le propriétaire lorsqu’un utilisateur accède au flux.
title: Créer une tâche dans Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
TQID: https://experienceleague.adobe.com/qQL3O4Vi8ncdlXtk2gvraWzquz3oZx5B-1YWTkwdVac
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
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
