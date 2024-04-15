---
description: Notes de mise à jour du Dynamic Chat - Documents Marketo - Documentation du produit
title: Notes de mise à jour de Dynamic Chat
hide: true
hidefromtoc: true
feature: Release Information, Dynamic Chat
source-git-commit: c2c95f36c710ba7a9ac75c2160c72e44b5f81a99
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 1%

---

# Notes de mise à jour : avril 2024 {#release-notes-apr-24}

Les versions d’Adobe Dynamic Chat fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive du déploiement des fonctionnalités. Parfois, il existe plusieurs versions en un mois. Par conséquent, veuillez consulter régulièrement les informations les plus récentes.

Page des notes de mise à jour standard pour Marketo Engage [peut être consulté ici](/help/marketo/release-notes/current.md){target="_blank"}.

## Publication d’avril {#april-release}

**Date de publication : 16 avril 2024**

### Flux de conversation désormais disponibles pour les clients sur Sélectionner un module {#conversational-flows-select-package}

Lorsque nous avons lancé Conversational Flows l’an dernier, les clients du package Dynamic Chat Select ne pouvaient tirer parti de cette fonctionnalité qu’en testant 100 engagements de durée de vie. Désormais, les flux de conversation sont entièrement disponibles pour tous les clients du module Sélectionner .

Les engagements Flux de conversation vont être comptabilisés dans la limite mensuelle de 250 conversations en cours pour les clients sur le package Sélectionner .

### Fonctions de rappel {#callback-functions}

Les fonctions de rappel vous permettent de collecter des événements d’analyse de Dynamic Chat dans des systèmes externes, tels qu’Adobe Analytics ou les Google Analytics, lorsque les visiteurs interagissent avec des conversations de Dynamic Chat. Vous activez les événements Dynamic Chat Analytics en enregistrant un rappel avec l’API pour écouter les événements. Cela vous permet d’avoir une vision plus globale de votre engagement Dynamic Chat en ce qui concerne d’autres données clés, telles que le trafic web.

### Conditions de disponibilité de l’agent en direct ajoutées à l’embranchement conditionnel {#live-agent-availability-conditional-branching}

Outre les champs Marketo natifs et personnalisés, vous pouvez désormais utiliser un embranchement conditionnel pour créer des branches en fonction de la disponibilité de l’agent. Cela s’avère utile si vous souhaitez offrir aux visiteurs la possibilité de parler avec un agent en direct uniquement lorsque des agents en direct sont disponibles.

CAPTURE D’ÉCRAN

### Condition de liste dynamique ajoutée à un embranchement conditionnel {#smart-list-condition}

Avec l’ajout de la nouvelle condition Liste dynamique des Marketo Engage dans l’embranchement conditionnel, vous pouvez créer des branches d’après les audiences préexistantes que vous avez déjà créées dans Marketo plutôt que de définir les conditions d’embranchement des audiences dans Dynamic Chat.

CAPTURE D’ÉCRAN

### Branchement conditionnel pour les flux de conversation {#conditional-branching-for-conversational-flows}

Nous avons publié un embranchement conditionnel pour les Dialogues plus tôt cette année et vous pouvez maintenant également profiter de l’embranchement conditionnel dans les flux de conversation ! L’embranchement conditionnel vous permet de créer des branches dans votre flux en fonction de différentes conditions.

### Chat en direct pour les flux de conversation {#live-chat-for-conversational-flows}

Nous avons lancé l’année dernière la fonctionnalité de chat en direct pour les boîtes de dialogue. Vous pouvez désormais ajouter des engagements de chat en direct à vos flux de conversation. Si vous utilisez des flux de conversation avec vos formulaires Marketo, vous pouvez désormais autoriser les visiteurs qualifiés à discuter avec un agent en direct immédiatement après l’envoi du formulaire.

### Activités Marketo Engage récentes dans la boîte de réception de l’agent {#recent-marketo-engage-activities-in-agent-inbox}

Nous avons ajouté des activités de Marketo Engage récentes à la section Activités récentes de la boîte de réception de l’agent de sorte que lorsqu’un visiteur du site demande à discuter avec un agent, l’agent peut facilement voir si le visiteur s’est récemment engagé dans l’une des activités Marketo suivantes (les 25 dernières activités) :

* E-mail ouvert
* Page web visitée
* Formulaire rempli
* A vécu un moment intéressant

CAPTURE D’ÉCRAN

### État de connexion au calendrier dans la gestion des agents {#calendar-connection-status-in-agent-management}

Les administrateurs peuvent désormais facilement identifier les agents disposant d’autorisations de réservation de réunions ayant connecté leurs calendriers en Dynamic Chat. Cela vous permet de vous assurer que l’équipe commerciale entière est connectée et prête à accepter les demandes de réunion de Dynamic Chat.

CAPTURE D’ÉCRAN

### Paramètre d’avertissement minimal dans la configuration du calendrier de l’agent {#minimum-notice-setting-in-agent-calendar-configuration}

Les clients ont signalé que les visiteurs web réservaient des réunions sur leur calendrier avec un préavis d’au moins 10 minutes. Nous avons donc ajouté un paramètre d’avertissement minimum dans la configuration du calendrier de l’agent et défini le délai d’avance par défaut sur 24 heures.

CAPTURE D’ÉCRAN

### Nouvelles notifications in-app {#new-in-app-notifications}

Nous avons introduit trois nouvelles notifications in-app pour vous aider à vous tenir informé du statut de votre instance de Dynamic Chat en temps réel.

* Texte
* Texte
* Texte

