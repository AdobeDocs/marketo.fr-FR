---
unique-page-id: 17728023
description: Création d’un événement avec  [!DNL Zoom] - Documents Marketo - Documentation du produit
title: Créez un événement avec  [!DNL Zoom]
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# Créer un événement avec [!DNL Zoom] {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Ajouter [!DNL Zoom] as a [!DNL LaunchPoint] Service](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Créer un programme d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Définir les [actions de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) appropriées pour suivre l’engagement

Créez d’abord votre webinaire dans [!DNL Zoom]. Certains paramètres de création de votre [!DNL Zoom] sont utilisés par Marketo, tandis que d’autres ne le sont que par [!DNL Zoom].

Après avoir créé un événement Marketo et associé un webinaire [!DNL Zoom] à celui-ci, les systèmes pourront partager les informations d’inscription et de présence. Pour obtenir de l’aide sur la création d’un webinaire, voir [Prise en main  [!DNL Zoom]  webinaires](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Saisissez les informations suivantes pour votre webinaire. Elles seront extraites dans Marketo via l’adaptateur. Si vous apportez des modifications à ces informations, vous devez cliquer sur le lien « Actualiser à partir du fournisseur de webinaires » sous Actions d’événement pour que Marketo voie les modifications.

**Titre et description**

* **Nom du webinaire** - Saisissez le nom du webinaire. Ce nom sera visible dans Marketo.

* **Description** (facultatif) - Saisissez la description du webinaire. La description peut être consultée dans Marketo.

**Date et heure**

* **Date de début** - Saisissez votre date de début. Il sera visible dans Marketo.

* **Heure de début** - Saisissez votre heure de début. Il sera visible dans Marketo.

* **Durée** - Saisissez la durée. L’heure de début et l’heure de fin peuvent être affichées dans Marketo.

* **Fuseau horaire** - Sélectionnez le fuseau horaire applicable. Il sera visible dans Marketo.

* **Webinaire récurrent**- Ne pas cocher.

* **Enregistrement** - Cochez cette case pour que l’enregistrement soit obligatoire. Vous utiliserez un formulaire Marketo ou une page de destination pour capturer les informations d’enregistrement qui seront transmises à [!DNL Zoom].

>[!NOTE]
>
>Marketo ne prend actuellement pas en charge les webinaires récurrents. Vous devez configurer une seule session entre chaque événement Marketo et [!DNL Zoom] webinaire.

![](assets/overview2.png)

>[!TIP]
>
>D’autres champs que vous configurerez dans [!DNL Zoom] n’affecteront PAS l’intégration. Reportez-vous au [[!DNL Zoom] Centre d’aide pour les webinaires](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) pour plus d’informations sur ces champs.

Maintenant, plongeons-nous dans Marketo !

1. Sélectionnez un événement. Cliquez sur **[!UICONTROL Actions d’événement]** et choisissez **[!UICONTROL Paramètres d’événement]**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Le type de canal de l’événement sélectionné doit être **webinaire**.

1. Sélectionnez **[!UICONTROL Zoom]** dans la liste **[!UICONTROL Partenaire de l’événement]**.

   ![](assets/eventsettings1.png)

1. Sélectionnez le compte [!DNL Zoom] auquel vous souhaitez associer votre événement.

   ![](assets/selectaccount.png)

1. Sélectionnez le webinaire .

   ![](assets/selectevent.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/eventsettingssave.png)

   Excellent ! Désormais, l’événement est synchronisé et planifié par [!DNL Zoom].

   >[!NOTE]
   >
   >Les champs envoyés par Marketo sont les suivants : Prénom, Nom, Adresse e-mail.

   >[!TIP]
   >
   >Pour remplir votre e-mail de confirmation avec cette URL unique, utilisez le jeton suivant dans votre e-mail : `{{member.webinar url}}`. Lorsque l’URL de confirmation est envoyée, ce jeton est automatiquement résolu sur l’URL de confirmation unique de la personne.
   >
   >Définissez votre e-mail de confirmation sur **Opérationnel** afin de vous assurer que les personnes qui s’inscrivent et peuvent se désinscrire reçoivent toujours leurs informations de confirmation.

   Les personnes qui s’inscrivent à votre webinaire sont redirigées vers votre fournisseur de webinaires via l’étape de flux **[!UICONTROL Modifier le statut du programme]** lorsque le [!UICONTROL Nouveau statut] est défini sur « Enregistré ». Aucun autre statut ne poussera la personne vers le serveur. Veillez également à ce que les étapes de flux **[!UICONTROL Modifier le statut du programme]** #1 et **[!UICONTROL Envoyer un e-mail]** soient #2.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Évitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos e-mails de confirmation. Utilisez plutôt la campagne intelligente du programme d’événement, comme illustré ci-dessus.

   >[!TIP]
   >
   >L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps, vous ne voyez toujours rien, sélectionnez **Actualiser à partir du fournisseur de webinaires** dans le menu Actions de l’événement de l’onglet **Résumé** de votre événement, puis cliquez sur l’icône d’actualisation en bas à droite de l’écran.
