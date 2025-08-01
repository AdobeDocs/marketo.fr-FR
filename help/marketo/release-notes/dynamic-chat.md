---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour de Dynamic Chat
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '3408'
ht-degree: 2%

---

# Notes de mise à jour de Dynamic Chat {#dynamic-chat-release}

Les versions de Adobe Dynamic Chat fonctionnent sur un modèle de diffusion continu, ce qui permet une approche plus évolutive du déploiement des fonctionnalités. Il arrive qu’il y ait plusieurs versions par mois. N’hésitez pas à vérifier régulièrement pour obtenir les informations les plus récentes.

La page Notes de mise à jour standard de Marketo Engage [se trouve ici](/help/marketo/release-notes/current.md){target="_blank"}.

## Version de juin 2025 {#june-2025-release}

**Date de publication : mardi 30 juin 2025**

### Réorganisation de la logique de routage {#routing-logic-revamp}

Nous avons repensé la logique de routage du chat en direct dans Dynamic Chat pour garantir un comportement d’engagement plus intelligent et plus prévisible pour tous les types de routage (compte, personnalisé, équipe et cycle de rotation). La nouvelle logique simplifie les flux de routage et améliore la gestion de secours lorsque des agents ne sont pas disponibles.

#### Améliorations clés du comportement de routage

* **Jusqu’à deux tentatives d’engagement par session**

   * Le système tente de se connecter à un maximum de deux agents (au plus), mais strictement dans la règle de routage principale.

   * Si un agent est disponible mais ne répond pas (par exemple, refuse ou manque la conversation), le système tentera de se connecter à un agent différent du même pool.

   * La logique de secours (comme la rotation) n’est activée que si aucun agent éligible n’est trouvé lors de la résolution initiale, et non pour réessayer après un échec de l’engagement.

* **Comportement Spécifique Aux Règles De Routage**

##### —Routage de compte—

Si le domaine d’e-mail d’un visiteur est mappé à un compte connu, l’agent mappé est toujours considéré comme prioritaire.

Si l’agent est disponible, le chat leur est directement adressé.

Si l’agent n’est pas disponible, le système :

* Ne tente pas d&#39;utiliser un autre agent, même si Round Robin est activé comme solution de secours.

* Au lieu de cela, il :

   * Affiche le calendrier de réunion de l&#39;agent mappé (si activé),
-ou-
   * Retourne à un message par défaut (au pire des cas).

La règle de routage au niveau de la carte (par exemple, Équipe, Personnalisé) n’est prise en compte que si le routage de compte n’est pas éligible (aucun domaine ou agent correspondant).

##### —Routage personnalisé/d’équipe—

Ces règles peuvent renvoyer plusieurs agents éligibles.

Si le premier agent disponible n&#39;engage pas, le système essaie un autre agent de la même liste.

La solution de secours Round Robin n’est pas déclenchée simplement parce qu’un agent ne répond pas.

Si aucun des agents n’engage :

