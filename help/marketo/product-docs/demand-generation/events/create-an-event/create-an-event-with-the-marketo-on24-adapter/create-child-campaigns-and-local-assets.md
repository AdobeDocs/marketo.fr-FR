---
unique-page-id: 10096675
description: Créer des campagnes enfants et des ressources locales - Documents marketing - Documentation du produit
title: Créer des campagnes enfants et des ressources locales
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# Créer des campagnes enfants et des ressources locales {#create-child-campaigns-and-local-assets}

Créez vos campagnes enfants et vos ressources locales à l’aide de Design Studio.

## landing page et formulaire {#landing-page-and-form}

Pour vous assurer que les utilisateurs sont correctement enregistrés auprès de ON24, les champs suivants doivent être inclus dans votre formulaire Marketo :

* Prénom
* Nom
* Adresse électronique

Vous pouvez également placer les champs suivants sur ON24 :

* Nom de la société
* Titre de la tâche

Avec l&#39;étape de flux appropriée ajoutée à la campagne d&#39;enregistrement, les gens seront poussés à ON24 et seront marqués comme enregistrés. Vous pouvez ajouter d’autres champs au formulaire et les informations seront capturées dans Marketo dans le cadre de l’enregistrement des détails de la personne.

>[!CAUTION]
>
>Pour réussir l’intégration, vous devez utiliser un formulaire Marketo pour enregistrer vos utilisateurs pour le Événement, ou un formulaire non Marketo avec l’intégration d’API appropriée pour envoyer les données d’enregistrement à Marketo.

## Courriers électroniques et jetons d’URL {#emails-and-url-tokens}

Créez l’invitation, la confirmation, le suivi et les e-mails de remerciement à l’aide de Marketing Cloud.

## Courrier électronique de confirmation de marketing et jeton d’URL {#marketo-confirmation-email-and-url-token}

Utilisez Marketing pour envoyer le courriel de confirmation de votre événement. Lorsqu’une personne s’enregistre, elle reçoit une URL unique à utiliser pour entrer dans le événement.

>[!NOTE]
>
>**Rappel**
>
>Pour renseigner votre message de confirmation avec cette URL unique, utilisez le jeton suivant dans votre message électronique : `{{member.webinar url}}`. Lorsque vous envoyez l’URL de confirmation, ce jeton correspond automatiquement à l’URL de confirmation unique de la personne.
>
>Définissez le type de votre message de confirmation sur **Operational** pour vous assurer que les personnes qui s&#39;inscrivent reçoivent leurs informations de confirmation, même si elles ne s&#39;abonnent pas.

>[!TIP]
>
>Vous pouvez configurer ON24 pour envoyer des messages de confirmation, de rappel ou de suivi. Pour plus d&#39;informations, consultez le site [d&#39;aide](http://webcastelitehelp.on24.com) ON24.

## Conditions requises pour l&#39;enregistrement des enfants Campaign {#registration-child-campaign-requirements}

Les événements contiennent une ou plusieurs campagnes enfants qui fonctionnent toutes ensemble pour déplacer les personnes à travers les états de programme et vous permettent de suivre les performances de votre événement.

Les campagnes enfants sont, par exemple, une campagne d’invitation, une campagne d’enregistrement et des campagnes de suivi.

>[!CAUTION]
>
>Pour que l&#39;adaptateur puisse faire son travail, vous DEVEZ créer une campagne d&#39;enregistrement. Cette campagne doit être déclenchée par la personne qui remplit un formulaire et la première étape doit changer le statut de programme de la personne en **état d’enregistrement**. La campagne envoie ensuite un message de confirmation. Consultez le reste de cet article pour plus de détails.

**Inscription/Confirmation (Trigger Campaign)**

* Liste intelligente
* Déclencheur basé sur le **remplissage du formulaire**. Veillez à inclure le landing page sur lequel se trouve le formulaire en utilisant la contrainte **d’** Ajoute, en particulier si le même formulaire est utilisé sur plusieurs landings page.

>[!CAUTION]
>
>Vous devez utiliser un formulaire Marketo pour enregistrer vos utilisateurs pour le événement, ou un formulaire non Marketo avec l’intégration d’API appropriée pour envoyer les données d’enregistrement à Marketo. Ceci est essentiel à la réussite de l’intégration de votre partenaire de événement.

>[!NOTE]
>
>Si vous utilisez un formulaire Marketo sur un landing page non Marketo, votre déclencheur sera **Remplit le formulaire** avec le nom du formulaire.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flux**

* **Modifier l&#39;état** du Programme - Définir sur Webinaire -> Inscrit.

Cette étape de flux est requise en tant que PREMIÈRE ÉTAPE de flux lors de la configuration de votre campagne enfant. Lorsqu’un état de programme d’une personne devient Enregistré, Marketo envoie les informations d’enregistrement à ON24. Aucun autre statut ne poussera la personne vers le bas.

* **Envoyer un courriel** - Confirmation par courriel. Définissez ce courrier électronique sur **Operational** pour que les personnes qui se sont abonnées et qui se sont inscrites le reçoivent toujours.

L’étape de flux **Envoyer un courriel** DOIT être la deuxième étape. L’e-mail de confirmation contient le `{{member.webinar url}}`, qui est renseigné par les informations renvoyées à Marketo à partir de ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>L’ordre de ces étapes de flux est important en raison de l’ordre dans lequel les actions sont exécutées dans Marketing. L’étape **Modifier l’état** du Programme envoie la personne à ON24 pour qu’elle s’enregistre et une URL unique est générée. Après cela, vous pouvez envoyer le courrier électronique de confirmation contenant cette URL unique à l’aide du `{{member.webinar URL}}` jeton.
>
>Si la personne est renvoyée avec une erreur d’enregistrement, elle ne recevra pas la confirmation par courrier électronique.

L’étape suivante consiste à [tester l’intégration](test-your-on24-event-integration.md)de votre événement ON24.

>[!MORELIKETHIS]
>
>* [Présentation des Événements d&#39;adaptateurs Marketo ON24](understanding-marketo-on24-adapter-events.md)
>* [Exemple d’intégration de Événement ON24](example-on24-event-integration.md)
>* [Comprendre l&#39;état des Programmes du webinaire](understanding-webinar-program-statuses.md)
>* [Testez votre intégration de Événement ON24](test-your-on24-event-integration.md)

>



