---
description: Autorisations - Documents Marketo - Documentation du produit
title: Autorisations
feature: Dynamic Chat
source-git-commit: 8b2eed5e28c46ea9c467fd25dd732c1654a09bed
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 4%

---

# Autorisations {#permissions}

Il existe cinq profils par défaut avec des autorisations prédéfinies que vous pouvez modifier en Dynamic Chat. Vous pouvez également créer un profil personnalisé avec un ensemble personnalisé d’autorisations. Passons en revue les deux.

## Modifier les autorisations existantes {#edit-existing-permissions}

1. Dans le [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, cliquez sur **Dynamic Chat**.

   ![](assets/permissions-1.png)

1. Dans le **Profils de produit** , sélectionnez le profil à modifier. Dans cet exemple, nous choisissons **Live Agent**.

   ![](assets/permissions-2.png)

1. Cliquez sur le bouton **Autorisations** .

   ![](assets/permissions-3.png)

1. Sélectionnez la zone du profil que vous souhaitez modifier. Dans cet exemple, nous choisissons la messagerie instantanée. Cliquez sur l’icône en forme de crayon.

   ![](assets/permissions-4.png)

1. Les éléments d’autorisation disponibles sont répertoriés à gauche. Vous pouvez choisir d’ajouter les autorisations une par une ou toutes à la fois. Dans cet exemple, il n’y en a qu’un seul disponible, nous ajoutons celui-ci. Cliquez sur le bouton **+** signe.

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >L’activation de l’inclusion automatique ajoute tous les éléments d’autorisation à la liste incluse. Lorsque de nouveaux éléments d’autorisation deviennent disponibles, ils sont automatiquement inclus pour ce profil de produit.

1. Cliquez sur **Enregistrer**.

   ![](assets/permissions-6.png)

Vous pouvez désormais répéter ce processus pour toute autre zone de Dynamic Chat.

![](assets/permissions-7.png)

## Création d’un profil {#create-a-profile}

1. Dans le [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, cliquez sur **Dynamic Chat**.

   ![](assets/permissions-8.png)

1. Dans le **Profils de produit** , cliquez sur **Nouveau profil**.

   ![](assets/permissions-9.png)

1. **Nom** votre profil de produit. Vous pouvez éventuellement lui attribuer un nom d’affichage et/ou une description, et choisir de faire en sorte que les utilisateurs soient informés lorsqu’ils sont ajoutés/supprimés. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/permissions-10.png)

1. Votre nouveau profil apparaîtra dans l’onglet Profils de produit . Sélectionnez-le.

   ![](assets/permissions-11.png)

1. Suivez maintenant les étapes 3 à 6 de la [section ci-dessus](#edit-existing-permissions) pour chaque zone souhaitée.


## Liste des autorisations {#list-of-permissions}

Vous trouverez ci-dessous une liste de toutes les autorisations disponibles pour chaque zone.

<table>
<thead>
  <tr>
    <th>Zone de Dynamic Chat</th>
    <th>Autorisations</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gestion des conversations</td>
    <td><li>Afficher les boîtes de dialogue</li>
    <li>Gérer les boîtes de dialogue (créer, supprimer)</li>
    <li>Publier les boîtes de dialogue</li>
    <li>Afficher les flux de conversation</li>
    <li>Gérer les flux de conversation (créer, supprimer)</li>
    <li>Publier les flux de conversation</li></td>
  </tr>
  <tr>
    <td>Chat en direct</td>
    <td><li>Boîte de réception de l’agent(e)</li>
    <li>Afficher mes conversations</li>
    <li>Afficher toutes les conversations</li>
    <li>Afficher le résumé de la conversation <b>*</b></li>
    <li>Affichage des réponses assistées <b>*</b></li></td>
  </tr>
  <tr>
    <td>Réunions</td>
    <td><li>Gérer toutes les réunions</li>
    <li>Gérer mes réunions</li></td>
  </tr>
  <tr>
    <td>Analytics</td>
    <td><li>Affichage des rapports de performances globales</li>
    <li>Afficher les rapports de tchat en direct</li>
    <li>Afficher les rapports sur les réunions</li>
    <li>Exporter des rapports</li></td>
  </tr>
  <tr>
    <td>Paramètres de l’agent</td>
    <td><li>Gérer la disponibilité de la messagerie instantanée</li>
    <li>Connexion à votre calendrier</li>
    <li>Gestion de la disponibilité du calendrier</li></td>
  </tr>
  <tr>
    <td>Paramètres d’administration</td>
    <td><li>Affichage des espaces de travail <b>*</b></li>
    <li>Gérer les espaces de travail (créer, modifier, supprimer) <b>*</b></li>
    <li>Affichage d’un tour</li>
    <li>Afficher des règles personnalisées</li>
    <li>Gestion des règles personnalisées (ajout, modification, suppression)</li>
    <li>Afficher la liste des comptes <b>*</b></li>
    <li>Gestion des comptes (ajout, modification, suppression) <b>*</b></li>
    <li>Gestion des paramètres de Chatbot</li>
    <li>Gérer les paramètres de flux de conversation</li>
    <li>Gérer la confidentialité et la sécurité</li>
    <li>Gestion des intégrations</li>
    <li>Gérer les langues <b>*</b></li>
    <li>Gestion des agents</li>
    <li>Affichage des équipes d’agents <b>*</b></li>
    <li>Gérer les équipes d’agents (ajout, modification, suppression) <b>*</b></li>
    <li>Afficher les limites d’utilisation</li></td>
  </tr>
</tbody>
</table>

**&#42;** Actuellement disponible uniquement pour les utilisateurs de Dynamic Prime
