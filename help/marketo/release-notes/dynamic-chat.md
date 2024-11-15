---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour de Dynamic Chat
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: b6fb381527a24286fef5e438d7bf12b029810e64
workflow-type: tm+mt
source-wordcount: '2427'
ht-degree: 2%

---

# Notes de mise à jour de Dynamic Chat {#dynamic-chat-release}

Les versions de Adobe Dynamic Chat fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive du déploiement des fonctionnalités. Parfois, il existe plusieurs versions en un mois. Par conséquent, veuillez consulter régulièrement les informations les plus récentes.

La page des notes de mise à jour standard du Marketo Engage [ se trouve ici ](/help/marketo/release-notes/current.md){target="_blank"}.

## Version de septembre/octobre 2024 {#sep-oct-release}

### Amélioration de l’analyse des conversations en direct {#enhanced-live-chat-analytics}

Plusieurs améliorations ont été apportées au tableau de bord Analytics, notamment :

* Nombre total de discussions en direct demandées : nombre de visiteurs ayant demandé une &quot;discussion avec l’agent&quot;

* Total des tchats en direct connectés : nombre de visiteurs connectés par rapport au total demandé pour une &quot;conversation avec l’agent&quot;

* Nombre total de demandes de messagerie instantanée manquantes : nombre de visiteurs sans assistance par rapport au total demandé pour une &quot;conversation avec l’agent&quot;

* Durée moyenne de la conversation en minutes : analyse de la &quot;durée moyenne de la conversation&quot; entre les visiteurs et vos agents

* Temps moyen de réponse de l’agent en secondes : analysez le &quot;temps moyen&quot; pris par les agents pour répondre à leurs questions et réponses sur le chat en direct.

* Tableau de bord quotidien : demandes de chat en direct connectées correctement, demandes de chat en direct non exécutées, tri et filtrage des activités de chat en direct récentes

![](assets/dynamic-chat-sep-oct-2024-release-1.png)

### Score de conversation {#conversation-scoring}

Quantifiez vos pistes en fonction de la qualité de leur interaction de conversation et utilisez cette mesure comme déclencheur/filtre dans les campagnes dynamiques de Marketo Engage. Utilisez le nouvel attribut _score de conversation_ sur les activités suivantes :

* Engagé dans un dialogue
* Engagé avec un flux de conversation
* Engagé avec un agent

**Choses à noter :**

* La valeur de score sera comprise entre 0, 1, 2 et 3 (la valeur par défaut est nulle).

* Une fois la conversation terminée ou supprimée, la valeur de notation ne peut pas être modifiée.

* Définir un score :

   * Dans la boîte de réception de l’agent : au cours d’une conversation en direct, l’agent peut mettre à jour ou définir un score pour la conversation, qui est stocké dans l’activité de conversation.

   * Dans le concepteur de flux, dans la carte d’objectif, l’utilisateur peut mettre à jour ou définir un score pour la conversation.

![](assets/dynamic-chat-sep-oct-2024-release-2.png)

![](assets/dynamic-chat-sep-oct-2024-release-3.png)

![](assets/dynamic-chat-sep-oct-2024-release-4.png)

### Nouvelle logique de création de piste {#new-lead-creation-logic}

Si une piste remplit un formulaire avec l’email `abc@test.com` et est cookie comme xyz, puis remplit par la suite le même formulaire avec l’email `def@test.com`, un nouvel enregistrement de personne est créé, mais le cookie xyz devient associé à la nouvelle personne et supprimé de la personne `abc@test.com`.

Ainsi, lorsqu’un visiteur avec cookie abc arrive sur une page et fournit un ID de courrier électronique sous la forme `abc@test.com` :

