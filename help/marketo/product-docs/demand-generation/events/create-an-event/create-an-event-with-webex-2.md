---
description: Création d’un événement avec Webex - Documents Marketo - Documentation du produit
title: Création d’un événement avec Webex
hide: true
hidefromtoc: true
feature: Events
source-git-commit: e21450610146eea3a14761a7365a35d9cacee523
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Création d’un événement avec Webex {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Ajout de Webex en tant que service LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Création d’un programme d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Définissez les [actions de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) pour suivre l’engagement
>* Assurez-vous d’utiliser les événements Webex (Classic)

Tout d’abord, créez un webinaire dans [Webex](https://www.webex.com/){target="_blank"}. Event in the Webex Event Center. Marketo only uses specific settings and fields for your integration, which we'll go through shortly. Other fields that you might want to configure for Webex are explained in the [Webex Event Center User Guide](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf){target="_blank"}.

>[!IMPORTANT]
>
>Marketo Engage ne prend en charge que les événements créés dans les événements Webex (Classic). Marketo ne prend pas en charge les événements créés dans les événements Webex (nouveaux) pour le moment.

## Informations de base {#basic-information}

* **Nom de l’événement -** Ce nom sera visible dans Marketo.
* **Case à cocher non répertoriée**

   * Il est recommandé de le faire. **not** répertorie votre événement. Cela permet de s’assurer que tous les utilisateurs s’enregistrent via votre page d’entrée Marketo. Les personnes qui s’inscrivent par le biais d’un mécanisme autre que Marketo s’afficheront dans Marketo une fois l’événement terminé ET uniquement si elles ont participé à l’événement.
   * Si vous choisissez de répertorier l’événement, celui-ci apparaîtra sur la page Liste des événements pour toute personne visitant votre site Web Event Center.

* **Registration -** Cochez cette case pour définir sur &quot;obligatoire&quot;. Vous utiliserez un formulaire Marketo ou une landing page pour capturer les informations d’enregistrement qui seront transmises à Webex.
* **Mot de passe d’événement**- (facultatif) Si vous utilisez ce champ, veillez à l’inclure dans votre email de confirmation.

![](assets/image2015-5-28-13-3a30-3a55.png)

## Date et Heure {#date-time}

* **Date de début** - Entrez votre date de début. Vous pourrez le voir dans Marketo.

* **Heure de début** - Saisissez votre heure de début. Vous pourrez le voir dans Marketo.

* **Durée estimée** - Indiquez la durée de l’événement. Vous pourrez le voir dans Marketo.

* **Fuseaux horaires** - Renseignez les fuseaux horaires applicables. Ils seront visibles dans Marketo.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Paramètres de conférence audio {#audio-conference-settings}

Ces paramètres résident uniquement dans Webex. Ils ne sont pas utilisés ou visibles dans Marketo, mais ils peuvent être importants pour votre webinaire. Vérifiez-les donc deux fois !

## Description et options de l’événement  {#event-description-options}

Les options suivantes sont utilisées ou visibles dans Marketo. Les autres champs résident uniquement dans Webex.

* **Description** - Entrez une description. Il sera visible, mais ne pourra pas être modifié dans Marketo.
* **Questionnaire post-événement** - Actuellement, Marketo ne peut pas capturer les informations d’une enquête post-événement Webex.
* **URL de destination** - (facultatif) Vous pouvez saisir l’URL d’une page d’entrée Marketo qui servira d’URL de destination à afficher une fois la session terminée.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Participants et inscription {#attendees-registration}

Vous pourrez contrôler la liste d’invitation, le formulaire d’enregistrement et d’autres courriers électroniques à l’aide d’un événement Marketo. Marketo ne prendra pas en charge d’autres fonctionnalités, notamment :

* **Nombre maximum d&#39;inscrits** - Actuellement **not** pris en charge à l’aide de l’intégration Marketo-Webex.  L’approbation manuelle des inscrits est disponible à l’aide de l’état de progression Approbation en attente dans Marketo.

* **ID d’enregistrement requis** - Actuellement pris en charge à l’aide de l’intégration Marketo-Webex. Vous pouvez utiliser Marketo pour envoyer l’e-mail de confirmation de votre événement. Lorsque la personne s’inscrit, elle reçoit une URL unique qu’elle utilise pour entrer dans l’événement.

  >[!TIP]
  >
  >Pour renseigner votre email de confirmation avec cette URL unique, utilisez le jeton suivant dans votre email : `{{member.webinar url}}`. Lorsque l’URL de confirmation est envoyée, ce jeton correspond automatiquement à l’URL de confirmation unique de la personne.
  >
  >Définissez votre adresse électronique de confirmation sur **Fonctionnement** afin de s&#39;assurer que les personnes qui s&#39;inscrivent et peuvent se désinscrire reçoivent toujours leurs informations de confirmation.

* **Mot de passe d’enregistrement** - (Facultatif) Actuellement non pris en charge à l’aide de l’intégration Marketo-Webex.
* **Règles de validation** - Actuellement non pris en charge à l’aide de l’intégration Marketo-Webex. Cependant, vous pouvez utiliser des campagnes intelligentes dans Marketo pour contrôler les approbations.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Présentateurs et panélistes {#presenters-panelists}

Les informations configurées dans cette section ne sont pas transmises à Marketo.

### Messages e-mail {#email-messages}

Vous utiliserez Marketo pour envoyer des emails à vos inscrits, des emails de confirmation, etc. Vous n’avez rien à configurer dans cette section. Désactivez (décochez) les options de message électronique dans Webex.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>L’intégration Marketo-Webex ne peut pas prendre en charge l’envoi d’emails de confirmation en dehors de Webex. La confirmation doit être envoyée via Marketo. Après avoir planifié l’événement, veillez à copier les informations de l’événement dans l’e-mail de confirmation de Marketo et à définir l’e-mail sur **Fonctionnement**.

Maintenant, nous sommes prêts à entrer dans Marketo !

1. Sélectionnez l’événement que vous avez créé. Ouvrez le **Actions d’événement** menu déroulant. Choisir **Paramètres d’événement.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >Le type de canal de l’événement sélectionné doit être **webinaire**.

1. Sous **Partenaire d’événement**, sélectionnez **Webex**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. Sous **Connexion**, sélectionnez votre connexion WebEx.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. Sous **Événement**, choisissez l’événement Webex que vous venez de créer. Sélectionnez ensuite une page de sauvegarde facultative, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Sélectionnez une page de sauvegarde facultative pour votre événement Webex. Choisissez parmi la liste déroulante des landing pages Marketo validées ou saisissez l&#39;URL d&#39;une landing page non Marketo.

   >[!TIP]
   >
   >Définissez une page de sauvegarde pour diriger un membre vers une page spécifique s’il clique sur l’URL de son événement personnalisé avant l’heure de début de l’événement.

   >[!NOTE]
   >
   >Les champs que Marketo envoie sont les suivants : Prénom, Nom, Adresse électronique.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Évitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos emails de confirmation. Utilisez plutôt la campagne dynamique du programme d’événements, comme illustré ci-dessus.

   >[!TIP]
   >
   >L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps, vous ne voyez toujours rien, sélectionnez **Actualisation à partir du fournisseur de webinaire** à partir du menu Actions d’événement dans la **Résumé** de votre événement.

Doux ! Votre événement Webex est maintenant synchronisé avec votre événement Marketo. Les personnes qui s’inscrivent à votre webinaire seront transférées à votre fournisseur de webinaires via l’étape de flux Modifier l’état du programme lorsque le nouvel état est défini sur &quot;Enregistré&quot;. Aucun autre statut ne repoussera la personne. Assurez-vous également d’effectuer l’étape de flux Modifier l’état du programme #1 et l’étape Envoyer un courrier électronique #2.

## Affichage de la planification  {#viewing-the-schedule}

Dans la vue de planification du programme, cliquez sur l’entrée de calendrier de votre événement. Vous pouvez voir le planning sur le côté droit de l&#39;écran !

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Pour modifier la planification de votre événement, vous devez modifier le webinaire sur Webex.
