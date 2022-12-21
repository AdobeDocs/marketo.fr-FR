---
unique-page-id: 17728023
description: Création d’un événement avec zoom - Documents Marketo - Documentation du produit
title: Création d’un événement avec zoom
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Création d’un événement avec zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Ajout de Zoom comme service LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Création d’un programme d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Définissez les [actions de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)pour suivre l’engagement


Commencez par créer votre webinaire dans Zoom. Certains paramètres de création de votre zoom sont utilisés par Marketo, d’autres uniquement par zoom.

Après avoir créé un événement Marketo et associé un webinaire Zoom, les systèmes pourront partager les informations d’inscription et de présence. Pour obtenir de l’aide sur la création d’un webinaire, voir  [Prise en main des webinaires de zoom](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Renseignez les informations suivantes pour votre webinaire et il sera transmis dans Marketo via l’adaptateur. Si vous apportez des modifications à ces informations, vous devez cliquer sur le lien &quot;Actualiser à partir du fournisseur de webinaires&quot; sous Actions d’événement afin que Marketo puisse voir les modifications.

**Titre et description**

* **Nom du webinaire** - Saisissez le nom du webinaire. Ce nom sera visible dans Marketo.

* **Description** (facultatif) - Entrez la description du webinaire. La description peut être affichée dans Marketo.

**Date et Heure**

* **Date de début** - Entrez votre date de début. Vous pourrez le voir dans Marketo.

* **Heure de début** - Saisissez votre heure de début. Vous pourrez le voir dans Marketo.

* **Durée** - Saisissez la durée. Les heures de début et de fin seront visibles dans Marketo.

* **Fuseau horaire** - Sélectionnez le fuseau horaire applicable. Vous pourrez le voir dans Marketo.

* **Webinaire récurrent**- Ne cochez pas.

* **Enregistrement** - Cochez cette case pour que l’enregistrement soit obligatoire. Vous utiliserez un formulaire Marketo ou une landing page pour capturer les informations d’enregistrement qui seront poussées vers Zoom.

>[!NOTE]
>
>Actuellement, Marketo ne prend pas en charge les webinaires récurrents. Vous devez configurer une session unique entre chaque webinaire Événement Marketo et Zoom .

![](assets/overview2.png)

>[!TIP]
>
>D’autres champs que vous allez configurer dans Zoom n’auront AUCUN impact sur l’intégration. Reportez-vous à la section [Centre d’aide du webinaire Zoom](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) pour plus d&#39;informations sur ces champs.

Maintenant, passons à Marketo !

1. Sélectionnez un événement. Cliquez sur **Actions d’événement** et choisissez **Paramètres d’événement**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Le type de canal de l’événement sélectionné doit être **webinaire**.

1. Choisir **Zoom** de la **Événement** **Partenaire** Liste.

   ![](assets/eventsettings1.png)

1. Sélectionnez le compte de zoom auquel vous souhaitez associer votre événement.

   ![](assets/selectaccount.png)

1. Sélectionnez le webinaire.

   ![](assets/selectevent.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/eventsettingssave.png)

   Excellent ! Désormais, l’événement est synchronisé et planifié par zoom.

   >[!NOTE]
   >
   >Les champs que Marketo envoie sont les suivants : Prénom, Nom, Adresse électronique.

   >[!TIP]
   >
   >Pour renseigner votre email de confirmation avec cette URL unique, utilisez le jeton suivant dans votre email : `{{member.webinar url}}`. Lorsque l’URL de confirmation est envoyée, ce jeton correspond automatiquement à l’URL de confirmation unique de la personne.
   >
   >Définissez votre adresse électronique de confirmation sur **Opérationnel** afin de s&#39;assurer que les personnes qui s&#39;inscrivent et peuvent se désinscrire reçoivent toujours leurs informations de confirmation.

   Les personnes qui s’inscrivent à votre webinaire seront retransmises à votre fournisseur de webinaires via le **Modifier l’état du programme** étape de flux lorsque le nouvel état est défini sur &quot;Registered&quot;. Aucun autre statut ne repoussera la personne. Veillez également à **Modifier l’état du programme** #1 étape de flux et **Envoyer un courrier électronique** #2 étape de flux.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Évitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos emails de confirmation. Utilisez plutôt la campagne dynamique du programme d’événements, comme illustré ci-dessus.

   >[!TIP]
   >
   >L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps, vous ne voyez toujours rien, sélectionnez **Actualisation à partir du fournisseur de webinaire** à partir du menu Actions d’événement dans la **Résumé** de votre événement.
