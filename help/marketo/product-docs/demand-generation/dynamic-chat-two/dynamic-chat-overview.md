---
description: Présentation du Dynamic Chat - Documents Marketo - Documentation du produit
title: Présentation du Dynamic Chat
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 3fc84a0e679b0b27aaf4ee251668a3ba0a62f9ef
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 3%

---

# Présentation du Dynamic Chat {#dynamic-chat-overview}

Dynamic Chat vous permet d’exploiter une interface conviviale pour cibler à la fois les personnes et les comptes qui visitent votre site web. Collectez le contenu approprié, tel que le nom, les coordonnées et le texte libre. Les visiteurs du site peuvent également réserver des réunions avec votre équipe de vente. Les données d’activité et d’engagement des Dynamic Chat peuvent être utilisées pour ajouter des membres aux programmes Marketo et déclencher des activités cross-canal.

>[!NOTE]
>
>Dynamic Chat est en cours de déploiement progressif et est actuellement en disponibilité limitée. Cette page sera mise à jour avec les informations de disponibilité générale dès qu&#39;elles seront disponibles.

>[!TIP]
>
>Visite [cette page](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) pour afficher des tutoriels vidéo de Dynamic Chat.

## Intégrations {#integrations}

Un composant clé de Dynamic Chat est sa capacité à interagir de manière native avec votre abonnement Marketo. Pour tirer parti de la fonctionnalité complète de cette intégration, vous devez d’abord lancer la synchronisation des données. Selon la taille de votre base de données Marketo, les données initiales peuvent prendre jusqu’à 24 heures, [synchronisation unique](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md) pour terminer.

Les éléments suivants sont synchronisés :

* Données de champ de personne
* Données de champ de l’entreprise
* Données d’activité

## Dialogues {#dialogues}

Les dialogues représentent un seul engagement de discussion. Considérez-le comme un conteneur avec tout ce dont vous avez besoin pour avoir un dialogue de conversation engageant avec les visiteurs de votre site web. Dans chaque dialogue, vous pouvez spécifier la ou les pages sur lesquelles vous souhaitez que le dialogue s’affiche, à qui vous souhaitez qu’il s’affiche, ainsi que le contenu et le flux du dialogue lui-même. En outre, vous pouvez trouver des mesures pour voir les performances de votre dialogue. [En savoir plus sur les boîtes de dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target="_blank"}.

## Configuration {#configuration}

Dans l&#39;onglet Configuration , personnalisez l&#39;aspect de vos différents Dialogues. Modifiez la police, les couleurs, le temps de réponse, etc. [En savoir plus sur la configuration](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target="_blank"}.

## Calendrier {#calendar}

Connectez votre calendrier Outlook ou Gmail pour l’utiliser dans la planification des rendez-vous dans le chatterbot. [En savoir plus sur le calendrier](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md){target="_blank"}

## Réunions {#meetings}

C&#39;est là que vous verrez toutes les nominations programmées par les visiteurs de votre site web à travers vos Dialogues. [En savoir plus sur les réunions](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/meetings.md){target="_blank"}

## Routage {#routing}

C’est là que vous pouvez voir la liste de tous les agents qui ont connecté leurs calendriers, l’ordre dans lequel ils seront présentés aux visiteurs du site web et créer des règles de routage personnalisées. [En savoir plus sur le routage](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/routing.md){target="_blank"}

## Chat en direct {#live-chat}

Offrir à vos visiteurs web qualifiés de se connecter à vos représentants commerciaux via [chat en direct](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md){target="_blank"}.

## Questions fréquentes {#faq}

**Puis-je installer Dynamic Chat n’importe où sur le site web de ma société ou est-ce que cela ne fonctionne que sur les landing pages Marketo ?**

Le fragment de code JavaScript du Dynamic Chat peut être installé sur n’importe quel site web ainsi que sur les landing pages Marketo.

**Quelle est la durée de stockage des données pour la création de rapports ?**

