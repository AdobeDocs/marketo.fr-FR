---
unique-page-id: 10096675
description: Créer des campagnes enfants et Assets local - Documents Marketo - Documentation du produit
title: Création de campagnes enfants et d’Assets locales
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 1%

---

# Création de campagnes enfants et d’Assets locales {#create-child-campaigns-and-local-assets}

Créez vos campagnes enfants et vos ressources locales à l’aide de Design Studio.

## Page d’entrée et formulaire {#landing-page-and-form}

Pour vous assurer que les utilisateurs sont correctement enregistrés auprès de ON24, les champs suivants doivent être inclus dans votre formulaire Marketo :

* Prénom
* Nom
* Adresse e-mail

Vous pouvez également transmettre les champs suivants à ON24 :

* Nom de l’entreprise
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
>Définissez le type de votre email de confirmation sur **Operational** pour vous assurer que les personnes qui s&#39;inscrivent reçoivent leurs informations de confirmation, même si elles sont désabonnées.

>[!TIP]
>
>Vous pouvez configurer ON24 pour envoyer des emails de confirmation, de rappel ou de relance. Pour plus d’informations, consultez le [site d’aide ON24](https://www.on24.com/live-webcast-elite/){target="_blank"} .

## Conditions requises pour l’enregistrement des campagnes enfants {#registration-child-campaign-requirements}

Les événements contiennent une ou plusieurs campagnes enfants qui fonctionnent toutes ensemble pour déplacer les personnes à travers les statuts de programme et vous permettre de suivre les performances de votre événement.

Par exemple, une campagne d’invitation, une campagne d’enregistrement et des campagnes de suivi.

>[!CAUTION]
>
>Pour que l’adaptateur effectue sa tâche, vous DEVEZ créer une campagne d’enregistrement. Cette campagne doit être déclenchée par la personne qui remplit un formulaire. La première étape doit modifier l’état du programme de la personne en **Registered**. L&#39;opération envoie alors un email de confirmation. Consultez le reste de cet article pour plus de détails.

**Enregistrement/Confirmation (campagne de déclenchement)**

* Liste intelligente
* Déclencheur basé sur **Remplit le formulaire**. Veillez à inclure la page d’entrée sur laquelle le formulaire réside en utilisant **Ajouter la contrainte**, en particulier si le même formulaire est utilisé sur plusieurs pages d’entrée.

>[!CAUTION]
>
>Vous devez utiliser un formulaire Marketo pour enregistrer vos utilisateurs pour l’événement, ou un formulaire non Marketo avec l’intégration d’API appropriée pour envoyer les données d’enregistrement vers Marketo. C’est essentiel au succès de l’intégration de votre partenaire d’événement.

>[!NOTE]
>
>Si vous utilisez un formulaire Marketo sur une page d’entrée autre que Marketo, le déclencheur sera **Remplit le formulaire** avec le nom du formulaire.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flux**

* **Modifier l’état du programme** - Défini sur Webinaire -> Enregistré.

Cette étape de flux est requise comme première étape de flux lors de la configuration de votre campagne enfant. Lorsque l’état du programme d’une personne passe à Registered, Marketo transmet les informations d’enregistrement à ON24. Aucun autre statut ne repoussera la personne.

* **Envoyer un courrier électronique** - Confirmation électronique. Définissez cet e-mail sur **Operational** afin que les personnes désabonnées qui se sont enregistrées le reçoivent toujours.

L’étape de flux **Envoyer un courrier électronique** DOIT être la deuxième étape. L’e-mail de confirmation contient le `{{member.webinar url}}`, qui contient des informations renvoyées à Marketo à partir de ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>L’ordre de ces étapes de flux est important en raison de l’ordre dans lequel les actions sont exécutées dans Marketo. L’étape **Modifier l’état du programme** envoie la personne à ON24 pour l’enregistrer et une URL unique est générée. Ensuite, vous pouvez envoyer l’email de confirmation qui inclut cette URL unique à l’aide du jeton `{{member.webinar URL}}`.
>
>Si la personne est renvoyée avec une erreur d’enregistrement, elle ne recevra pas la confirmation par email.

L’étape suivante consiste à [tester votre intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Compréhension des événements d’adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [Exemple d’intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Comprendre les états du programme webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
