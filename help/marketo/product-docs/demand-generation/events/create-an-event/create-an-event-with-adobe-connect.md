---
unique-page-id: 2949865
description: Création d’un Événement avec Adobe Connect - Marketo Docs - Documentation du produit
title: Créer un Événement avec Adobe Connect
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# Créer un Événement avec Adobe Connect {#create-an-event-with-adobe-connect}

La synchronisation avec Adobe Connect vous permet de gérer votre inscription et votre participation au webinaire dans Marketo, ce qui garantit que l’engagement ne sera pas non suivi.

>[!PREREQUISITES]
>
>* [Lier Adobe Connect et Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Créer un Programme de Événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


Tout d&#39;abord, assurez-vous d&#39;avoir créé votre réunion ou séminaire à Adobe Connect. Si vous avez besoin d&#39;aide, consultez le Guide [de l&#39;utilisateur](http://help.adobe.com/en_US/connect/9.0/using/index.html)Adobe Connect. Les réunions et séminaires que vous créez en Adobe Connect doivent être créés dans le dossier que vous avez spécifié lorsque vous avez saisi vos informations d’identification dans Marketing Cloud. Après avoir créé votre réunion ou séminaire, prenez note de toute information logistique pertinente (telle que le numéro de téléphone) à utiliser dans votre courriel de confirmation et votre fichier ICS.

>[!NOTE]
>
>Pour le **moment, nous ne prenons pas** en charge Adobe Connect On-Site.

1. Sur la page d’accueil d’un nouveau événement, sélectionnez Actions **de**&#x200B;Événement, puis Paramètres **de**&#x200B;Événement.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Si les paramètres **de** Événement ne s’affichent pas dans la liste déroulante, assurez-vous que le canal de événement a **Événement avec le webinaire** sélectionné sous &quot;S’applique à&quot;.

1. Sous **Événement Partner**, sélectionnez **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Sélectionnez votre **ID de connexion** et votre **Événement**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/event-settings-overview.png)

   Sympa ! Votre événement Adobe Connect est désormais synchronisé avec votre événement Marketing.

   >[!NOTE]
   >
   >Les champs envoyés par Marketo sont les suivants : Prénom, Nom, Adresse électronique.

   >[!TIP]
   >
   >Pour insérer l’URL unique de la personne dans un courrier électronique, utilisez ce jeton : `{{member.webinar url}}`. Lorsque le courrier électronique est envoyé, ce jeton résout automatiquement l’URL de confirmation unique de la personne en provenance d’Adobe Connect.
   >
   >Définissez votre message de confirmation sur **Operational** pour vous assurer que les personnes qui s&#39;inscrivent et peuvent être désabonnées reçoivent toujours leurs informations de confirmation.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Evitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos messages de confirmation. Utilisez plutôt la campagne intelligente du programme de événement, comme illustré ci-dessus.

   >[!TIP]
   >
   >L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps, vous ne voyez toujours rien, sélectionnez **Actualiser à partir du fournisseur** de webinaires dans le menu Actions de Événement de l’onglet Résumé de votre événement.

   >[!MORELIKETHIS]
   >
   > * [Ajouter Adobe Connect en tant que service LaunchPoint](../../../../product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   > * [Modification d’un Canal de Événement](../../../../product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)


Les personnes qui s’abonnent à votre webinaire seront repoussées vers votre fournisseur de webinaires via l’étape de flux Modifier l’état du Programme lorsque le nouvel état est défini sur &quot;Inscrit&quot;. Aucun autre statut ne poussera la personne vers le bas. Veillez également à passer à l’étape 1 du flux d’état du Programme de modification et à l’étape 2 du flux d’envoi de courrier électronique.
