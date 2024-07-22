---
unique-page-id: 2949874
description: Créer un événement avec GotoWebinar - Documents Marketo - Documentation du produit
title: Création d’un événement avec GotoWebinar
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Création d’un événement avec GotoWebinar {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [Ajouter GoToWebinar en tant que service LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Créer un programme d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Définissez les [actions de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) appropriées pour effectuer le suivi de l’engagement

Commencez par créer votre webinaire dans GoToWebinar. Certains paramètres de création de votre GoToWebinar sont utilisés par Marketo et d’autres uniquement par GoToWebinar.

Une fois que vous avez créé un événement Marketo et associé le GoToWebinar, les systèmes pourront partager les informations d’inscription et de présence.

Vous trouverez ci-dessous une liste des paramètres utilisés par Marketo.

## Titre et description {#title-and-description}

**Nom du webinaire** : saisissez le nom du webinaire. Ce nom sera visible dans Marketo.

**Description** (facultatif) - saisissez la description du webinaire. La description peut être affichée dans Marketo.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Date et Heure {#date-time}

Renseignez les informations suivantes pour votre webinaire et il sera transmis dans Marketo via l’adaptateur. Si vous apportez des modifications à ces informations, vous devez cliquer sur le lien &quot;**Actualiser à partir du fournisseur de webinaires**&quot; sous **Actions d’événement**, afin que Marketo puisse afficher les modifications.

**Date de début** - entrez votre date de début. Vous pourrez le voir dans Marketo.

**Heure de début** : saisissez l’heure de début. Vous pourrez le voir dans Marketo.

**Heure de fin** : saisissez l’heure de fin. Vous pourrez le voir dans Marketo.

**Fuseau horaire** : sélectionnez le fuseau horaire applicable. Il sera visible dans Marketo.

**Type -** défini sur **Une session**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Actuellement, Marketo ne prend pas en charge les webinaires récurrents. Vous devez configurer une session unique entre chaque événement Marketo et chaque webinaire GoToWebinaire.

>[!TIP]
>
>Si vous avez besoin d’aide supplémentaire sur GoToWebinar, consultez leur [site d’aide](https://support.logmeininc.com/gotowebinar).

Maintenant, passons à Marketo !

1. Sélectionnez un événement. Cliquez sur **Actions d’événement** et sélectionnez **Paramètres d’événement**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >Le type de canal de l’événement sélectionné doit être **webinar**.

1. Sélectionnez **GoToWebinar** dans la liste **Event Partner**.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Sélectionnez le compte.

   ![](assets/rtaimage-2.png)

1. Sélectionnez le webinaire.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. Excellent ! L’événement est maintenant synchronisé et planifié par **GoToWebinar**.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Les champs que Marketo envoie sont les suivants : Prénom, Nom, Adresse électronique. Ces champs sont obligatoires et ne doivent pas être vides.

   >[!TIP]
   >
   >Pour renseigner votre email de confirmation avec cette URL unique, utilisez le jeton suivant dans votre email : `{{member.webinar url}}`. Lorsque l’URL de confirmation est envoyée, ce jeton correspond automatiquement à l’URL de confirmation unique de la personne.
   >
   >Définissez votre email de confirmation sur **Operational** pour vous assurer que les personnes qui s&#39;inscrivent et peuvent se désabonner reçoivent toujours leurs informations de confirmation.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Évitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos emails de confirmation. Utilisez plutôt la campagne dynamique du programme d’événements, comme illustré ci-dessus.

   >[!TIP]
   >
   >L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu aussi longtemps que vous ne voyez toujours rien, sélectionnez **Actualiser à partir du fournisseur de webinaires** dans le menu Actions d’événement dans l’onglet **Résumé** de votre événement.

Les personnes qui s’inscrivent à votre webinaire seront transférées à votre fournisseur de webinaires via l’étape de flux Modifier l’état du programme lorsque le nouvel état est défini sur &quot;Enregistré&quot;. Aucun autre statut ne repoussera la personne. Assurez-vous également d’effectuer l’étape de flux Modifier l’état du programme #1 et l’étape Envoyer un courrier électronique #2.

## Affichage de la planification  {#viewing-the-schedule}

Dans la vue de planification du programme, cliquez sur l’entrée de calendrier de votre événement. Le planning s’affiche dans la partie droite de l’écran.

>[!NOTE]
>
>Pour modifier la planification de votre événement, vous devez modifier le webinaire sur GoToWebinar.

![](assets/image2015-5-14-15-3a3-3a13.png)
