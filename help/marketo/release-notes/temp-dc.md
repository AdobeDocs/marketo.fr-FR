---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour de Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 7fbfdc6d34d2f1174e921464d64689b0c5687914
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 3%

---

# Notes de mise à jour du Dynamic Chat TEMP {#dynamic-chat-release}

## Version de septembre/octobre 2024 {#august-release}

### Amélioration de l’analyse des conversations en direct {#enhanced-live-chat-analytics}

Plusieurs améliorations ont été apportées au tableau de bord Analytics, notamment :

* Nombre total de discussions en direct demandées : nombre de visiteurs ayant demandé une &quot;discussion avec l’agent&quot;

* Total des tchats en direct connectés : nombre de visiteurs connectés par rapport au total demandé pour une &quot;conversation avec l’agent&quot;

* Nombre total de demandes de messagerie instantanée manquantes : nombre de visiteurs sans assistance par rapport au total demandé pour une &quot;conversation avec l’agent&quot;

* Durée moyenne de la conversation en minutes : analyse de la &quot;durée moyenne de la conversation&quot; entre les visiteurs et vos agents

* Temps moyen de réponse de l’agent en secondes : analysez le &quot;temps moyen&quot; pris par les agents pour répondre à leurs questions et réponses sur le chat en direct.

* Tableau de bord quotidien : demandes de chat en direct connectées correctement, demandes de chat en direct non exécutées, tri et filtrage des activités de chat en direct récentes

CAPTURE D’ÉCRAN

### Score de conversation {#conversation-scoring}

Quantifiez vos pistes en fonction de la qualité de leur interaction de conversation et utilisez cette mesure comme déclencheur/filtre dans les campagnes dynamiques de Marketo Engage. Utilisez le nouvel attribut _score de conversation_ sur les activités suivantes :

* Engagé dans un dialogue
* Engagé avec un flux de conversation
* Engagé avec un agent

**Choses à noter :**

* La valeur de score sera comprise entre 0, 1, 2 et 3 (la valeur par défaut est nulle).

* Une fois la conversation terminée ou supprimée, enregistrez dans l’activité la valeur de notation et publiez qu’elle ne peut pas être modifiée????? (que signifie cette phrase ?)

* Définir un score :

   * Dans la boîte de réception de l’agent : au cours d’une conversation en direct, l’agent peut mettre à jour ou définir un score pour la conversation, qui est stocké dans l’activité de conversation.

   * Dans le concepteur de flux, dans la carte d’objectif, l’utilisateur peut mettre à jour ou définir un score pour la conversation.

CAPTURE D’ÉCRAN

CAPTURE D’ÉCRAN

CAPTURE D’ÉCRAN

### Nouvelle logique de création de piste {#new-lead-creation-logic}

Si une piste remplit un formulaire avec l’email `abc@test.com` et est cookie comme xyz, puis remplit ensuite le même formulaire avec l’email `def@test.com`, un nouveau prospect est créé, mais le cookie xyz devient associé à la nouvelle piste et supprimé de la piste `abc@test.com`.

À partir de ce moment, `abc@test.com` sera une piste sans cookie. LEAD ANONYME??

Ainsi, lorsqu’un visiteur avec cookie abc arrive sur une page et fournit un ID de courrier électronique sous la forme `abc@p.com` :

TABLE

### Optimisation du temps de chargement du flux de conversation {#optimized-conversation-flow-load-time}

Pour améliorer l’expérience utilisateur, un chargeur de minuteur s’affiche maintenant au lieu d’un espace vide pendant le chargement du flux de conversation. CONVERSATION OU CONVERSATION???

**Avant**

GIF

**After**

GIF

### Option d’héritage de la police {#option-to-inherit-font}

Vous pouvez désormais activer le chatterbot pour qu’il hérite directement de la police de la page web où il est hébergé plutôt que de gérer la police de marque dans Dynamic Chat. Lorsque vous activez cette option, le chatterbot prend la police définie sur la balise `<body>` de la page.

CAPTURE D’ÉCRAN

### Intégration de Demandbase avec Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Les utilisateurs de Demandbase peuvent apporter leur propre licence Demandbase et activer l’intégration. Utilisez les attributs de personne Demandbase pour le ciblage de dialogue, la valorisation de marque conditionnelle et le routage personnalisé.

La résolution de ces valeurs d’attribut par rapport à une piste serait effectuée en temps réel et est stockée dans le profil de piste respectif.