<table><thead>
  <tr>
    <th>Visitor</th>
    <th>Cookie</th>
    <th>Email fourni</th>
    <th>Comportement attendu</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Anonyme</td>
    <td>abc</td>
    <td>N’existe pas dans la base de données</td>
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
    <td>S’il existe déjà une personne connue, transférez le cookie et résolvez ce profil. S’il n’existe aucune personne avec cet email, créez un nouvel enregistrement de personne et transférez le cookie.</td>
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
    <td>ce scénario n’est pas possible comme s’il s’agissait d’un nouveau cookie par   valeur par défaut considérée comme nouveau profil anonyme</td>
  </tr>
</tbody></table>

### Optimisation du temps de chargement du flux de conversation {#optimized-conversation-flow-load-time}

Pour améliorer l’expérience utilisateur, un chargeur de fuseaux horaires s’affiche maintenant au lieu d’un espace vide pendant le chargement du flux de conversation.

**Avant**

![](assets/dynamic-chat-sep-oct-2024-release-5.png)

**After**

![](assets/dynamic-chat-sep-oct-2024-release-6.gif)

### Option d’héritage de la police {#option-to-inherit-font}

Vous pouvez désormais activer le chatterbot pour qu’il hérite directement de la police de la page web où il est hébergé plutôt que de gérer la police de marque dans Dynamic Chat. Lorsque vous activez cette option, le chatterbot prend la police définie sur la balise `<body>` de la page.

![](assets/dynamic-chat-sep-oct-2024-release-7.png)

### Intégration de Demandbase avec Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Les utilisateurs de Demandbase peuvent apporter leur propre licence Demandbase et activer l’intégration. Utilisez les attributs de personne Demandbase pour le ciblage de dialogue, la valorisation de marque conditionnelle et le routage personnalisé.

La résolution de ces valeurs d’attribut par rapport à une personne est effectuée en temps réel et est stockée dans le profil de personne respectif.

## Version d’août 2024 {#august-release}

**Date de publication : samedi 23 août 2024**

### Format personnalisé de vos messages de conversation {#custom-format-conversation-messages}