* Le système affiche le calendrier du premier agent essayé (s&#39;il est activé),
-ou-
* Affiche le message de secours par défaut.

##### —Routage circulaire—

Lorsqu&#39;il est utilisé comme règle de transmission principale, le système :

* Tente d&#39;engager le premier agent disponible à partir du pool circulaire.

* Si le premier agent ne répond pas, il réessaye avec le meilleur agent éligible suivant.

Si la fonction Round Robin est utilisée comme solution de secours, elle s’active uniquement si aucun agent n’est résolu à partir de la règle principale.

##### Flux d’expérience du visiteur

Le système vérifie si le routage de compte est applicable.

* Si oui et que l’agent est disponible, il se connecte immédiatement.

* Si l’agent n’est pas éligible ou indisponible, il passe à la règle de routage au niveau de la carte.

La règle de routage au niveau de la carte (personnalisée, d’équipe, à tour de rôle) est évaluée.

* La disponibilité (autorisations, statut) des agents éligibles est vérifiée.

* Le système engage un agent et, si nécessaire, tente un deuxième agent à partir de la même règle.

* Si aucun engagement ne réussit, une logique de secours est appliquée :

   * Calendrier de secours (si activé),
-ou-
   * Message par défaut.

La solution de secours Round Robin n’est prise en compte que lorsqu’aucun agent éligible n’est trouvé dans la règle de routage principale, et non lorsque des agents individuels ne répondent pas.

##### Cas d’utilisation

<p>

_**Routage de compte**_

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>Le domaine du visiteur est mappé à un compte ; le chat en direct est activé pour l’agent mappé et il est disponible</td>
    <td>La conversation se connecte directement à l’agent mappé</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>L’agent mappé n’est pas disponible, la solution de secours arrondie est activée</td>
    <td>Le système sélectionne un agent disponible par rotation et l’engage </td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>L'agent mappé n'est pas disponible, pas de solution de secours Round Robin ; la réservation de réunion est activée</td>
    <td>Le système affiche le calendrier de l’agent mappé ou affiche un message de secours par défaut</td>
  </tr>
</tbody></table>

_**Routage personnalisé**_

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>La logique personnalisée résout une liste d’agents ; le premier agent est disponible et accepte la conversation.</td>
    <td>La conversation se connecte au premier agent.</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>La règle personnalisée ne résout aucun agent, la fonction de secours Round Robin est activée.</td>
    <td>Le système sélectionne un agent disponible par rotation et l’engage.</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>Deux agents ont été résolus ; aucun d'eux n'accepte la conversation, la solution de secours définie sur le calendrier de réunion.</td>
    <td>Le calendrier de l’agent qui a été essayé pour la première fois s’affiche ou un message de secours par défaut s’affiche.</td>
  </tr>
</tbody></table>

_**Routage de l&#39;équipe**_

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>L’équipe comprend des agents qui utilisent le chat en direct ; le premier agent disponible accepte le chat.</td>
    <td>La conversation se connecte à cet agent.</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>Aucun agent d'équipe n'est disponible et la solution de secours circulaire est activée.</td>
    <td>Le système sélectionne et se connecte à un agent du pool Round Robin.</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>Deux agents disponibles, mais aucun ne s’engage ; calendrier de secours activé.</td>
    <td>Le calendrier de l’agent qui a été tenté pour la première fois s’affiche ou un message de secours est déclenché.</td>
  </tr>
</tbody></table>

_**Routage circulaire**_

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>Round Robin pool a plusieurs agents ; le second agent accepte le chat après le premier ne l'accepte pas.</td>
    <td>La conversation se connecte au second agent.</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>Aucun agent disponible dans le pool Round Robin ; le calendrier des réunions est activé.</td>
    <td>Le calendrier s’affiche pour le premier agent de la liste (s’il est configuré) ou un message de secours s’affiche.</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>Aucun agent disponible ; la solution de secours est désactivée.</td>
    <td>Un message de secours statique s’affiche pour le visiteur.</td>
  </tr>
</tbody></table>

### Notification Pulse {#pulse-notification}

Chaque fois qu’un visiteur demande à se connecter à un agent, nous lui fournissons une notification in-app via le navigateur. Mais parfois, les agents ratent ces conversations.

Avec cette version, l’agent en direct peut obtenir une notification par e-mail, Slack, in-app et par navigateur lorsqu’un nouveau visiteur souhaite discuter.

1. Sur la page d’accueil de Adobe Experience Cloud, cliquez sur l’icône Compte et sélectionnez **Préférences**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Faites défiler jusqu’à _Notifications_ et effectuez vos sélections Dynamic Chat souhaitées.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Le contenu d’une notification Pulse peut être le même que celui que nous utilisons pour les notifications in-app dans le navigateur.

## Version D’Avril/Mai 2025 {#apr-may-25-release}

### Son de notification de message {#message-notification-sound}

Vous avez désormais la possibilité d’activer un son pour le visiteur à chaque fois que le chatbot est déclenché au cours d’une session. Vous avez le choix entre plusieurs sons.

### Activer les messages Poke sur Mobile {#enable-poke-messages-on-mobile}

« Poke », qui affiche la question d’ouverture à côté de l’icône de conversation sans que le visiteur ait à cliquer dessus pour la voir, est désormais une option à activer pour les visiteurs qui utilisent un appareil mobile.

### Mise à jour de secours par défaut {#default-fallback-update}

Pour toute règle personnalisée/équipe en tant que carte de conversation en direct : si aucun agent n’est disponible (ou si le chat ne peut pas se connecter), la carte revient à la case départ à tour de rôle pour les agents disponibles (tous ceux qui sont disponibles à ce moment, quelle que soit la logique/règle de routage placée dans le flux).

### Intégration Demandbase {#demandbase-integration}

Les utilisateurs Demandbase peuvent utiliser les attributs de personne Demandbase pour le ciblage de boîte de dialogue, le branding conditionnel et le routage personnalisé dans Dynamic Chat.

## Version De Septembre/Octobre 2024 {#sep-oct-release}

### Analyses du chat en direct améliorées {#enhanced-live-chat-analytics}

Plusieurs améliorations ont été apportées au tableau de bord Analytics, notamment :

* Nombre total de discussions en direct demandées : nombre de visiteurs demandés pour une « conversation avec l’agent »

* Total du chat en direct connecté : nombre de visiteurs connectés par rapport au total demandé pour un « chat avec agent »

* Nombre total de demandes de conversation en direct manquantes : nombre de visiteurs sans assistance par rapport au total demandé pour une « conversation avec l’agent »

* Durée moyenne de conversation en minutes : analysez la « durée moyenne de conversation » entre les visiteurs et vos agents.

* Temps de réponse moyen de l’agent en secondes : analysez le « temps moyen pris » par les agents pour répondre aux questions et réponses de leur chat en direct.

* Tableau de bord quotidien : requêtes de chat en direct connectées avec succès, requêtes de chat en direct manquantes, trier et filtrer les activités récentes de chat en direct

![](assets/dynamic-chat-sep-oct-2024-release-1.png)

### Notation des conversations {#conversation-scoring}

Quantifiez vos prospects en fonction de la qualité de leur interaction de conversation et utilisez cette mesure comme déclencheur/filtre dans les campagnes intelligentes Marketo Engage. Utilisez le nouvel attribut _score de conversation_ sur les activités suivantes :

* Engagé dans un dialogue
* Engagé dans un flux de conversation
* Engagement avec un agent

**Points à noter :**

* La valeur du score sera comprise entre 0, 1, 2 et 3 (la valeur par défaut est null).

* Une fois la conversation terminée ou supprimée, la valeur de score ne peut pas être modifiée

* Définition d’un score :

   * Dans la boîte de réception de l’agent, au cours d’une conversation en direct, l’agent peut mettre à jour ou définir un score pour la conversation, qui est stocké dans l’activité de conversation

   * Dans le concepteur de flux, dans la carte d’objectif, l’utilisateur peut mettre à jour ou définir un score pour la conversation

![](assets/dynamic-chat-sep-oct-2024-release-2.png)

![](assets/dynamic-chat-sep-oct-2024-release-3.png)

![](assets/dynamic-chat-sep-oct-2024-release-4.png)

### Nouvelle logique de création de leads {#new-lead-creation-logic}

Si un prospect remplit un formulaire avec le `abc@test.com` d’e-mail et est copié en tant que xyz, puis remplit le même formulaire avec le `def@test.com` d’e-mail, un nouvel enregistrement de personne est créé, mais le cookie xyz est associé au nouvel utilisateur et supprimé du `abc@test.com` de personne.

Ainsi, lorsqu’un visiteur avec le cookie abc arrive sur une page et fournit un ID d’e-mail comme `abc@test.com` :

<table><thead>
  <tr>
    <th>Visitor</th>
    <th>Cookie</th>
    <th>E-mail fourni</th>
    <th>Comportement attendu</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Anonyme</td>
    <td>abc</td>
    <td>N'existe pas dans la base de données</td>
    <td>Créer une nouvelle personne</td>
  </tr>
  <tr>
    <td>Anonyme</td>
    <td>abc</td>
    <td>Existe dans la base de données</td>
    <td>Fusionner la personne</td>
  </tr>
  <tr>
    <td>Anonyme</td>
    <td>xyz</td>
    <td>Existe dans la base de données</td>
    <td>Fusionner la personne</td>
  </tr>
  <tr>
    <td>Personne connue</td>
    <td>abc</td>
    <td>Identique à la personne existante</td>
    <td>Mettre à jour la personne</td>
  </tr>
  <tr>
    <td>Personne connue</td>
    <td>abc</td>
    <td>Différent de la personne existante</td>
    <td>S’il existe déjà une personne connue, transférez le cookie et résolvez ce profil. Si cet e-mail ne comporte aucune personne, créez un nouvel enregistrement de personne et transférez le cookie</td>
  </tr>
  <tr>
    <td>Personne connue</td>
    <td>xyz</td>
    <td>Identique à la personne existante</td>
    <td>Ajouter un nouveau cookie à la même personne</td>
  </tr>
  <tr>
    <td>Personne connue</td>
    <td>xyz</td>
    <td>Différent de la personne existante</td>
    <td>ce scénario n’est pas possible, comme s’il s’agissait d’un nouveau cookie :   Valeur par défaut considérée comme un nouveau profil anonyme</td>
  </tr>
</tbody></table>

### Option d’héritage de la police {#option-to-inherit-font}

Vous pouvez désormais permettre au chatbot d’hériter directement de la police de la page web où elle est hébergée, au lieu de gérer la police de la marque dans Dynamic Chat. Lorsque vous activez cette option, le bot conversationnel utilise la police définie sur `<body>` balise de la page.

![](assets/dynamic-chat-sep-oct-2024-release-5.png)

### Intégration de Demandbase à Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Les utilisateurs Demandbase peuvent apporter leur propre licence Demandbase et activer l&#39;intégration. Utilisez les attributs de personne Demandbase pour le ciblage de boîte de dialogue, le branding conditionnel et le routage personnalisé.

La résolution de ces valeurs d’attribut sur une personne est effectuée en temps réel et sont stockées dans le profil de personne correspondant.

### Optimisation du temps de chargement du flux de conversation {#optimized-conversation-flow-load-time}

Pour améliorer l’expérience utilisateur, un chargeur de scintillement s’affiche désormais au lieu d’un espace vide pendant le chargement du flux de conversation.

**Avant**

![](assets/dynamic-chat-sep-oct-2024-release-6.png)

**Après**

![](assets/dynamic-chat-sep-oct-2024-release-7.gif)

## Version d’août 2024 {#august-release}

**Date de publication : samedi 23 août 2024**

### Personnaliser le format de vos messages de conversation {#custom-format-conversation-messages}

Les concepteurs de flux prennent désormais en charge [l’insertion d’HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"} pour personnaliser l’aspect de vos conversations.

![](assets/dynamic-chat-aug-2024-release-1.png)

### Défilement du bot conversationnel vers le bas {#chatbot-scroll-to-bottom}

Une icône a été ajoutée au chatbot pour permettre aux visiteurs web d’accéder directement au dernier message. Cela permet aux visiteurs et aux visiteuses de faire défiler le texte pour revenir rapidement à la conversation.

![](assets/dynamic-chat-aug-2024-release-2.png)

### Notifications Core Pulse {#core-pulse-notifications}

Les utilisateurs reçoivent désormais une [ notification par e-mail ](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"} en cas d’échec d’une réservation de réunion ou d’une discussion en direct.

![](assets/dynamic-chat-aug-2024-release-3.png)

### Prise en charge de plusieurs conversations {#support-for-multiple-conversations}

Le bot conversationnel prend désormais en charge plusieurs conversations. Les visiteurs et visiteuses du site Web peuvent engager différentes conversations sur différentes pages en même temps, avec la possibilité de passer d’une page à l’autre.

![](assets/dynamic-chat-aug-2024-release-4.png)

### Tri par défaut du contenu {#default-sorting-for-content}

Par défaut, vos logs de conversation, questions sans réponse et tableaux de génération de questions sont triés par date de création (du plus récent au plus ancien).

### Résolution des leads en temps réel {#real-time-lead-resolution}

Lors d’une conversation avec un prospect anonyme et qu’un ID d’e-mail est fourni, nous déterminons si un enregistrement de prospect connu existe avec cet ID d’e-mail et utilisons cet enregistrement pour la personnalisation en temps réel. Si nous trouvons plusieurs enregistrements, nous les fusionnons en temps réel. Ce comportement est implémenté pour les boîtes de dialogue et les flux de conversation.

### Synchronisation des prospects sans cookies depuis Marketo Engage {#syncing-leads-without-cookies}

Auparavant, lorsque la synchronisation Marketo Engage était activée, Dynamic Chat synchronisait uniquement les prospects connus avec un ou plusieurs identifiants de cookie provenant de Marketo Engage. Désormais, tous les prospects connus (identifiant de cookie présent ou non) seront synchronisés dans Dynamic Chat et pourront être utilisés pour la personnalisation des conversations.

### Transmettre des données de visiteur supplémentaires aux flux de conversation {#pass-additional-visitor-data}

Si vous capturez des informations sur les visiteurs par d’autres canaux tels que les formulaires ou les connexions, vous pouvez désormais transmettre ces informations directement à Dynamic Chat.

![](assets/dynamic-chat-aug-2024-release-5.png)

### Actualisation des données déduites {#refreshed-inferred-data}

La majorité des conversations sur un site web ont lieu avec des visiteurs anonymes. Vous pouvez toujours les cibler par le biais de données déduites, qui repose sur les adresses IP des visiteurs. Nous avons mis à jour notre base de données d&#39;adresses IP et de données déduites respectives qui prend désormais en charge quatre fois plus d&#39;adresses IP.

### Son ajouté à la notification du navigateur de l’agent {#sound-added-to-agent-browser-notification}

Lorsqu’un chat en direct est affecté à un agent, il reçoit une notification du navigateur. Mais de temps en temps, ils ne les voient pas. Nous avons ajouté un [son de notification](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"} pour éviter les notifications manquées à l’avenir.

![](assets/dynamic-chat-aug-2024-release-6.png)

### Possibilité de mettre à jour le profil du prospect pendant le chat en direct {#update-lead-profile-during-live-chat}

Au cours d’une discussion en direct, les agents souhaitent capturer des informations sur le visiteur et mettre à jour le profil correspondant. Il existe désormais une option pour mettre à jour les valeurs d’attribut des objets lead et société.

![](assets/dynamic-chat-aug-2024-release-7.png)

## Version de juin 2024 {#june-release}

**Date de publication : vendredi 6 juin 2024**

### Carte Flux de conversation {#conversational-flow-card}

Simplifiez plusieurs étapes d’un flux dans vos boîtes de dialogue à l’aide de la carte Flux de conversation .

Exemple : si votre objectif est de générer les inscriptions à votre webinaire par le biais de plusieurs boîtes de dialogue, vous devrez recréer le même flux dans toutes les boîtes de dialogue qui ont cet objectif. Et si vous devez mettre à jour un détail, vous devez modifier chaque boîte de dialogue individuelle une par une. Ce n’est plus le cas, grâce à la carte Flux de conversation .

En plus de réutiliser des flux sur plusieurs boîtes de dialogue, vous pouvez utiliser le même flux de transition pour déclencher via d’autres canaux, tels que les formulaires et les pages de destination.

![](assets/dynamic-chat-june-2024-release-1.png)

### Limites d’utilisation {#usage-limits}

La page Limites d’utilisation vous présente des informations importantes, telles que les détails du package et le statut de votre limite d’utilisation.

![](assets/dynamic-chat-june-2024-release-2.png)

## Version de mai 2024 {#may-release}

**Date de mise à jour : jeudi 15 mai 2024**

### Bibliothèque de réponses préapprouvée {#pre-approved-response-library}

[Créez une bibliothèque approuvée par marketing](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} de questions et réponses générées par l’IA pour aider à configurer un chat IA génératif en quelques minutes.

![](assets/dynamic-chat-may-2024-release-1.png)

### Questions sans réponse {#unanswered-questions}

[Utilisez un référentiel de questions sans réponse](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"} issues de conversations précédentes pour générer de nouvelles réponses préapprouvées en conservant une bibliothèque de réponses avec les informations les plus récentes.

![](assets/dynamic-chat-may-2024-release-2.png)

### Résumés de la conversation {#conversation-summaries}

[Donnez aux agents commerciaux un résumé des conversations](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"} y compris des idées sur les principaux sujets de discussion avant les réunions afin de réduire le temps de préparation et de mieux armer les agents commerciaux avec les dernières informations.

![](assets/dynamic-chat-may-2024-release-3.png)

### Raccourcis de vente GenAI {#genai-sales-shortcuts}

[Fournissez aux agents de chat en direct des moyens plus rapides](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"} pour accéder aux réponses générées par l’IA, modifier les réponses générées existantes et rechercher du contenu supplémentaire à envoyer aux acheteurs lors de la conversation.

![](assets/dynamic-chat-may-2024-release-4.png)

### Aide à la conversation {#conversation-assist}

Aidez les agents commerciaux à répondre avec précision lors de conversations en direct en utilisant des réponses préapprouvées par votre équipe marketing.

### Coups de pouce dans la conversation {#conversation-nudges}

Incitez les visiteurs et visiteuses web à utiliser un call-to-action pour mener les conversations à leur terme.

<p>

## Version d’avril 2024 {#april-release}

**Date de publication : mercredi 23 avril 2024**

### Flux de conversation désormais disponibles pour tous les utilisateurs {#conversational-flows-available-to-all-users}

Rendez vos formulaires et vos pages de destination plus conversationnels et raccourcissez l’entonnoir des ventes en permettant aux prospects qualifiés de réserver une réunion ou une conversation avec le service des ventes immédiatement après un envoi de formulaire avec Conversational Forms, désormais entièrement disponible&#42; pour tous les utilisateurs de Dynamic Chat.

_&#42;Précédemment disponible en version d’essai avec 100 engagements à vie. Les engagements de flux de conversation seront désormais comptabilisés dans la limite mensuelle de 250 conversations engagées pour les utilisateurs du package Sélectionner_.

### Fonctions de rappel {#callback-functions}

[Fonctions de rappel](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"} vous permettent de collecter des événements d’analyse Dynamic Chat dans des systèmes externes, tels qu’Adobe Analytics ou Google Analytics, lorsque les visiteurs et visiteuses participent à des conversations Dynamic Chat. Vous activez les événements Dynamic Chat Analytics en enregistrant un rappel avec l’API pour écouter les événements. Vous disposez ainsi d’une vue plus holistique de votre engagement Dynamic Chat par rapport à d’autres données essentielles, telles que le trafic web.

### Conditions de disponibilité des agents dynamiques ajoutées à l’embranchement conditionnel {#live-agent-availability-conditional-branching}

Outre les champs Marketo Engage natifs et personnalisés, vous pouvez désormais utiliser l’embranchement conditionnel pour créer des branches en fonction de la disponibilité de l’agent. Cela s’avère utile si vous souhaitez uniquement offrir aux visiteurs la possibilité de parler à un agent en direct lorsqu’il existe des agents en direct disponibles.

![](assets/dynamic-chat-release-1.png)

### Condition de liste dynamique ajoutée à l’embranchement conditionnel {#smart-list-condition}

Grâce à l’ajout de la nouvelle condition de liste dynamique Marketo Engage dans l’embranchement conditionnel, vous pouvez créer des branches basées sur des audiences préexistantes que vous avez déjà créées dans Marketo Engage plutôt que de définir des conditions d’embranchement des audiences dans Dynamic Chat.

![](assets/dynamic-chat-release-2.png)

### Embranchement conditionnel pour les flux de conversation {#conditional-branching-for-conversational-flows}

Nous avons lancé l’embranchement conditionnel pour les boîtes de dialogue plus tôt cette année. Vous pouvez désormais tirer parti de l’embranchement conditionnel dans les flux de conversation également ! L’embranchement conditionnel vous permet de créer des branches dans votre flux en fonction de différentes conditions.

### Chat en direct pour les flux de conversation {#live-chat-for-conversational-flows}

Nous avons publié la fonctionnalité de chat en direct pour les dialogues en 2023. Vous pouvez désormais ajouter des engagements de chat en direct à vos flux de conversation également. Si vous utilisez des flux de conversation avec vos formulaires Marketo Engage, vous pouvez désormais permettre aux visiteurs qualifiés de discuter avec un agent en direct immédiatement après l’envoi du formulaire.

### Activités Marketo Engage récentes dans la boîte de réception de l’agent {#recent-marketo-engage-activities-in-agent-inbox}

Nous avons ajouté des activités Marketo Engage récentes à la section Activités récentes de la boîte de réception de l’agent. Ainsi, lorsqu’un visiteur du site demande à discuter avec un agent, l’agent peut rapidement voir si le visiteur s’est récemment engagé dans l’une des activités Marketo Engage suivantes (25 dernières activités) :

* E-mail ouvert
* Page web visitée
* Formulaire rempli
* A vécu un moment intéressant

![](assets/dynamic-chat-release-3.png)

### Statut de la connexion au calendrier dans la gestion des agents {#calendar-connection-status-in-agent-management}

Les administrateurs peuvent désormais facilement identifier les agents disposant d’autorisations de réservation de réunion qui ont connecté leurs calendriers dans Dynamic Chat. Vous pouvez ainsi vous assurer que toute votre équipe commerciale est connectée et prête à accepter les demandes de réunion de Dynamic Chat.

![](assets/dynamic-chat-release-4.png)

### Paramètre d’avis minimal dans la configuration du calendrier de l’agent {#minimum-notice-setting-in-agent-calendar-configuration}

Les utilisateurs ont signalé que les visiteurs et visiteuses web réservaient des réunions dans leur calendrier avec un préavis aussi court que 10 minutes. Nous avons donc introduit un paramètre de préavis minimum dans la configuration du calendrier de l’agent et défini le délai par défaut à 24 heures.

![](assets/dynamic-chat-release-5.png)

### Ajout/suppression du comportement de l’utilisateur mis à jour {#add-remove-user-behavior-updated}

Certains utilisateurs ont indiqué avoir des problèmes avec l’ajout et la suppression d’agents dans le Module de conversation dynamique. Nous avons donc apporté quelques modifications pour résoudre ces problèmes.

Lorsqu’un utilisateur est ajouté à Admin Console avec une autorisation de conversation en direct ou de réservation de réunion, il s’affiche immédiatement dans la liste Gestion des agents et peut être ajouté aux boîtes de dialogue, aux flux de conversation, aux règles de routage et aux équipes.

Lorsqu’un utilisateur disposant d’autorisations de réservation de réunion ou de chat en direct est supprimé d’Admin Console, il est immédiatement supprimé de Dynamic Chat, ne sera plus disponible pour le chat en direct ou le routage de réunion et ne sera plus pris en compte dans les limites de licence.

### Amélioration des performances des rapports de niveau conversation {#improved-conversation-level-report-performance}

Les rapports individuels de niveau Dialogue et Flux de conversation sont désormais plus performants et plus précis. Auparavant, le chargement des rapports de boîte de dialogue pouvait prendre plusieurs secondes et les données pouvaient parfois être incohérentes par rapport aux rapports de performances globaux. Désormais, vos rapports de boîte de dialogue individuels se chargent en un instant et les données sont toujours alignées avec les données de rapports globales.

![](assets/dynamic-chat-release-6.png)

### Mises à jour des autorisations {#permission-updates}

Nous avons nettoyé la structure des autorisations et les noms dans Adobe Admin Console pour rendre la gestion des autorisations plus intuitive.

* La catégorie « Gestion des conversations » s’appelle désormais « Conversations »
* La catégorie &#39;Réunions&#39; s&#39;appelle désormais &#39;Activités&#39;
* La catégorie &#39;Paramètres d&#39;agent&#39; est maintenant appelée &#39;Agents&#39;
* La catégorie &#39;Paramètres d&#39;administration&#39; s&#39;appelle désormais &#39;Configuration&#39;
* La catégorie &#39;Live Chat&#39; a été supprimée et toutes les autorisations de Live Chat ont été déplacées vers la catégorie Agents

![](assets/dynamic-chat-release-7.png)

### Prise en charge des liens hypertexte dans la boîte de réception de l’agent {#support-for-hyperlinks-in-agent-inbox}

Désormais, lorsque les agents de chat en direct partagent des URL avec les visiteurs du chat, ces URL sont liées par un lien hypertexte afin que les visiteurs puissent simplement cliquer dessus pour accéder à la page, plutôt que d’avoir à copier et coller l’URL dans leur navigateur.

### Saisir le comportement de clé mis à jour dans la boîte de réception de l’agent {#enter-key-behavior-updated-in-agent-inbox}

Nous avons changé le comportement de la clé de retour dans la boîte de réception de l’agent. Par conséquent, appuyer sur la touche Retour ou Entrée enverra votre message et appuyer sur Maj + Entrée créera un saut de ligne.

![](assets/dynamic-chat-release-8.png)

### Page circulaire supprimée {#round-robin-page-removed}

Ne vous inquiétez pas ! Le routage circulaire est toujours entièrement fonctionnel et fonctionne de la même manière qu&#39;il l&#39;a toujours fait. Nous venons de supprimer la page qui montrait une liste souvent inexacte d&#39;agents et leur ordre dans la file d&#39;attente de routage à tour de rôle.

Lorsque nous avons publié Dynamic Chat en 2022, il n’y avait aucune prise en charge du chat en direct, seulement de la réservation de réunions, et la page de routage à tour de rôle a été conçue en tenant compte uniquement de la réservation de réunions. Avec l’introduction du chat en direct l’année dernière, la page de round robin est devenue obsolète, car elle ne reflétait pas précisément la nature plus complexe du routage de round robin entre les agents avec à la fois des autorisations de réservation de réunion et de chat en direct. Nous avons exploré quelques options différentes pour résoudre ce problème, mais nous avons finalement décidé que la supprimer complètement était la meilleure option pour minimiser la confusion.

![](assets/dynamic-chat-release-9.png)

## Version de février 2024 {#february-release}

**Date de mise à jour : vendredi 22 février 2024**

### Page Conversations {#conversations-page}

La nouvelle page Conversations vous offre un guichet unique pour afficher les transcriptions de toutes les conversations (automatisées et en direct) qui ont eu lieu pour votre instance, à partir de prospects connus et anonymes, ce qui vous permet de mieux connaître la manière dont vos clients interagissent avec vos boîtes de dialogue, flux de conversation et agents en direct.

![](assets/dynamic-chat-release-10.png)

### La période dans le tableau de bord global est passée de 90 jours à 24 mois {#date-range-in-global-dashboard}

Vous avez demandé et nous avons tenu parole. Vous pouvez désormais afficher les données d’engagement de Dynamic Chat pendant un maximum de deux ans dans tous les tableaux de bord Analytics.

### Embranchement conditionnel dans les boîtes de dialogue {#conditional-branching-in-dialogues}

L’embranchement conditionnel vous permet de créer des branches dans vos flux de boîte de dialogue en fonction de différentes conditions. Désormais, vous pouvez présenter différents contenus à différentes personnes dans la même boîte de dialogue en fonction des attributs du prospect et de la société dans Marketo Engage.

## Version de janvier 2024 {#january-release}

**Date de publication : jeudi 24 janvier 2024**

### Paramètre de limite des conversations en direct simultanées dans la gestion des agents {#Concurrent-live-chat-limit-setting}

Par défaut, chaque agent de chat en direct de votre instance peut participer à un maximum de 5 sessions de chat en direct à la fois. Nous avons introduit un nouveau paramètre dans la gestion des agents qui vous permet d’ajuster cette limite de 1 à 10.

![](assets/dynamic-chat-release-11.png)
