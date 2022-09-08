---
unique-page-id: 10096656
description: Création d’un événement avec l’adaptateur Marketo ON24 - Documents Marketo - Documentation du produit
title: Création d’un événement avec l’adaptateur Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Création d’un événement avec l’adaptateur Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

>[!IMPORTANT]
>
>Depuis août 2022, ON24 ne prend plus en charge les nouvelles intégrations Marketo. Les informations de cet article s’appliquent uniquement aux utilisateurs existants.

Vous devez connaître les blocs de création et la séquence recommandée pour la création d’événements dans Marketo. Vous devez également posséder une connaissance pratique des concepts Marketo suivants :

* [Programmes Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) ainsi que les événements, et les différences entre eux.
* [Canaux](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [Ressources locales](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [Campagnes enfants](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) et [Statuts du programme](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Reportez-vous à la section [Documentation de l’API Marketo](https://developers.marketo.com/documentation/rest/) pour plus d’informations sur les API Marketo.

## Conditions préalables {#prerequisites}

Les éléments suivants sont requis pour utiliser l’intégration Marketo ON24 :

* **Abonnement aux webcasts ON24** - Si vous ne disposez pas d&#39;un abonnement actuel, contactez directement ON24. **REMARQUE**: L’édition hébergée ON24 est requise. La gestion des événements ON24 n’est pas requise.

* **Droits d’administrateur sur ON24** - Vous en aurez besoin pour utiliser ce connecteur et créer des invités dans le système ON24.
* **Identifiants de connexion ON24** - Vous devrez saisir ces informations dans Marketo pour activer l’intégration : Nom d’utilisateur, mot de passe, ID client et clé client. Contactez votre gestionnaire de compte ON24 ou l’assistance ON24 si vous avez besoin d’aide sur vos informations d’identification.
* **Formulaire d’enregistrement** - Utilisez un formulaire Marketo ou un formulaire non Marketo avec l’API appropriée pour vous assurer que les données d’enregistrement et les informations d’enregistrement sont transmises à Marketo.
* **Campagne d’enregistrement** - Une campagne enfant d’enregistrement dans votre événement Marketo doit être créée et configurée correctement pour que votre intégration de partenaire d’événement fonctionne.

## Flux de processus {#process-flow}

Pour créer un événement avec l’adaptateur Marketo On24, procédez comme suit :

1. [Création de votre événement de webinaire dans ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [Configuration des paramètres d’événement et synchronisation du Marketo avec votre webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [Créer des campagnes enfants et des ressources locales](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [Test de votre intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [Exemple d’intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [Présentation des états du programme du webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [Mises à jour de l’enregistrement d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
