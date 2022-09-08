---
unique-page-id: 10096675
description: Créer des campagnes enfants et des ressources locales - Documents Marketo - Documentation du produit
title: Créer des campagnes enfants et des ressources locales
exl-id: 272105e1-43d6-455c-a533-aae65e859384
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 1%

---

# Créer des campagnes enfants et des ressources locales {#create-child-campaigns-and-local-assets}

>[!IMPORTANT]
>
>Depuis août 2022, ON24 ne prend plus en charge les nouvelles intégrations Marketo. Les informations de cet article s’appliquent uniquement aux utilisateurs existants.

Créez vos campagnes enfants et vos ressources locales à l’aide de Design Studio.

## Page d’entrée et formulaire {#landing-page-and-form}

Pour vous assurer que les utilisateurs sont correctement enregistrés auprès de ON24, les champs suivants doivent être inclus dans votre formulaire Marketo :

* Prénom
* Nom
* Adresse e-mail

Vous pouvez également transmettre les champs suivants à ON24 :

* Nom de la société
* Intitulé du poste

Une fois l’étape de flux appropriée ajoutée à la campagne d’enregistrement, les personnes sont transférées vers ON24 et marquées comme étant enregistrées. Vous pouvez ajouter d’autres champs au formulaire et les informations seront capturées dans Marketo dans le cadre de l’enregistrement des détails de la personne.

>[!CAUTION]
>
>Pour une intégration réussie, vous devez utiliser un formulaire Marketo pour enregistrer vos personnes pour l’événement, ou un formulaire non Marketo avec l’intégration d’API appropriée pour transmettre les données d’enregistrement à Marketo.

## Emails et jetons d’URL {#emails-and-url-tokens}

Créez l’invitation, la confirmation, le suivi et remerciez les emails à l’aide de Marketo.

## Marketo Confirmation Email et jeton URL {#marketo-confirmation-email-and-url-token}

Utilisez Marketo pour envoyer l’e-mail de confirmation de votre événement. Lorsqu’une personne s’inscrit, elle reçoit une URL unique à utiliser pour entrer dans l’événement.

>[!NOTE]
>
>Pour renseigner votre email de confirmation avec cette URL unique, utilisez le jeton suivant dans votre email : `{{member.webinar url}}`. Lorsque vous envoyez l’URL de confirmation, ce jeton correspond automatiquement à l’URL de confirmation unique de la personne.
>
>Définissez le type de votre email de confirmation sur **Opérationnel** pour s&#39;assurer que les personnes qui s&#39;inscrivent reçoivent leurs informations de confirmation, même si elles sont désabonnées.

>[!TIP]
>
>Vous pouvez configurer ON24 pour envoyer des emails de confirmation, de rappel ou de relance. Voir [Site d’aide ON24](https://www.on24.com/live-webcast-elite/) pour plus d’informations.

## Exigences d’enregistrement des campagnes enfants {#registration-child-campaign-requirements}

Les événements contiennent une ou plusieurs campagnes enfants qui fonctionnent toutes ensemble pour déplacer les personnes à travers les statuts de programme et vous permettre de suivre les performances de votre événement.

Par exemple, une campagne d’invitation, une campagne d’enregistrement et des campagnes de suivi.

>[!CAUTION]
>
>Pour que l’adaptateur effectue sa tâche, vous DEVEZ créer une campagne d’enregistrement. Cette campagne doit être déclenchée par la personne qui remplit un formulaire. La première étape doit modifier l’état du programme de la personne en **Inscrits**. L&#39;opération envoie alors un email de confirmation. Consultez le reste de cet article pour plus de détails.

**Enregistrement/Confirmation (campagne de déclenchement)**

* Liste intelligente
* Déclencheur basé sur **Remplir le formulaire**. Veillez à inclure la page d’entrée sur laquelle se trouve le formulaire en utilisant **Ajouter une contrainte**, en particulier si le même formulaire est utilisé sur plusieurs landing pages.

>[!CAUTION]
>
>Vous devez utiliser un formulaire Marketo pour enregistrer vos utilisateurs pour l’événement, ou un formulaire non Marketo avec l’intégration d’API appropriée pour envoyer les données d’enregistrement vers Marketo. C’est essentiel au succès de l’intégration de votre partenaire d’événement.

>[!NOTE]
>
>Si vous utilisez un formulaire Marketo sur une page d’entrée autre que Marketo, votre déclencheur sera **Remplir le formulaire** par le nom du formulaire.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flux**

* **Modifier l’état du programme** - Défini sur Webinaire -> Enregistré.

Cette étape de flux est requise comme première étape de flux lors de la configuration de votre campagne enfant. Lorsque l’état du programme d’une personne passe à Registered, Marketo transmet les informations d’enregistrement à ON24. Aucun autre statut ne repoussera la personne.

* **Envoyer un courrier électronique** - Adresse électronique de confirmation. Définissez cet e-mail sur **Opérationnel** pour que les personnes désinscrites qui se sont inscrites continuent de le recevoir.

Le **Envoyer un courrier électronique** étape de flux DOIT être la deuxième étape. L’e-mail de confirmation contient la variable `{{member.webinar url}}`, qui est renseignée avec les informations renvoyées à Marketo à partir de ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>L’ordre de ces étapes de flux est important en raison de l’ordre dans lequel les actions sont exécutées dans Marketo. Le **Modifier l’état du programme** L’étape envoie la personne à ON24 pour l’enregistrer et une URL unique est générée. Ensuite, vous pouvez envoyer l’e-mail de confirmation contenant cette URL unique à l’aide de la variable `{{member.webinar URL}}` jeton.
>
>Si la personne est renvoyée avec une erreur d’enregistrement, elle ne recevra pas la confirmation par email.

L’étape suivante consiste à [test de l’intégration de votre événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md).

>[!MORELIKETHIS]
>
>* [Présentation des événements de l’adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [Exemple d’intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Présentation des états du programme du webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