90 jours (voir la liste complète des limites [below](#limits-in-dynamic-chat)).

**Le Dynamic Chat autorise-t-il les conversations en direct ?**

Non, il utilise uniquement des réponses prédéterminées.

**Le Dynamic Chat prend-il en charge d’autres langues que l’anglais ?**

Oui. Le Dynamic Chat prend en charge les langues suivantes : français, allemand, japonais, espagnol, italien, portugais brésilien, coréen, chinois simplifié et chinois traditionnel. En savoir plus dans la section [section](#changing-the-language).

**Prenez-vous en charge la fonctionnalité AI/NLP ?**

La fonctionnalité AI/NLP n’est pas prise en charge.

**Comment cibler les personnes anonymes ?**

Dans votre boîte de dialogue, vous devez utiliser la variable _L’adresse électronique de personne est vide_ attribut.

## Modification de la langue {#changing-the-language}

Pour modifier la langue de votre Dynamic Chat, procédez comme suit.

>[!IMPORTANT]
>
>La modification de la langue au niveau du profil modifie la langue de _all_ des applications Experience Cloud, pas seulement des applications Dynamic Chat.

1. Dans votre compte d’Experience Cloud, cliquez sur l’icône des paramètres et sélectionnez **Préférences**.

   ![](assets/dynamic-chat-overview-1.png)

1. Cliquez sur la langue actuelle sous votre adresse électronique.

   ![](assets/dynamic-chat-overview-2.png)

1. Choisissez votre nouvelle langue (la seconde langue est facultative) et cliquez sur **Enregistrer**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Le choix de quelques dizaines de langues n&#39;est possible que dans les langues suivantes : anglais, français, allemand, japonais, espagnol, italien, portugais brésilien, coréen, chinois simplifié et chinois traditionnel.

Lorsque vous mettez à jour la langue, tout dans l’application elle-même change, à l’exception des mots que vous avez personnellement renseignés (par exemple, les réponses de diffusion en continu).

## Limites en Dynamic Chat {#limits-in-dynamic-chat}

<table>
  <th>Paramètre</th>
  <th>Description</th>
  <th>Limite</th>
 <tr>
  <td>Dialogues totaux</td>
  <td>Nombre de boîtes de dialogue (publiées et préliminaires)</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Calendriers totaux</td>
  <td>Nombre de calendriers connectés</td>
  <td>25</td>
 </tr>
 <tr>
  <td>Nombre total d’utilisateurs (administrateurs et utilisateurs marketing)</td>
  <td>Nombre d’utilisateurs combinés autorisés par instance de Dynamic Chat</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Dialogues publiés</td>
  <td>Nombre de boîtes de dialogue publiées enregistrées</td>
  <td>100</td>
 </tr>
 <tr>
  <td>URL cible par dialogue</td>
  <td>Nombre d’URL Target pouvant être ajoutées à un seul dialogue</td>
  <td>20</td>
 </tr>
 <tr>
  <td>Attributs par dialogue</td>
  <td>Nombre d’attributs pouvant être ajoutés aux critères d’audience pour un seul dialogue</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Groupes</td>
  <td>Nombre de groupes pouvant être ajoutés à un seul dialogue</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Attributs par groupe</td>
  <td>Nombre d’attributs pouvant être ajoutés à un groupe</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Cartes</td>
  <td>Nombre de cartes pouvant être ajoutées à la zone de travail par dialogue</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Période de conservation des données de piste anonyme</td>
  <td>Durée pendant laquelle les informations d’une piste anonyme sans engagement seront conservées</td>
  <td>90 jours</td>
 </tr>
 <tr>
  <td>Période de conservation de l’activité de l’objectif</td>
  <td>Durée pendant laquelle les données d’activité d’objectif sont conservées</td>
  <td>24 mois</td>
 </tr>
 <tr>
  <td>Période de conservation de l’activité de document</td>
  <td>Durée pendant laquelle les données d’activité de document sont conservées</td>
  <td>24 mois</td>
 </tr>
 <tr>
  <td>Interaction avec la période de rétention de l’activité de dialogue</td>
  <td>La durée d’interaction avec les données d’activité Dialogue est conservée</td>
  <td>90 jours</td>
 </tr>
 <tr>
  <td>Période de conservation de l’activité de réservation d’une réunion</td>
  <td>La durée de la réunion pendant laquelle l’activité de réservation sera stockée dans Dynamic Chat</td>
  <td>24 mois</td>
 </tr>
 <tr>
  <td>Conversations en cours</td>
  <td>Nombre de conversations en ligne avec lesquelles les visiteurs web peuvent interagir par mois</td>
  <td>250</td>
 </tr>
 <tr>
  <td>Conversations déclenchées</td>
  <td>Nombre de conversations en ligne qui peuvent être présentées aux visiteurs web par mois</td>
  <td>25,000</td>
 </tr>
</table>
