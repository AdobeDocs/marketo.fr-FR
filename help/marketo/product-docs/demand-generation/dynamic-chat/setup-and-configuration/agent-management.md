---
description: Découvrez la gestion des agents dans Dynamic Chat. Affichez les agents, gérez les équipes, définissez des règles de secours et contrôlez la manière dont les réunions et les discussions en direct sont attribuées.
title: Gestion des agentes et agents
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
TQID: https://experienceleague.adobe.com/WZgOsCc5-8oEKLPhj6ziYMIhrYKHxHjrqhLp73mirSU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 3%

---

# Gestion des agentes et agents {#agent-management}

Dans Gestion des agents, affichez une liste d’agents dans votre instance Dynamic Chat, gérez les équipes et définissez vos règles de secours.

![](assets/agent-management-1.png)

## Agents {#agents}

Cet onglet répertorie tous les agents de votre instance Dynamic Chat et inclut des informations telles que leur nom, leur adresse e-mail, le statut du chat en direct, etc.

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Si un agent récemment ajouté n’apparaît pas ici, deux heures peuvent être nécessaires après son ajout dans l’Admin Console d’Adobe.

## Équipes {#teams}

Les administrateurs peuvent créer des équipes d’agents pour faciliter le routage vers des groupes spécifiques d’agents commerciaux.

>[!AVAILABILITY]
>
>L’accès à Teams nécessite un abonnement à Dynamic Chat Prime. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

![](assets/agent-management-3.png)

### Création d’une équipe {#create-a-team}

1. Cliquez sur **+ Créer une équipe**.

   ![](assets/agent-management-4.png)

1. Donnez un nom à votre équipe.

   ![](assets/agent-management-5.png)

1. Cliquez sur le menu déroulant **Ajouter des agents** et sélectionnez les agents souhaités.

   ![](assets/agent-management-6.png)

1. Cliquez sur **Créer**.

   ![](assets/agent-management-7.png)

## Règles de secours {#fallback-rules}

### Réunion de secours {#meeting-fallback}

Sélectionnez un message standard (système) ou écrivez-en un personnalisé pour que les visiteurs puissent le voir lorsque la réservation de réunion n’est pas disponible.

![](assets/agent-management-8.png)

### Secours de la discussion en direct {#live-chat-fallback}

Sélectionnez un message standard (système) ou écrivez-en un personnalisé pour que les visiteurs puissent le voir lorsque la discussion en direct n’est pas disponible.

![](assets/agent-management-9.png)

>[!NOTE]
>
>* Si vous cochez la case _Inclure l’option de réservation de réunion_, le visiteur du chat aura la possibilité de réserver une réunion lorsqu’aucun agent n’est disponible pour le chat en direct.
>
>* **Pour toutes les règles/équipes personnalisées en tant que carte de conversation en direct** : lors de la recherche d’agents, s’ils ne sont pas disponibles ou ne peuvent pas se connecter, il faudra retourner à la table ronde pour essayer de trouver les « agents disponibles » (tous ceux qui sont disponibles à ce moment, quelle que soit la logique/règle de routage placée dans le flux).

>[!TIP]
>
>Lors de la création d’un message personnalisé, vous pouvez mettre en forme la police, utiliser des liens et même insérer des émoticônes.

## Paramètres {#settings}

### Limite du nombre de Live Chats simultanés {#concurrent-live-chat}

Définissez le nombre de conversations actives simultanées qu’un agent peut prendre à la fois. Peut être compris entre 1 et 10.

![](assets/agent-management-10.png)

### Limite de temps d’attente du visiteur {#visitor-wait-time}

Contrôle la durée maximale pendant laquelle un visiteur attend (en secondes) pour être connecté à un agent en direct avant de recevoir un message de secours. Peut être défini entre 10 et 500 secondes.

![](assets/agent-management-11.png)
