---
description: Présentation de Dynamic Chat - Documents Marketo - Documentation du produit
title: Présentation de la conversation dynamique
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 8aaa6f5225f7965228c3472c0cf6beb2259f3642
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Présentation de la conversation dynamique {#dynamic-chat-overview}

Dynamic Chat vous permet d’utiliser une interface conviviale pour cibler à la fois les personnes et les comptes qui visitent votre site web. Collectez le contenu approprié, tel que le nom, les coordonnées et le texte libre. Les visiteurs du site peuvent également réserver des réunions avec votre équipe de vente. Les données d’activité et d’engagement des conversations dynamiques peuvent être utilisées pour ajouter des membres aux programmes Marketo et déclencher des activités cross-canal.

>[!NOTE]
>
>Dynamic Chat est en cours de déploiement progressif et est actuellement en disponibilité limitée. Cette page sera mise à jour avec les informations de disponibilité générale dès qu&#39;elles seront disponibles.

>[!TIP]
>
>Visite [cette page](https://dcweb.z20.web.core.windows.net/) pour afficher des tutoriels vidéo ainsi qu’une démonstration enregistrée de Dynamic Chat.

## Intégrations {#integrations}

Un composant clé de Dynamic Chat est sa capacité à interagir en mode natif avec votre abonnement Marketo. Pour tirer parti de la fonctionnalité complète de cette intégration, vous devez d’abord lancer la synchronisation des données. Selon la taille de votre base de données Marketo, les données initiales peuvent prendre jusqu’à 24 heures, [synchronisation unique](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) pour terminer.

Les éléments suivants sont synchronisés :

* Données de champ de personne
* Données de champ de l’entreprise
* Données d’activité

## Dialogues {#dialogues}

Les dialogues représentent un seul engagement de discussion. Considérez-le comme un conteneur avec tout ce dont vous avez besoin pour avoir un dialogue de conversation engageant avec les visiteurs de votre site web. Dans chaque dialogue, vous pouvez spécifier la ou les pages sur lesquelles vous souhaitez que le dialogue s’affiche, à qui vous souhaitez qu’il s’affiche, ainsi que le contenu et le flux du dialogue lui-même. En outre, vous pouvez trouver des mesures pour voir les performances de votre dialogue. [En savoir plus sur les boîtes de dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Configuration {#configuration}

Dans l&#39;onglet Configuration , personnalisez l&#39;aspect de vos différents Dialogues. Modifiez la police, les couleurs, le temps de réponse, etc. [En savoir plus sur la configuration](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Calendrier {#calendar}

Dans l’onglet Calendrier , connectez votre calendrier (Outlook ou Gmail) pour l’utiliser dans la planification des rendez-vous dans le chatterbot. Une fois que le calendrier d’un utilisateur est connecté à Dynamic Chat, cet utilisateur est ajouté à la file d’attente et son calendrier est disponible pour que les visiteurs du site web puissent planifier des rendez-vous.

Vous pouvez également personnaliser le corps de l’invitation envoyée au visiteur lorsqu’il planifie un rendez-vous dans le calendrier de l’utilisateur.

## Réunions {#meetings}

C&#39;est là que vous verrez toutes les nominations programmées par les visiteurs de votre site web à travers vos Dialogues. Vous y trouverez l’adresse électronique de la personne ayant réservé la nomination, avec laquelle elle a réservé la nomination, le moment où la nomination est programmée et si la réunion s’est déroulée ou non.

## Routage {#routing}

C’est là que vous pouvez voir la liste de tous les agents qui ont connecté leurs calendriers ainsi que l’ordre dans lequel ils seront présentés aux visiteurs du site web. Les réunions tournent autour du robot, donc si vous avez cinq agents et l&#39;agent trois qui ont pris la dernière réunion, l&#39;agent quatre aura le suivant, suivi de l&#39;agent cinq, puis revenir à l&#39;agent un.

## FAQ {#faq}

**Est-ce que le tchat dynamique permet le chat en direct ?**

Non, il utilise uniquement des réponses prédéterminées.

**Comment cibler les personnes anonymes ?**

Dans votre boîte de dialogue, vous devez utiliser la variable _Le courrier électronique de personne est vide_ attribut.

**Prenez-vous en charge la fonctionnalité AI/NLP ?**

La fonctionnalité AI/NLP n’est pas prise en charge.

**Quelle est la durée de stockage des données pour la création de rapports ?**

90 jours.

**Dynamic Chat offre-t-il des langues autres que l’anglais ?**

Pas pour le moment.