### Ajout/suppression d’un comportement utilisateur mis à jour {#add-remove-user-behavior-updated}

Certains clients nous informent des problèmes qu’ils rencontraient lors de l’ajout et de la suppression d’agents dans Dynamic chat. Nous avons donc apporté des modifications pour résoudre ces problèmes.

Lorsqu’un utilisateur est ajouté à un Admin Console avec une autorisation de conversation en direct ou de réservation de réunion, il apparaît immédiatement dans la liste Gestion des agents et peut être ajouté aux dialogues, flux de conversation, règles de routage et équipes.

Lorsqu’un utilisateur disposant d’autorisations de réservation de réunions ou de conversation en direct est supprimé du Admin Console, il est immédiatement supprimé du Dynamic Chat, il n’est plus disponible pour les conversations en direct ou le routage de réunions, et il ne sera plus pris en compte dans les limites de licence.

### Amélioration des performances des rapports sur les niveaux de conversation {#improved-conversation-level-report-performance}

Les rapports au niveau du dialogue individuel et du flux de conversation sont désormais plus performants et précis. Auparavant, le chargement des rapports de dialogue pouvait prendre plusieurs secondes et les données étaient parfois incompatibles avec les rapports de performances globaux. Désormais, vos rapports de dialogue individuels se chargeront en un instant et les données seront toujours alignées avec les données de rapport globales.

CAPTURE D’ÉCRAN

### Mises à jour des autorisations {#permission-updates}

Nous avons nettoyé la structure et les noms des autorisations dans Adobe Admin Console afin de rendre la gestion des autorisations plus intuitive.

* La catégorie Gestion des conversations s’appelle désormais Conversations .
* La catégorie Réunions est désormais appelée Activités
* La catégorie Paramètres de l’agent est désormais appelée Agents
* La catégorie Paramètres d’administration est désormais appelée Configuration
* La catégorie Chat en direct a été supprimée et toutes les autorisations de chat en direct ont été déplacées vers la catégorie Agents

CAPTURE D’ÉCRAN

### Prise en charge des hyperliens dans la boîte de réception de l’agent {#support-for-hyperlinks-in-agent-inbox}

Désormais, lorsque les agents de conversation en direct partagent des URL avec les visiteurs de la conversation, ces URL sont liées par un lien hypertexte, de sorte que les visiteurs puissent simplement cliquer dessus pour accéder à la page, plutôt que d’avoir à copier et coller l’URL dans leur navigateur.

### Entrer le comportement clé mis à jour dans la boîte de réception de l’agent {#enter-key-behavior-updated-in-agent-inbox}

Nous avons modifié le comportement de la clé de retour dans la boîte de réception de l’agent afin que l’utilisation de la touche Retour ou Entrée envoie votre message et que l’utilisation de la touche Maj+Entrée crée un saut de ligne.

CAPTURE D’ÉCRAN

### Suppression de la page Round Robin {#round-robin-page-removed}

Ne vous inquiétez pas ! Le routage de la boucle est toujours entièrement fonctionnel et fonctionne de la même manière qu’il l’a toujours été. Nous venons de supprimer la page qui montrait une liste souvent inexacte d&#39;agents et leur ordre dans la file d&#39;attente de routage du robot-rond.

Pour donner un peu de contexte, lorsque nous avons lancé Dynamic Chat en 2022, il n&#39;y avait pas de prise en charge du chat en direct, seulement les réservations de réunions et la page de routage du robin rond a été conçue uniquement en tenant compte des réservations de réunions. Avec l&#39;introduction du chat en direct l&#39;année dernière, la page de braquages en rond est devenue obsolète parce qu&#39;elle ne reflétait pas exactement la nature plus complexe du routage de roquettes en rond entre les agents avec des autorisations de réservation de réunions et de chat en direct. Nous avons exploré plusieurs options pour résoudre ce problème, mais nous avons finalement décidé que le supprimer était la meilleure option pour réduire la confusion.

## Publication de février {#february-release}

**Date de publication : 22 février 2024**

### Page Conversations {#conversations-page}

La nouvelle page Conversations vous offre un guichet unique pour afficher les transcriptions de toutes les conversations (automatisées et en direct) qui se sont produites pour votre instance, à partir de pistes connues et anonymes, ce qui vous permet de mieux comprendre comment vos clients interagissent avec vos boîtes de dialogue, vos flux de conversation et vos agents en direct.

CAPTURE D’ÉCRAN

La période dans le tableau de bord global est passée de 90 jours à 24 mois.

Vous avez demandé et nous avons livré. Vous pouvez désormais afficher les données d’engagement des Dynamic Chat pendant deux ans au maximum dans tous les tableaux de bord Analytics.

### Branchement conditionnel dans les boîtes de dialogue {#conditional-branching-in-dialogues}

L’embranchement conditionnel vous permet de créer des branches dans vos flux de dialogue en fonction de différentes conditions. Vous pouvez désormais présenter un contenu différent à différentes personnes dans le même dialogue en fonction des attributs de prospect et de société dans Marketo.

## Publication de janvier {#january-release}

**Date de publication : 24 janvier 2024**

### Limite concomitante de clics en direct dans la gestion des agents {#Concurrent-live-chat-limit-setting}

Par défaut, chaque agent de chat en direct de votre instance peut participer à un maximum de 5 sessions de chat en direct à la fois. Nous avons introduit un nouveau paramètre dans la gestion des agents qui vous permet d’ajuster cette limite de 1 à 10.

CAPTURE D’ÉCRAN
