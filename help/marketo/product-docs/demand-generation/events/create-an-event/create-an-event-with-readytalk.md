---
unique-page-id: 2949870
description: Création d’un Événement avec ReadyTalk - Marketo Docs - Documentation du produit
title: Créer un Événement avec ReadyTalk
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# Créer un Événement avec ReadyTalk {#create-an-event-with-readytalk}

>[!PREREQUISITES]
>
>* [Ajouter ReadyTalk en tant que service LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [Créer un Programme de Événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Définir les [actions de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)appropriées pour suivre l&#39;engagement


Configurez d&#39;abord votre événement dans le centre de conférences ReadyTalk. Si vous avez besoin d&#39;aide, consultez le [Centre de ressources ReadyTalk](https://www.readytalk.com/resources/readytalk). Lors du choix du type d&#39;inscription, sélectionnez **pré-inscription avant la réunion**. Si vous sélectionnez _vous inscrire au moment de la réunion_, Marketo **ne saisira pas** un statut enregistré pour votre peuple et n&#39;enregistrera qu&#39;un statut de personne de Participé _après_ la conclusion du webinaire.

Ne cochez pas **m&#39;avertir de nouvelles inscriptions par courrier électronique**.

![](assets/image2015-5-28-21-3a18-3a39.png)

Si vous utilisez ReadyTalk pour envoyer des courriers électroniques de confirmation, vous devez également ajouter une description. Enregistrez votre événement dans ReadyTalk lorsque vous avez terminé.

>[!NOTE]
>
>Pour planifier un Événement assisté par un opérateur, cliquez sur le lien **Demander des services de Événement** situé sur le côté gauche de l&#39;écran d&#39;accueil du centre de conférences pour planifier un événement avec notre équipe de Événements.

Vous êtes maintenant prêt à lier votre événement au marketing.

1. Sélectionnez votre événement, puis cliquez sur **Actions de Événement** et enfin **Paramètres de Événement.**

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >Le type de canal du événement sélectionné doit être **webinar.**

1. Sous **Partenaire de Événement,** sélectionnez **ReadyTalk**.

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. Sous **Connexion,** sélectionnez votre connexion ReadyTalk.

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. Sous **Événement**, sélectionnez le événement à lier, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   Sympa ! Votre événement est maintenant synchronisé.

   >[!NOTE]
   >
   >Les champs envoyés par Marketo sont les suivants : Prénom, Nom, Adresse électronique.

   >[!TIP]
   >
   >Pour renseigner votre message de confirmation avec cette URL unique, utilisez le jeton suivant dans votre message électronique : `{{member.webinar url}}`. Lorsque l’URL de confirmation est envoyée, ce jeton correspond automatiquement à l’URL de confirmation unique de la personne.
   >
   >Définissez votre message de confirmation sur Opérationnel pour vous assurer que les personnes qui s&#39;inscrivent et qui peuvent ne pas s&#39;abonner reçoivent leurs informations de confirmation.

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >Evitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos messages de confirmation. Utilisez plutôt la campagne intelligente du programme de événement, comme illustré ci-dessus.

   >[!TIP]
   >
   >L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps, vous ne voyez toujours rien, sélectionnez **Actualiser à partir du fournisseur de webinaires** dans le menu Actions du Événement de l&#39;onglet **Résumé** de votre événement.

## Affichage de la planification {#viewing-the-schedule}

Dans la vue de Planning du programme, cliquez sur l’entrée de calendrier correspondant à votre événement. Vous pouvez voir la planification sur le côté droit de l&#39;écran !

![](assets/image2015-5-18-12-9-58.png)

Les personnes qui s’abonnent à votre webinaire seront repoussées vers votre fournisseur de webinaires via l’étape de flux Modifier l’état du Programme lorsque le nouvel état est défini sur &quot;Inscrit&quot;. Aucun autre statut ne poussera la personne vers le bas. Veillez également à passer à l’étape 1 du flux d’état du Programme de modification et à l’étape 2 du flux d’envoi de courrier électronique.
