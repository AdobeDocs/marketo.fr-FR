---
unique-page-id: 37356429
description: Créer une Tâche dans Microsoft - Documents marketing - Documentation du produit
title: Créer une Tâche dans Microsoft
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---


# Créer une Tâche dans Microsoft {#create-task-in-microsoft}

En tant que spécialiste du marketing, vous disposez d’informations qui peuvent aider les ventes à conclure des affaires. Vous pouvez créer des tâches pour leur indiquer ce qu’ils doivent faire et quand ils doivent le faire.

Créer une Tâche dans Microsoft crée une tâche sous Activités liées à la personne (responsable ou contact) dans Microsoft.

>[!NOTE]
>
>Cette étape de flux ne fonctionne **que si elle est utilisée avec des déclencheurs**, et non avec des filtres, dans votre campagne dynamique.

Par défaut, l’étape de flux se présente comme suit :

![](assets/msd1.png)

>[!NOTE]
>
>Lorsque l&#39;utilisateur de synchronisation de Marketo crée des tâches, **Due In** est un champ obligatoire pour que la tâche soit créée dans Microsoft. Si aucune valeur n’est saisie, Marketo saisit cinq jours par défaut.

Personnalisez tous les champs pour créer la tâche comme vous le souhaitez.

![](assets/msd2.png)

>[!NOTE]
>
>Le champ &quot;État&quot; spécifié pour la tâche dans l’action de flux met à jour le champ : &quot;Motif du statut&quot; dans Microsoft.

>[!TIP]
>
>Vous pouvez utiliser `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` et `{{system.tokens}}` dans **Objet** et **Description**. Voir [Jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) pour plus de détails.
