---
description: Présentation De Dynamic Chat - Documents Marketo - Documentation Du Produit
title: Présentation de Dynamic Chat
feature: Dynamic Chat
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 4%

---

# Présentation d’[!DNL Dynamic Chat] {#dynamic-chat-overview}

Dynamic Chat vous permet de tirer parti d’une interface conviviale pour cibler les personnes et les comptes qui visitent votre site web. Collectez le contenu pertinent, tel que le nom, les coordonnées et le texte libre. Les visiteurs du site peuvent également discuter avec un agent en direct et même réserver des réunions avec votre équipe des ventes. Les données d’activité et d’engagement de Dynamic Chat peuvent être utilisées pour ajouter des membres aux programmes Marketo et déclencher des activités cross-canal.

>[!TIP]
>
>Consultez [cette page](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html){target="_blank"} pour visionner des tutoriels vidéo sur Dynamic Chat.

## Intégrations {#integrations}

Un composant essentiel de Dynamic Chat est sa capacité à interagir de manière native avec votre abonnement Marketo. Pour tirer pleinement parti de cette intégration, vous devez d’abord lancer la synchronisation des données. Selon la taille de votre base de données Marketo, l’exécution de la synchronisation initiale [unique](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"} peut prendre jusqu’à 24 heures pour les données.

Les éléments suivants sont synchronisés :

* Données de champ de personne
* Données de champ d’entreprise
* Données d’activité

## Dialogues {#dialogues}

Les boîtes de dialogue représentent un engagement de conversation unique. Considérez-le comme un conteneur avec tout ce dont vous avez besoin pour avoir un dialogue de conversation engageant avec les visiteurs de votre site web. Dans chaque boîte de dialogue, vous pouvez spécifier la ou les pages sur lesquelles vous souhaitez que la boîte de dialogue apparaisse, à qui vous souhaitez qu’elle apparaisse, ainsi que le contenu et le flux de la boîte de dialogue elle-même. De plus, vous pouvez trouver des mesures pour évaluer les performances de votre boîte de dialogue. [En savoir plus sur les boîtes de dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}.

## Configuration {#configuration}

Dans l’onglet Configuration , personnalisez l’aspect de vos différentes boîtes de dialogue. Modifiez la police, les couleurs, le temps de réponse, etc. [En savoir plus sur la configuration](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}.

## Calendrier {#calendar}

Connectez votre calendrier Outlook ou Gmail pour l&#39;utiliser dans la planification des rendez-vous dans le chatbot. [En savoir plus sur le calendrier](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## Réunions {#meetings}

C’est là que vous verrez tous les rendez-vous qui ont été programmés par les visiteurs et visiteuses du site par le biais de vos différentes boîtes de dialogue. [En savoir plus sur les réunions](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## Routage {#routing}

C&#39;est là que vous pouvez voir une liste de tous les agents qui ont connecté leurs calendriers, l&#39;ordre dans lequel ils seront présentés aux visiteurs du site Web et créer des règles de routage personnalisées. [En savoir plus sur le routage](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## Chat en direct {#live-chat}

Offrez à vos visiteurs et visiteuses web qualifiés de communiquer avec vos représentants et représentantes commerciaux via [chat en direct](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}.

## Flux conversationnel {#conversational-flow}

[Concevez une conversation](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"} qui peut être déclenchée par un visiteur en fonction d’une action que vous avez désignée (par exemple, remplir un formulaire, cliquer sur un lien, etc.).

## IA générative {#generative-ai}

[L’IA générative](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/overview.md){target="_blank"} dans Adobe Dynamic Chat traite en temps réel les signaux d’intention, les préférences des utilisateurs et utilisatrices et les comportements passés afin de générer des messages personnalisés et pertinents pour les visiteurs et visiteuses du chat.

## Changer de langue {#changing-the-language}

Suivez les étapes ci-dessous pour modifier votre langue Dynamic Chat.

>[!IMPORTANT]
>
>La modification de la langue au niveau du profil modifie la langue pour _toutes_ les applications Experience Cloud, pas seulement pour les [!DNL Dynamic Chat].

1. Dans votre compte Experience Cloud, cliquez sur l’icône des paramètres et choisissez **[!UICONTROL Préférences]**.

   ![](assets/dynamic-chat-overview-1.png)

1. Cliquez sur la langue actuelle sous votre adresse e-mail.

   ![](assets/dynamic-chat-overview-2.png)

1. Choisissez votre nouvelle langue (la deuxième langue est facultative) et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Il existe quelques dizaines de langues à choisir, mais [!DNL Dynamic Chat] ne prend en charge que les langues suivantes : anglais, français, allemand, japonais, espagnol, italien, portugais brésilien, coréen, chinois simplifié et chinois traditionnel.

Lorsque vous mettez à jour la langue, tout ce qui se trouve dans l’application change, à l’exception des mots que vous avez personnellement renseignés (par exemple, réponses en flux continu).

## Limites de conservation des données de Dynamic Chat {#dynamic-chat-data-retention-limits}

Vous trouverez ci-dessous quelques-unes des limites/paramètres de Dynamic Chat. Pour obtenir une liste complète, reportez-vous à la page Marketo Engage [Description du produit](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

<table>
  <th>Type de données</th>
  <th>Période De Rétention</th>
 <tr>
  <td>Lead Anonyme Sans Engagement</td>
  <td>90 jours</td>
 </tr>
 <tr>
  <td>Activité de l’objectif</td>
  <td>24 mois</td>
 </tr>
 <tr>
  <td>Activité de document</td>
  <td>24 mois</td>
 </tr>
 <tr>
  <td>Interaction avec l’activité de boîte de dialogue</td>
  <td>90 jours</td>
 </tr>
 <tr>
  <td>Activité de réservation de réunion</td>
  <td>24 mois</td>
 </tr>
</table>

## Questions fréquentes {#faq}

Consultez la [FAQ Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/faq.md){target="_blank"}.
