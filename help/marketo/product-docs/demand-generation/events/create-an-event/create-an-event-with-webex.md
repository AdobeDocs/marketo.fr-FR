---
unique-page-id: 2949863
description: Création d’un événement avec Webex - Documents Marketo - Documentation du produit
title: Création d’un événement avec Webex
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# Création d’un événement avec Webex {#create-an-event-with-webex}

Après avoir créé un webinaire dans Webex, vous devrez synchroniser votre événement avec Marketo Engage.

>[!PREREQUISITES]
>
>* [Ajouter Webex en tant que service LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Créer un programme d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Définissez les [actions de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) appropriées pour suivre l’engagement

## Planification de votre webinaire {#schedule-your-webinar}

Vous planifiez votre événement et choisissez vos paramètres préférés dans [Webex](https://www.webex.com/){target="_blank"}. Seules les informations suivantes sont visibles dans Marketo : nom du webinaire, date et heure de début/fin, fuseau horaire et description. Vous trouverez des informations supplémentaires sur les webex Webinars [ici](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

### Informations de base {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **Topic** : il s’agit de votre nom d’événement et il sera consultable dans Marketo.
* **Date et heure** : date de début/fin, heure de début/fin, durée et fuseau horaire sont tous visibles dans Marketo.
* **Nombre maximal de participants** : le nombre maximal de participants détermine les fonctionnalités Webex prises en charge.
* **Affichage Web pour les participants** : cochez cette option pour que votre webinaire soit diffusé en direct à tous les participants.
* **Panelistes** : invitez des personnes spécifiques à être membres de groupes sur votre webinaire.
* **Programme webinaire** : renseignez ce champ si vous souhaitez fournir du contexte dans l’invitation par courrier électronique envoyée aux listes.

### Sécurité {#security}

![](assets/create-an-event-with-webex-2.png)

* **Mot de passe du webinaire** : (facultatif) Si vous utilisez ce champ, veillez à l’inclure dans votre email de confirmation.
* **Mot de passe du webinaire** : (facultatif) Si vous utilisez ce champ, veillez à l’inclure dans votre agenda de webinaires.
* **Require account** : limite les participants aux seuls comptes Webex.

### Options de connexion audio {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **Type de connexion audio** : choisissez comment les participants au webinaire rejoignent la partie audio de votre webinaire.
* **Tons d’entrée et de sortie** : sélectionnez le son que vous souhaitez pour les utilisateurs lorsqu’une personne entre dans le webinaire ou en sort (connexion audio par téléphone requise).
* **Panelliste muet** : sélectionnez les paramètres de muet de votre choix.

### Options avancées {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **Enregistrement automatique** : cochez cette case pour que votre webinaire soit enregistré automatiquement.
* **Session d’entraînement** : cochez cette option pour qu’une session d’entraînement démarre au début du webinaire.
* **Sessions de ventilation** : les sessions de ventilation vous permettent de préaffecter des groupes et des participants avant le début du webinaire, ou de les autoriser à se joindre au cours du webinaire.
* **Série de webinaires** : l’ajout à une série de webinaires permet aux utilisateurs de voir votre webinaire s’il est public ou non.
* **Enregistrement** : nécessite que les participants s’enregistrent et reçoivent l’approbation de l’hôte avant d’assister.
* **Rappel d’email** : choisissez un rappel d’email allant de 15 minutes avant que le webinaire ne commence jusqu’à deux jours.
* **Options de webinaire** : déterminez les fonctionnalités disponibles pour les participants au webinaire.
* **Droits de participant** : les privilèges de participant déterminent les actions disponibles pour les participants au webinaire.

>[!NOTE]
>
>L’intégration Marketo-Webex ne peut pas prendre en charge l’envoi d’emails de confirmation en dehors de Webex. La confirmation doit être envoyée via Marketo. Après avoir planifié l’événement, veillez à copier les informations d’événement dans l’e-mail de confirmation Marketo et à définir l’e-mail sur _Operational_.

## Synchronisation de votre événement avec Marketo Engage {#sync-your-event-with-marketo-engage}

1. Dans Marketo, recherchez et sélectionnez le programme d’événements de votre choix. Dans la liste déroulante **Actions d’événement**, sélectionnez **Paramètres d’événement**.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >Le type de canal de l’événement sélectionné doit être **webinar**.

1. Dans la liste déroulante **Event Partner**, sélectionnez **Webex Webinars**.

   ![](assets/create-an-event-with-webex-6.png)

1. Dans la liste déroulante **Connexion**, sélectionnez votre connexion Webex.

   ![](assets/create-an-event-with-webex-7.png)

1. Dans la liste déroulante **Event**, choisissez votre événement Webex.

   ![](assets/create-an-event-with-webex-8.png)

1. Les détails de votre webinaire seront renseignés. Cliquez sur **Enregistrer**.

   ![](assets/create-an-event-with-webex-9.png)

Votre événement Webex est maintenant synchronisé avec votre programme d’événements Marketo. Les personnes qui s’inscrivent à votre webinaire seront transférées à votre fournisseur de webinaires via l’étape de flux _Modifier l’état du programme_ lorsque le nouvel état est défini sur &quot;Enregistré&quot;. Aucun autre statut ne repoussera la personne. Veillez à effectuer l’étape de flux _Modifier l’état du programme_ #1 et l’étape de flux _Envoyer un courrier électronique_ #2.

## Informations à noter {#things-to-note}

* Évitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos emails de confirmation. Utilisez plutôt la campagne dynamique de votre programme d’événements.

* L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps que vous ne voyez toujours rien, cliquez sur **Actualiser à partir du fournisseur de webinaires** dans la liste déroulante **Actions d’événement** de l’onglet **Résumé** de votre programme d’événements.
