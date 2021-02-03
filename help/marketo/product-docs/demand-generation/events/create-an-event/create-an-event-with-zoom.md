---
unique-page-id: 17728023
description: Création d’un Événement avec Zoom - Docs marketing - Documentation du produit
title: Création d’un Événement avec zoom
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---


# Création d’un Événement avec le zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Ajouter le zoom comme service LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Créer un Programme de Événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Définir les [actions de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)appropriées pour suivre l&#39;engagement


Créez d’abord votre webinaire dans Zoom. Certains paramètres de création de zoom sont utilisés par Marketing et d’autres uniquement par Zoom.

Une fois que vous avez créé un événement Marketo et associé un webinaire Zoom, les systèmes pourront partager les informations d’inscription et de présence. Pour obtenir de l’aide sur la création d’un webinaire, voir [Prise en main des webinaires de zoom](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Entrez les informations suivantes pour votre webinaire et il sera extrait dans Marketo via l&#39;adaptateur. Si vous apportez des modifications à ces informations, vous devez cliquer sur le lien &quot;Actualiser à partir du fournisseur de webinaires&quot; sous Actions du Événement, afin que Marketo puisse voir les modifications.

**Titre et description**

* **Nom**  du webinaire : entrez le nom du webinaire. Ce nom peut être affiché dans Marketing.

* **Description**  (facultatif) - Entrez la description du webinaire. La description sera visible dans Marketo.

**Date et heure**

* **Date**  du début - Entrez votre date de début. Ceci sera visible dans Marketing Cloud.

* **Heure**  du début - Entrez votre heure de début. Ceci sera visible dans Marketing Cloud.

* **Durée**  : entrez la durée. L’heure de début et l’heure de fin seront visibles dans Marketing Cloud.

* **Fuseau**  horaire : sélectionnez le fuseau horaire approprié. Ceci sera visible dans Marketing Cloud.

* **Webinaire** récurrent - Ne cochez pas.

* **Inscription**  - Cochez cette case pour que l&#39;inscription soit obligatoire. Vous utiliserez un landing page/formulaire Marketo pour capturer les informations d’enregistrement qui seront poussées vers le zoom.

>[!NOTE]
>
>Actuellement, Marketo ne prend pas en charge les webinaires récurrents. Vous devez configurer une session unique entre chaque Événement marketing et chaque webinaire de zoom.

![](assets/overview2.png)

>[!TIP]
>
>D’autres champs configurés dans Zoom n’affectent PAS l’intégration. Pour plus d&#39;informations sur ces champs, consultez le [Centre d&#39;aide du webinaire sur le zoom](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar).

Maintenant, passons à Marketo !

1. Sélectionnez un événement. Cliquez sur **Actions de Événement** et sélectionnez **Paramètres de Événement**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Le type de canal du événement sélectionné doit être **webinar**.

1. Choisissez **Zoom** dans la Liste **Événement** **Partenaire**.

   ![](assets/eventsettings1.png)

1. Sélectionnez le compte de zoom auquel vous souhaitez associer votre événement.

   ![](assets/selectaccount.png)

1. Sélectionnez le webinaire.

   ![](assets/selectevent.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/eventsettingssave.png)

   Excellent ! Le événement est désormais synchronisé et planifié par zoom.

   >[!NOTE]
   >
   >Les champs envoyés par Marketo sont les suivants : Prénom, Nom, Adresse électronique.

   >[!TIP]
   >
   >Pour renseigner votre message de confirmation avec cette URL unique, utilisez le jeton suivant dans votre message électronique : `{{member.webinar url}}`. Lorsque l’URL de confirmation est envoyée, ce jeton correspond automatiquement à l’URL de confirmation unique de la personne.
   >
   >Définissez votre message de confirmation sur **Opérationnel** pour vous assurer que les personnes qui s&#39;inscrivent et peuvent ne pas s&#39;abonner reçoivent toujours leurs informations de confirmation.

   Les personnes qui s’inscrivent à votre webinaire seront reportées à votre fournisseur de webinaires par le biais de l’étape de flux **Modifier l’état du Programme** lorsque le nouvel état est défini sur &quot;Inscrit&quot;. Aucun autre statut ne poussera la personne vers le bas. Veillez également à effectuer **Changer l’état du Programme** l’étape de flux 1 et **Envoyer un courriel** l’étape de flux 2.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Evitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos messages de confirmation. Utilisez plutôt la campagne intelligente du programme de événement, comme illustré ci-dessus.

   >[!TIP]
   >
   >L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps, vous ne voyez toujours rien, sélectionnez **Actualiser à partir du fournisseur de webinaires** dans le menu Actions du Événement de l&#39;onglet **Résumé** de votre événement.
