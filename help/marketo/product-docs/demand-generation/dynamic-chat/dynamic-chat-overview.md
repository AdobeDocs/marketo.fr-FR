---
description: Présentation du Dynamic Chat - Documents Marketo - Documentation du produit
title: Présentation du Dynamic Chat
feature: Dynamic Chat
source-git-commit: 9a8f6fe57b585ba0eac6a577bf99e0419d8818a1
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 2%

---

# Présentation du Dynamic Chat {#dynamic-chat-overview}

Dynamic Chat vous permet d’exploiter une interface conviviale pour cibler à la fois les personnes et les comptes qui visitent votre site web. Collectez le contenu approprié, tel que le nom, les coordonnées et le texte libre. Les visiteurs du site peuvent également réserver des réunions avec votre équipe de vente. Les données d’activité et d’engagement des Dynamic Chat peuvent être utilisées pour ajouter des membres aux programmes Marketo et déclencher des activités cross-canal.

>[!TIP]
>
>Visite [cette page](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html){target="_blank"} pour afficher des tutoriels vidéo de Dynamic Chat.

## Intégrations {#integrations}

Un composant clé de Dynamic Chat est sa capacité à interagir de manière native avec votre abonnement Marketo. Pour tirer parti de la fonctionnalité complète de cette intégration, vous devez d’abord lancer la synchronisation des données. Selon la taille de votre base de données Marketo, les données initiales peuvent prendre jusqu’à 24 heures, [synchronisation unique](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"} pour terminer.

Les éléments suivants sont synchronisés :

* Données de champ de personne
* Données de champ de l’entreprise
* Données d’activité

## Dialogues {#dialogues}

Les dialogues représentent un seul engagement de discussion. Considérez-le comme un conteneur avec tout ce dont vous avez besoin pour avoir un dialogue de conversation engageant avec les visiteurs de votre site web. Dans chaque dialogue, vous pouvez spécifier la ou les pages sur lesquelles vous souhaitez que le dialogue s’affiche, à qui vous souhaitez qu’il s’affiche, ainsi que le contenu et le flux du dialogue lui-même. En outre, vous pouvez trouver des mesures pour voir les performances de votre dialogue. [En savoir plus sur les boîtes de dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}.

## Configuration {#configuration}

Dans l&#39;onglet Configuration , personnalisez l&#39;aspect de vos différents Dialogues. Modifiez la police, les couleurs, le temps de réponse, etc. [En savoir plus sur la configuration](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}.

## Calendrier {#calendar}

Connectez votre calendrier Outlook ou Gmail pour l’utiliser dans la planification des rendez-vous dans le chatterbot. [En savoir plus sur le calendrier](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## Réunions {#meetings}

C&#39;est là que vous verrez toutes les nominations programmées par les visiteurs de votre site web à travers vos Dialogues. [En savoir plus sur les réunions](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## Routage {#routing}

C’est là que vous pouvez voir la liste de tous les agents qui ont connecté leurs calendriers, l’ordre dans lequel ils seront présentés aux visiteurs du site web et créer des règles de routage personnalisées. [En savoir plus sur le routage](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## Chat en direct {#live-chat}

Offrir à vos visiteurs web qualifiés de se connecter à vos représentants commerciaux via [chat en direct](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}.

## Questions fréquentes {#faq}

**Puis-je installer Dynamic Chat n’importe où sur le site web de ma société ou est-ce que cela ne fonctionne que sur les landing pages Marketo ?**

Le fragment de code JavaScript du Dynamic Chat peut être installé sur n’importe quel site web ainsi que sur les landing pages Marketo.

**Quelle est la durée de stockage des données pour la création de rapports ?**

90 jours.

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

## Limites de rétention des données du Dynamic Chat {#dynamic-chat-data-retention-limits}

<table>
  <th>Type de données</th>
  <th>Période de rétention</th>
 <tr>
  <td>Un leader anonyme sans engagement</td>
  <td>90 jours</td>
 </tr>
 <tr>
  <td>Activité Objectif</td>
  <td>24 mois</td>
 </tr>
 <tr>
  <td>Activité du document</td>
  <td>24 mois</td>
 </tr>
 <tr>
  <td>Interaction avec l’activité de dialogue</td>
  <td>90 jours</td>
 </tr>
 <tr>
  <td>Activité de réservation de réunion</td>
  <td>24 mois</td>
 </tr>
</table>