Les concepteurs de diffusions prennent désormais en charge [l’insertion d’HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"} pour personnaliser l’aspect de vos conversations.

![](assets/dynamic-chat-aug-2024-release-1.png)

### Défilement du chatbot vers le bas {#chatbot-scroll-to-bottom}

Une icône a été ajoutée dans le chatterbot pour permettre aux visiteurs web d’accéder directement au dernier message. Cela permet aux visiteurs de parcourir le texte pour revenir rapidement à la conversation.

![](assets/dynamic-chat-aug-2024-release-2.png)

### Notifications Push principales {#core-pulse-notifications}

Les utilisateurs reçoivent désormais une [ notification par email ](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"} lorsqu’une réunion de réservation ou un chat en direct échoue.

![](assets/dynamic-chat-aug-2024-release-3.png)

### Prise en charge de plusieurs conversations {#support-for-multiple-conversations}

Le chatterbot prend désormais en charge plusieurs conversations. Les visiteurs du site web peuvent engager différentes conversations en même temps sur différentes pages, avec la possibilité de basculer entre elles.

![](assets/dynamic-chat-aug-2024-release-4.png)

### Tri par défaut du contenu {#default-sorting-for-content}

Par défaut, les logs de conversation, les questions sans réponse et les tableaux de génération de questions sont triés par date de création (de la plus récente à la plus ancienne).

### Résolution des pistes en temps réel {#real-time-lead-resolution}

Lors d’une conversation avec un prospect anonyme et qu’un ID de courrier électronique est fourni, nous nous résolvons si un enregistrement de piste connu existe avec cet ID de courrier électronique et nous utilisons cet enregistrement pour la personnalisation en temps réel. Si nous trouvons plusieurs enregistrements, nous les fusionnons en temps réel. Ce comportement est implémenté à la fois pour les dialogues et les flux de conversation.

### Synchronisation des pistes sans cookies de Marketo Engage {#syncing-leads-without-cookies}

Auparavant, lorsque la synchronisation du Marketo Engage était activée, Dynamic Chat synchronisait uniquement les pistes connues avec un ou plusieurs identifiants de cookie du Marketo Engage. Désormais, toutes les pistes connues (ID de cookie présent ou non) seront synchronisées dans Dynamic Chat et peuvent être utilisées pour la personnalisation des conversations.

### Transmission de données de visiteur supplémentaires aux flux de conversation {#pass-additional-visitor-data}

Si vous capturez les informations sur les visiteurs par le biais d’autres canaux tels que les formulaires ou la connexion, vous pouvez désormais les transmettre directement à Dynamic Chat.

![](assets/dynamic-chat-aug-2024-release-5.png)

### Actualisation des données déduites {#refreshed-inferred-data}

La majorité des conversations sur un site web se font avec des visiteurs anonymes. Vous pouvez toujours les cibler par le biais de données déduites, qui reposent sur les adresses IP des visiteurs. Nous avons mis à jour notre base de données d’adresses IP et de données respectives déduites qui prend désormais en charge quatre fois plus d’adresses IP.

### Son ajouté à la notification du navigateur de l’agent {#sound-added-to-agent-browser-notification}

Lorsqu’une conversation en direct est assignée à un agent, il reçoit une notification du navigateur. Mais parfois ils ne les voient pas. Nous avons ajouté un [son de notification](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"} pour empêcher les notifications manquées de continuer.

![](assets/dynamic-chat-aug-2024-release-6.png)

### Possibilité de mettre à jour le profil de prospect lors de la conversation en direct {#update-lead-profile-during-live-chat}

Lors d’une conversation en direct, les agents veulent capturer des informations sur le visiteur et mettre à jour le profil correspondant. Il existe désormais une option permettant de mettre à jour les valeurs d’attribut des objets prospect et société.

![](assets/dynamic-chat-aug-2024-release-7.png)

## Version de juin 2024 {#june-release}

**Date de publication : vendredi 6 juin 2024**

### Carte de flux de conversation {#conversational-flow-card}

Rationalisez plusieurs étapes dans un flux de vos boîtes de dialogue en utilisant la carte Flux de conversation .

Exemple : si votre objectif est de générer des inscriptions pour votre webinaire via plusieurs Dialogues, vous devrez recréer le même flux dans tous les Dialogues ayant cet objectif. Et si vous devez mettre à jour n&#39;importe quel détail, vous devez modifier chaque Dialogue individuellement un par un. Ce n&#39;est plus le cas, grâce à la carte Flux de conversation .

En plus de réaffecter les flux à plusieurs boîtes de dialogue, vous pouvez également utiliser le même flux de transition pour le déclencher via d’autres canaux, tels que les formulaires et les pages d’entrée.

![](assets/dynamic-chat-june-2024-release-1.png)

### Limites d’utilisation {#usage-limits}

La page Limites d’utilisation affiche des informations importantes, telles que les détails du module et l’état de votre limite d’utilisation.

![](assets/dynamic-chat-june-2024-release-2.png)

## Version de mai 2024 {#may-release}

**Date de mise à jour : jeudi 15 mai 2024**

### Bibliothèque de réponses prévalidée {#pre-approved-response-library}

[Créez une bibliothèque approuvée par le marketing](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} de questions et réponses générées par l’IA pour configurer le chat d’IA générative en quelques minutes.

![](assets/dynamic-chat-may-2024-release-1.png)

### Questions sans réponse {#unanswered-questions}

[Utilisez un référentiel de questions sans réponse](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"} des conversations précédentes pour générer de nouvelles réponses préapprouvées en conservant une bibliothèque de réponses avec les dernières informations.

![](assets/dynamic-chat-may-2024-release-2.png)

### Résumé des conversations {#conversation-summaries}

[Donnez aux agents de vente les conversations résumées](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"}, y compris des informations sur les sujets de discussion clés avant les réunions pour réduire le temps de préparation et mieux armer les agents de vente des informations les plus récentes.

![](assets/dynamic-chat-may-2024-release-3.png)

### Raccourcis commerciaux de GenAI {#genai-sales-shortcuts}

[Fournissez aux agents de conversation en direct des moyens plus rapides](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"} pour accéder aux réponses générées par l’IA, modifier les réponses générées existantes et rechercher du contenu supplémentaire à envoyer aux acheteurs pendant la conversation.

![](assets/dynamic-chat-may-2024-release-4.png)

### Aide à la conversation {#conversation-assist}

Aidez les agents de vente à réagir avec précision lors de conversations en direct à l’aide de réponses préapprouvées par votre équipe marketing.

### Poudrières de conversation {#conversation-nudges}

Déplacez les visiteurs web par un appel à l’action pour mener les conversations à leur terme.

<p>

## Version d’avril 2024 {#april-release}

**Date de publication : mercredi 23 avril 2024**

### Flux de conversation désormais disponibles pour tous les utilisateurs {#conversational-flows-available-to-all-users}

Rendez vos formulaires et vos pages d’entrée plus conversationnels et raccourcissez l’entonnoir de vente en permettant aux prospects qualifiés de réserver une réunion ou une discussion avec les ventes immédiatement après l’envoi d’un formulaire avec Conversational Forms, désormais entièrement disponible &#42; pour tous les utilisateurs Dynamic Chat.

_&#42;Auparavant disponible en tant que fonctionnalité d’évaluation avec 100 engagements de durée de vie. Les engagements de flux de conversation vont désormais être pris en compte dans la limite mensuelle de 250 conversations ouvertes pour les utilisateurs sur le package Sélectionner._

### Fonctions de rappel {#callback-functions}

Les [ fonctions de rappel ](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"} vous permettent de collecter des événements d’analyse de Dynamic Chat dans des systèmes externes, tels qu’Adobe Analytics ou les Google Analytics, lorsque les visiteurs interagissent avec des conversations de Dynamic Chat. Vous activez les événements Dynamic Chat Analytics en enregistrant un rappel avec l’API pour écouter les événements. Cela vous permet d’avoir une vision plus globale de votre engagement Dynamic Chat en ce qui concerne d’autres données clés, telles que le trafic web.

### Conditions de disponibilité de l’agent en direct ajoutées à l’embranchement conditionnel {#live-agent-availability-conditional-branching}

Outre les champs de Marketo Engage natifs et personnalisés, vous pouvez désormais utiliser un embranchement conditionnel pour créer des branches en fonction de la disponibilité de l’agent. Cela s’avère utile si vous souhaitez offrir aux visiteurs la possibilité de parler avec un agent en direct uniquement lorsque des agents en direct sont disponibles.

![](assets/dynamic-chat-release-1.png)

### Condition de liste dynamique ajoutée à un embranchement conditionnel {#smart-list-condition}

Avec l’ajout de la nouvelle condition Liste dynamique Marketo Engage dans l’embranchement conditionnel, vous pouvez créer des branches d’après les audiences préexistantes que vous avez déjà créées dans Marketo Engage plutôt que de définir des conditions d’embranchement d’audience dans Dynamic Chat.

![](assets/dynamic-chat-release-2.png)

### Branchement conditionnel pour les flux de conversation {#conditional-branching-for-conversational-flows}

Nous avons publié un embranchement conditionnel pour les Dialogues plus tôt cette année, et vous pouvez maintenant également tirer parti de l’embranchement conditionnel dans les flux de conversation ! L’embranchement conditionnel vous permet de créer des branches dans votre flux en fonction de différentes conditions.

### Chat en direct pour les flux de conversation {#live-chat-for-conversational-flows}

Nous avons lancé en 2023 la fonctionnalité de chat en direct pour les boîtes de dialogue. Vous pouvez désormais ajouter des engagements de chat en direct à vos flux de conversation. Si vous utilisez des flux de conversation avec vos formulaires de Marketo Engage, vous pouvez désormais autoriser les visiteurs qualifiés à discuter avec un agent en direct immédiatement après l’envoi du formulaire.

### Activités Marketo Engage récentes dans la boîte de réception de l’agent {#recent-marketo-engage-activities-in-agent-inbox}

Nous avons ajouté des activités de Marketo Engage récentes à la section Activités récentes de la boîte de réception de l’agent. Ainsi, lorsqu’un visiteur du site demande à discuter avec un agent, l’agent peut rapidement voir si le visiteur s’est récemment engagé dans l’une des activités de Marketo Engage suivantes (les 25 dernières activités) :

* E-mail ouvert
* Page web visitée
* Formulaire rempli
* A vécu un moment intéressant

![](assets/dynamic-chat-release-3.png)

### État de connexion au calendrier dans la gestion des agents {#calendar-connection-status-in-agent-management}

Les administrateurs peuvent désormais facilement identifier les agents disposant d’autorisations de réservation de réunions ayant connecté leurs calendriers en Dynamic Chat. Cela vous permet de vous assurer que l’équipe commerciale entière est connectée et prête à accepter les demandes de réunion de Dynamic Chat.

![](assets/dynamic-chat-release-4.png)

### Paramètre d’avertissement minimal dans la configuration du calendrier de l’agent {#minimum-notice-setting-in-agent-calendar-configuration}

Les utilisateurs ont signalé que les visiteurs web réservaient des réunions sur leur calendrier avec un préavis d’au moins 10 minutes. Nous avons donc ajouté un paramètre d’avertissement minimum dans la configuration du calendrier de l’agent et défini le délai d’avance par défaut sur 24 heures.

![](assets/dynamic-chat-release-5.png)

### Ajout/suppression d’un comportement utilisateur mis à jour {#add-remove-user-behavior-updated}

Certains utilisateurs ont indiqué qu’ils rencontraient des problèmes lors de l’ajout et de la suppression d’agents dans Dynamic chat. Nous avons donc apporté des modifications pour résoudre ces problèmes.

Lorsqu’un utilisateur est ajouté à un Admin Console avec une autorisation de conversation en direct ou de réservation de réunion, il apparaît immédiatement dans la liste Gestion des agents et peut être ajouté à des boîtes de dialogue, des flux de conversation, des règles de routage et des équipes.

Lorsqu’un utilisateur disposant d’autorisations de réservation de réunions ou de conversation en direct est supprimé de l’Admin Console, il est immédiatement supprimé de l’Dynamic Chat, il n’est plus disponible pour le chat en direct ou le routage de réunions, et il ne sera plus pris en compte dans les limites de licence.

### Amélioration des performances des rapports sur les niveaux de conversation {#improved-conversation-level-report-performance}

Les rapports au niveau du dialogue individuel et du flux de conversation sont désormais plus performants et précis. Auparavant, le chargement des rapports de dialogue pouvait prendre plusieurs secondes et les données étaient parfois incohérentes avec les rapports de performances globales. Désormais, vos rapports Dialogue individuels se chargent en un instant et les données seront toujours alignées avec les données de rapport globales.

![](assets/dynamic-chat-release-6.png)

### Mises à jour des autorisations {#permission-updates}

Nous avons nettoyé la structure et les noms des autorisations dans Adobe Admin Console afin de rendre la gestion des autorisations plus intuitive.

* La catégorie &quot;Gestion des conversations&quot; s’appelle désormais &quot;Conversations&quot;.
* La catégorie &quot;Réunions&quot; est désormais appelée &quot;Activités&quot;.
* La catégorie &quot;Paramètres de l’agent&quot; est désormais appelée &quot;Agents&quot;.
* La catégorie &quot;Paramètres d’administration&quot; s’appelle désormais &quot;Configuration&quot;.
* La catégorie &quot;Chat en direct&quot; a été supprimée et toutes les autorisations de chat en direct ont été déplacées vers la catégorie Agents.

![](assets/dynamic-chat-release-7.png)

### Prise en charge des hyperliens dans la boîte de réception des agents {#support-for-hyperlinks-in-agent-inbox}

Désormais, lorsque les agents de conversation en direct partagent des URL avec les visiteurs de la conversation, ces URL sont liées par un lien hypertexte afin que les visiteurs puissent simplement cliquer dessus pour accéder à la page, plutôt que d’avoir à copier et coller l’URL dans leur navigateur.

### Entrer le comportement clé mis à jour dans la boîte de réception de l’agent {#enter-key-behavior-updated-in-agent-inbox}

Nous avons modifié le comportement de la clé de retour dans la boîte de réception de l’agent. Dès lors, appuyez sur la touche Retour ou Entrée pour envoyer votre message et appuyez sur Maj+Entrée pour créer un saut de ligne.

![](assets/dynamic-chat-release-8.png)

### Suppression de la page Round Robin {#round-robin-page-removed}

Ne vous inquiétez pas ! Le routage de la boucle est toujours entièrement fonctionnel et fonctionne de la même manière qu’il l’a toujours été. Nous venons de supprimer la page qui montrait une liste souvent inexacte d&#39;agents et leur ordre dans la file d&#39;attente de routage du robot-rond.

Quand nous avons lancé Dynamic Chat en 2022, il n&#39;y avait pas de prise en charge du chat en direct, il n&#39;y avait que des réservations de réunions, et la page de routage du robin rond a été conçue uniquement en tenant compte des réservations de réunions. Avec l&#39;introduction du chat en direct l&#39;année dernière, la page de braquages en rond est devenue obsolète, car elle ne reflétait pas exactement la nature plus complexe du routage des vols en rond entre les agents avec des autorisations de réservation de réunions et de chat en direct. Nous avons exploré plusieurs options pour résoudre ce problème, mais nous avons finalement décidé que le supprimer était la meilleure option pour réduire la confusion.

![](assets/dynamic-chat-release-9.png)

## Version de février 2024 {#february-release}

**Date de mise à jour : vendredi 22 février 2024**

### Page Conversations {#conversations-page}

La nouvelle page Conversations vous offre un guichet unique pour afficher les transcriptions de toutes les conversations (automatisées et en direct) qui se sont produites pour votre instance, à partir de pistes connues et anonymes, ce qui vous permet de mieux comprendre comment vos clients interagissent avec vos boîtes de dialogue, vos flux de conversation et vos agents en direct.

![](assets/dynamic-chat-release-10.png)

### La période dans le tableau de bord global est passée de 90 jours à 24 mois. {#date-range-in-global-dashboard}

Vous avez demandé et nous avons livré. Vous pouvez désormais afficher les données d’engagement des Dynamic Chat pendant deux ans au maximum dans tous les tableaux de bord Analytics.

### Branchement conditionnel dans les boîtes de dialogue {#conditional-branching-in-dialogues}

L’embranchement conditionnel vous permet de créer des branches dans vos flux de dialogue en fonction de différentes conditions. Vous pouvez désormais présenter un contenu différent à différentes personnes dans le même dialogue en fonction des attributs de prospect et de société dans Marketo Engage.

## Version de janvier 2024 {#january-release}

**Date de publication : jeudi 24 janvier 2024**

### Limite concomitante de clics en direct dans la gestion des agents {#Concurrent-live-chat-limit-setting}

Par défaut, chaque agent de chat en direct de votre instance peut participer à un maximum de 5 sessions de chat en direct à la fois. Nous avons introduit un nouveau paramètre dans la gestion des agents qui vous permet d’ajuster cette limite de 1 à 10.

![](assets/dynamic-chat-release-11.png)
