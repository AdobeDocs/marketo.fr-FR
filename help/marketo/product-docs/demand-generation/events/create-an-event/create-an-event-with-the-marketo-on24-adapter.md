---
unique-page-id: 10096656
description: Créer un Événement avec l'adaptateur Marketo ON24 - Docs marketing - Documentation du produit
title: Créer un Événement avec l'adaptateur Marketo ON24
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Créer un Événement avec l&#39;adaptateur Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

## Avant de commencer {#before-you-begin}

Vous devez connaître les blocs de création et la séquence recommandée pour la création de Événements dans Marketo. Vous devez également posséder une connaissance pratique des concepts de Marketo suivants :

* [](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) Programmes marketing et Événements, et les différences entre eux
* [Canaux](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [Ressources locales](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [Etat des ](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) campagnes et des  [Programmes enfants](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Pour plus d’informations sur les API de marketing, consultez la [documentation de l’API de marketing](https://developers.marketo.com/documentation/rest/).

## Conditions préalables {#prerequisites}

Les éléments suivants sont requis pour utiliser l’intégration de Marketo ON24 :

* **Abonnement aux webcasts**  ON24 - Si vous n&#39;avez pas d&#39;abonnement actuel, communiquez directement avec ON24. **REMARQUE** : On24 Hosted Edition est requis. On24 Événement Management n&#39;est pas requis.

* **Droits d&#39;administrateur sur ON24**  - Vous en aurez besoin pour utiliser ce connecteur et créer des invités dans le système ON24.
* **Informations d’identification**  de connexion ON24 - Vous devez entrer ces informations dans Marketo pour activer l’intégration : Nom d’utilisateur, Mot de passe, ID de client et clé de client. Contactez votre gestionnaire de compte ON24 ou le service d’assistance ON24 si vous avez besoin d’aide pour vos informations d’identification.
* **Formulaire**  d&#39;inscription - Utilisez un formulaire Marketo ou un formulaire non Marketo avec l&#39;API appropriée pour vous assurer que les données d&#39;inscription et les informations d&#39;inscription sont transmises à Marketo.
* **Campagne**  enfant d&#39;inscription : une campagne enfant d&#39;inscription dans votre Événement Marketo doit être créée et configurée correctement pour que l&#39;intégration de votre partenaire de Événement fonctionne.

## Flux de processus {#process-flow}

Pour créer un Événement avec l&#39;adaptateur Marketo On24, procédez comme suit :

1. [Entrez vos informations d&#39;identification ON24 dans Marketo](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [Création de votre Événement de webinaire dans ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [Configuration des paramètres du Événement et synchronisation du marketing avec votre webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [Créer des campagnes enfants et des ressources locales](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [Testez votre intégration de Événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [Exemple d’intégration de Événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [Comprendre l&#39;état des Programmes du webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [Mises à jour de l&#39;abonnement Événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
