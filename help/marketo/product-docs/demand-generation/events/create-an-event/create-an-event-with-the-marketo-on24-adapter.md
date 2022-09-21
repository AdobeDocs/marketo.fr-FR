---
unique-page-id: 10096656
description: Création d’un événement avec l’adaptateur Marketo ON24 - Documents Marketo - Documentation du produit
title: Création d’un événement avec l’adaptateur Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Création d’un événement avec l’adaptateur Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

Vous devez connaître les blocs de création et la séquence recommandée pour la création d’événements dans Marketo. Vous devez également posséder une connaissance pratique des concepts Marketo suivants :

* [Programmes Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;} ainsi que les événements, et les différences entre eux
* [Canaux](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target=&quot;_blank&quot;}
* [Ressources locales](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target=&quot;_blank&quot;}
* [Campagnes enfants](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;} et [Statuts du programme](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target=&quot;_blank&quot;}

>[!NOTE]
>
>Reportez-vous à la section [Documentation de l’API Marketo](https://developers.marketo.com/documentation/rest/){target=&quot;_blank&quot;} pour plus d’informations sur les API Marketo.

## Conditions préalables {#prerequisites}

Les éléments suivants sont requis pour utiliser l’intégration Marketo ON24 :

* **Abonnement aux webcasts ON24** - Si vous ne disposez pas d&#39;un abonnement actuel, contactez directement ON24. **REMARQUE**: L’édition hébergée ON24 est requise. La gestion des événements ON24 n’est pas requise.

* **Droits d’administrateur sur ON24** - Vous en aurez besoin pour utiliser ce connecteur et créer des invités dans le système ON24.
* **Identifiants de connexion ON24** - Vous devrez saisir ces informations dans Marketo pour activer l’intégration : Nom d’utilisateur, mot de passe, ID client et clé client. Contactez votre gestionnaire de compte ON24 ou l’assistance ON24 si vous avez besoin d’aide sur vos informations d’identification.
* **Formulaire d’enregistrement** - Utilisez un formulaire Marketo ou un formulaire non Marketo avec l’API appropriée pour vous assurer que les données d’enregistrement et les informations d’enregistrement sont transmises à Marketo.
* **Campagne d’enregistrement** - Une campagne enfant d’enregistrement dans votre événement Marketo doit être créée et configurée correctement pour que votre intégration de partenaire d’événement fonctionne.

## Flux de processus {#process-flow}

Pour créer un événement avec l’adaptateur Marketo On24, procédez comme suit :

1. [Création de votre événement de webinaire dans ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target=&quot;_blank&quot;}
1. [Configuration des paramètres d’événement et synchronisation du Marketo avec votre webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;}
1. [Créer des campagnes enfants et des ressources locales](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target=&quot;_blank&quot;}
1. [Test de votre intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target=&quot;_blank&quot;}
1. [Exemple d’intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
1. [Présentation des états du programme du webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target=&quot;_blank&quot;}
1. [Mises à jour de l’enregistrement d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target=&quot;_blank&quot;}
