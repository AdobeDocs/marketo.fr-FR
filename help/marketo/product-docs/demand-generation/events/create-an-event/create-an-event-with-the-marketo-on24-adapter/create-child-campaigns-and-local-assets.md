---
unique-page-id: 10096675
description: Créer des campagnes enfants et des Assets locales - Documents Marketo - Documentation du produit
title: Créer des campagnes enfant et des ressources locales
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 3%

---

# Créer des campagnes enfant et des ressources locales {#create-child-campaigns-and-local-assets}

Créez vos campagnes enfants et vos ressources locales à l’aide de Design Studio.

## Page de destination et formulaire {#landing-page-and-form}

Pour vous assurer que les utilisateurs sont correctement inscrits auprès de ON24, les champs suivants doivent être inclus dans votre formulaire Marketo :

* Prénom
* Nom
* Adresse e-mail

Vous pouvez également pousser les champs suivants vers ON24 :

* Nom de la société
* Intitulé du poste

Avec l’étape de flux appropriée ajoutée à la campagne d’enregistrement, les personnes seront redirigées vers ON24 et seront marquées comme enregistrées. Vous pouvez ajouter d’autres champs au formulaire et les informations seront capturées dans Marketo dans le cadre de l’enregistrement des détails de la personne.

>[!CAUTION]
>
>Pour une intégration réussie, vous devez utiliser un formulaire Marketo pour inscrire vos membres à l’événement ou un formulaire autre que Marketo avec l’intégration d’API appropriée pour transmettre les données d’enregistrement à Marketo.

## E-mails et jetons d’URL {#emails-and-url-tokens}

Créez les e-mails d’invitation, de confirmation, de suivi et de remerciement à l’aide de Marketo.

## E-mail de confirmation Marketo et jeton URL {#marketo-confirmation-email-and-url-token}

Utilisez Marketo pour envoyer l’e-mail de confirmation de votre événement. Lorsqu’une personne s’enregistre, elle reçoit une URL unique à utiliser pour saisir l’événement.

>[!NOTE]
>
>Pour remplir votre e-mail de confirmation avec cette URL unique, utilisez le jeton suivant dans votre e-mail : `{{member.webinar url}}`. Lorsque vous envoyez l’URL de confirmation, ce jeton est automatiquement résolu sur l’URL de confirmation unique de la personne.
>
>Définissez le type de votre e-mail de confirmation sur **Opérationnel** afin de vous assurer que les personnes qui s’enregistrent reçoivent leurs informations de confirmation, même si elles se sont désabonnées.

>[!TIP]
>
>Vous pouvez configurer ON24 pour envoyer des e-mails de confirmation, de rappel ou de relance. Pour plus d’informations, consultez le site d’aide [ON24](https://support.on24.com/hc/en-us/categories/26127314569115-Webcast-Elite){target="_blank"}.

## Exigences relatives aux campagnes enfants enregistrées {#registration-child-campaign-requirements}

Les événements contiennent une ou plusieurs campagnes enfants qui fonctionnent toutes ensemble pour faire passer les personnes par les statuts du programme et vous permettre de suivre les performances de votre événement.

Parmi les exemples de campagnes enfants, citons une campagne d’invitation, une campagne d’enregistrement et des campagnes de suivi.

>[!CAUTION]
>
>Pour que la carte fonctionne correctement, vous DEVEZ créer une campagne d&#39;enregistrement. Cette campagne doit être déclenchée par la personne remplissant un formulaire. La première étape doit modifier le statut du programme de la personne en **Enregistré**. La campagne envoie ensuite un e-mail de confirmation. Voir le reste de cet article pour plus de détails.

**Enregistrement/Confirmation (Déclencher Une Campagne)**

* Liste intelligente
* Déclencheur basé sur **remplit le formulaire**. Veillez à inclure la page de destination sur laquelle réside le formulaire à l’aide de l’option **Ajouter une contrainte**, en particulier si le même formulaire est utilisé sur plusieurs pages de destination.

>[!CAUTION]
>
>Vous devez utiliser un formulaire Marketo pour inscrire vos membres à l’événement ou un formulaire autre que Marketo avec l’intégration d’API appropriée pour transmettre les données d’enregistrement à Marketo. Ceci est essentiel au succès de l’intégration de votre partenaire d’événement.

>[!NOTE]
>
>Si vous utilisez un formulaire Marketo sur une page de destination autre que Marketo, votre déclencheur sera **[!UICONTROL Remplit le formulaire]** avec le [!UICONTROL Nom du formulaire].

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flux**

* **[!UICONTROL Modifier le statut du programme]** - Définir sur Webinaire -> Enregistré.

Cette étape de flux est requise comme PREMIÈRE ÉTAPE DE FLUX lors de la configuration de votre campagne enfant. Lorsque le statut du programme d’une personne passe à Enregistré, Marketo transmet les informations d’enregistrement à ON24. Aucun autre statut ne poussera la personne vers le serveur.

* **[!UICONTROL Envoyer un e-mail]** - E-mail de confirmation. Définissez cet e-mail sur **Opérationnel** afin que les personnes désabonnées qui se sont enregistrées le reçoivent toujours.

L’étape de flux **[!UICONTROL Envoyer un e-mail]** DOIT être la deuxième étape. L’e-mail de confirmation contient le `{{member.webinar url}}`, qui est renseigné avec les informations renvoyées à Marketo depuis ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>L’ordre de ces étapes de flux est important en raison de l’ordre dans lequel les actions sont exécutées dans Marketo. L’étape **[!UICONTROL Modifier le statut du programme]** envoie la personne à ON24 pour qu’elle s’enregistre et une URL unique est générée. Ensuite, vous pouvez envoyer l’e-mail de confirmation qui inclut cette URL unique à l’aide du jeton `{{member.webinar URL}}`.
>
>Si la personne est renvoyée avec une erreur d’enregistrement, elle ne recevra pas l’e-mail de confirmation.

L’étape suivante consiste à [tester votre intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Présentation des événements de l&#39;adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [Exemple d’intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Présentation des statuts du programme de webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
