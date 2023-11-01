---
unique-page-id: 2949863
description: Création d’un événement avec Webex - Documents Marketo - Documentation du produit
title: Création d’un événement avec Webex
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 1%

---

# Création d’un événement avec Webex {#create-an-event-with-webex}

Après avoir créé un webinaire dans Webex, vous devrez synchroniser votre événement avec Marketo Engage.

>[!PREREQUISITES]
>
>* [Ajout de Webex en tant que service LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Création d’un programme d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Définissez les [actions de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) pour suivre l’engagement

## Planification de votre webinaire {#schedule-your-webinar}

Vous planifiez votre événement et choisissez vos paramètres préférés dans la section [Webex](https://www.webex.com/){target="_blank"}. Only the following information is viewable in Marketo: webinar name, start/end date & time, time zone, and description. Additional information about Webex Webinars [can be found here](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

### Informations de base {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **Rubrique**: il s’agit du nom de votre événement et il sera visible dans Marketo.
* **Date et heure**: la date de début/fin, l’heure de début/fin, la durée et le fuseau horaire sont tous visibles dans Marketo.
* **Nombre maximal de participants**: le nombre maximal de participants détermine les fonctionnalités Webex prises en charge.
* **Vue Web pour les participants**: cochez cette case pour que votre webinaire soit diffusé en direct à tous les participants.
* **Panelistes**: invitez des personnes spécifiques à être membres de groupes sur votre webinaire.
* **Programme du webinaire**: renseignez cette variable si vous souhaitez fournir un contexte dans l’invitation par courrier électronique envoyée aux listes.

### Sécurité {#security}

![](assets/create-an-event-with-webex-2.png)

* **Mot de passe du séminaire**: (facultatif) si vous utilisez ce champ, veillez à l’inclure dans votre email de confirmation.
* **Mot de passe du panneau**: (facultatif) si vous utilisez ce champ, veillez à l’inclure dans votre agenda de webinaire.
* **Compte requis**: limite les participants aux seuls comptes Webex.

### Options de connexion audio {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **Type de connexion audio**: choisissez comment les participants au webinaire rejoignent la partie audio de votre webinaire.
* **Tons d’entrée et de sortie**: sélectionnez le son que vous souhaitez pour les utilisateurs lorsqu’une personne entre dans le webinaire ou en sort (connexion audio par téléphone requise).
* **Liste déroulante**: sélectionnez les paramètres de mise en sourdine de votre choix.

### Options avancées {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **Enregistrement automatique**: cochez cette case pour que votre webinaire soit automatiquement enregistré.
* **Session de pratique**: cochez cette option pour qu’une session d’entraînement démarre au début du webinaire.
* **Sessions de ventilation**: les sessions de ventilation vous permettent de préaffecter des groupes de discussion et des participants avant le démarrage du webinaire, ou de leur permettre de participer au webinaire.
* **Série de webinaires**: l’ajout à une série de webinaires permet aux utilisateurs de visionner votre webinaire, qu’il soit public ou non.
* **Enregistrement**: nécessite que les participants s’enregistrent et reçoivent la validation de l’hôte avant de participer.
* **Rappel email**: choisissez un rappel par email compris entre 15 minutes et le début du webinaire jusqu’à deux jours.
* **Options de webinaire**: déterminez les fonctionnalités disponibles pour les participants au webinaire.
* **Privilèges de participant**: les privilèges des participants déterminent les actions disponibles pour les participants au webinaire.

>[!NOTE]
>
>L’intégration Marketo-Webex ne peut pas prendre en charge l’envoi d’emails de confirmation en dehors de Webex. La confirmation doit être envoyée via Marketo. Après avoir planifié l’événement, veillez à copier les informations de l’événement dans l’e-mail de confirmation de Marketo et à définir l’e-mail sur _Fonctionnement_.

## Synchronisation de votre événement avec Marketo Engage {#sync-your-event-with-marketo-engage}

1. Dans Marketo, recherchez et sélectionnez le programme d’événements de votre choix. Dans le **Actions d’événement** , sélectionnez **Paramètres d’événement**.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >Le type de canal de l’événement sélectionné doit être **webinaire**.

1. Dans le **Partenaire d’événement** , sélectionnez **Webinaires Webex**.

   ![](assets/create-an-event-with-webex-6.png)

1. Dans le **Connexion** , sélectionnez votre connexion WebEx.

   ![](assets/create-an-event-with-webex-7.png)

1. Dans le **Événement** , choisissez votre événement Webex.

   ![](assets/create-an-event-with-webex-8.png)

1. Les détails de votre webinaire seront renseignés. Cliquez sur **Enregistrer**.

   ![](assets/create-an-event-with-webex-9.png)

Votre événement Webex est maintenant synchronisé avec votre programme d’événements Marketo. Les personnes qui s’inscrivent à votre webinaire seront retransmises à votre fournisseur de webinaires via le _Modifier l’état du programme_ étape de flux lorsque le nouvel état est défini sur &quot;Registered&quot;. Aucun autre statut ne repoussera la personne. Veillez à _Modifier l’état du programme_ #1 de l’étape de flux et _Envoyer un courrier électronique_ #2 étape de flux.

## Informations à noter {#things-to-note}

* Évitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos emails de confirmation. Utilisez plutôt la campagne dynamique de votre programme d’événements.

* L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps, vous ne voyez toujours rien, cliquez sur **Actualisation à partir du fournisseur de webinaire** dans le **Actions d’événement** dans la **Résumé** de votre programme d’événements.
