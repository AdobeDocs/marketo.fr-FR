---
description: Créer une tâche à Veeva - Documents Marketo - Documentation du produit
title: Créer une tâche à Veeva
exl-id: 342e45dd-2038-432d-a6b6-1740c8f0b58e
source-git-commit: dfd0ab50a6d77cf88767cc6fb3fe3f2874e0607b
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Créer une tâche à Veeva {#create-task-in-veeva}

En tant que marketeur, vous disposez d’informations qui peuvent vous aider à conclure des transactions. Vous pouvez créer des tâches pour leur indiquer ce qu’ils doivent faire et quand ils doivent le faire.

![](assets/create-task-in-veeva-1.png)

>[!NOTE]
>
>Lorsque l’utilisateur de synchronisation Marketo crée des tâches, **Échéance dans** est un champ obligatoire pour la tâche à créer à Veeva. Marketo saisit cinq jours par défaut s’il n’y a aucune valeur.

Par défaut, l’étape de flux se présente comme suit :

![](assets/create-task-in-veeva-2.png)

Personnalisez tous les champs pour créer la tâche comme vous le souhaitez.

![](assets/create-task-in-veeva-3.png)

>[!TIP]
>
>Vous pouvez utiliser `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` et `{{system.tokens}}` dans l’ objet et la description. Voir [Jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target=&quot;_blank&quot;} pour plus d’informations.