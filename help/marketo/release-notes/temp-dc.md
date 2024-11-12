---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour de Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: 342d52439a21668a3bf94e5149710b20e4ddb83f
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 4%

---

# Notes de mise à jour du Dynamic Chat TEMP {#dynamic-chat-release}

## Version de septembre/octobre 2024 {#august-release}

### Amélioration de l’analyse des conversations en direct {#enhanced-live-chat-analytics}

Plusieurs améliorations ont été apportées au tableau de bord Analytics, notamment :

* Nombre total de discussions en direct demandées : nombre de visiteurs ayant demandé un &quot;tchat avec agent&quot;

* Total des conversations en direct connectées : nombre de visiteurs connectés par rapport au total demandé pour une &quot;conversation avec un agent&quot;.

* Nombre total de demandes de messagerie instantanée manquantes : nombre de visiteurs sans assistance par rapport au total demandé pour une &quot;conversation avec un agent&quot;.

* Durée moyenne de la conversation en minutes : analyse de la &quot;durée moyenne de la conversation&quot; entre les visiteurs et vos agents

* Temps moyen de réponse de l’agent en secondes : analysez le &quot;temps moyen&quot; pris par les agents pour répondre à leurs questions et réponses sur le chat en direct.

* Tableau de bord quotidien : demandes de chat en direct connectées correctement, demandes de chat en direct non exécutées, tri et filtrage des activités de chat en direct récentes

CAPTURE D’ÉCRAN

### Score de conversation

Quantifiez vos pistes en fonction de la qualité de leur interaction de conversation et utilisez cette mesure comme déclencheur/filtre dans les campagnes dynamiques de Marketo Engage. Utilisez le nouvel attribut _score de conversation_ sur les activités suivantes :

* Engagé dans un dialogue
* Engagé avec un flux de conversation
* Engagé avec un agent

**Choses à noter :**

* La valeur de score sera comprise entre 0, 1, 2 et 3 (la valeur par défaut est nulle).

* Une fois la conversation terminée ou supprimée, enregistrez dans l’activité la valeur de notation et publiez qu’elle ne peut pas être modifiée???????????????????????????????? (qu’est-ce que cela signifie)

* Définir un score :

   * Dans la boîte de réception de l’agent : au cours d’une conversation en direct, l’agent peut mettre à jour ou définir un score pour la conversation, qui est stocké dans l’activité de conversation.

   * Dans le concepteur de flux, dans la carte d’objectif, l’utilisateur peut mettre à jour ou définir un score pour la conversation.

CAPTURE D’ÉCRAN

CAPTURE D’ÉCRAN

CAPTURE D’ÉCRAN

### Nouvelle logique de création de piste {#new-lead-creation-logic}

Si une piste remplit un formulaire avec l’email `abc@test.com` et est cookie comme xyz, puis remplit ensuite le même formulaire avec l’email `def@test.com`, un nouveau prospect est créé, mais le cookie xyz devient associé à la nouvelle piste et supprimé de la piste `abc@test.com`.

À partir de ce moment, `abc@test.com` sera une piste sans cookie. ANON LEAD??

Ainsi, lorsqu’un visiteur avec cookie abc arrive sur une page et fournit un ID de courrier électronique sous la forme `abc@p.com` :

TABLE
