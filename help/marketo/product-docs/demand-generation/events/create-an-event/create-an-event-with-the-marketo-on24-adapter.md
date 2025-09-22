---
unique-page-id: 10096656
description: Création d’un événement avec l’adaptateur Marketo ON24 - Documentation de Marketo - Documentation du produit
title: Créer un événement avec l’adaptateur Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 6%

---

# Créer un événement avec l’adaptateur Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

Vous devez connaître les blocs de création et la séquence recommandée pour la création d’événements dans Marketo. Vous devez également avoir une connaissance pratique des concepts Marketo suivants :

* [Programmes Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"} ainsi que les événements, et les différences entre eux
* [Canaux](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Assets local](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Campagnes enfants](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} et [Statuts des programmes](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Reportez-vous à la documentation de l’API Marketo [&#128279;](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} pour plus d’informations sur les API Marketo.

## Conditions préalables {#prerequisites}

Les éléments suivants sont requis pour utiliser l’intégration ON24 de Marketo :

* **Abonnement aux webdiffusions ON24** - Si vous n&#39;avez pas d&#39;abonnement en cours, contactez ON24 directement. **REMARQUE** : l’édition hébergée ON24 est requise. La gestion des événements ON24 n&#39;est pas obligatoire.

* **Droits d&#39;administrateur sur ON24** - Vous en aurez besoin pour utiliser ce connecteur et créer des invités dans le système ON24.
* **Informations d’identification de connexion ON24** - Vous devez saisir ces informations dans Marketo pour activer l’intégration : nom d’utilisateur, mot de passe, identifiant client et clé client. Contactez votre gestionnaire de compte ON24 ou l&#39;assistance ON24 si vous avez besoin d&#39;aide pour vos informations d&#39;identification.
* **Formulaire d’enregistrement** - Utilisez un formulaire Marketo ou un formulaire autre que Marketo avec l’API appropriée pour vous assurer que les données d’enregistrement et les informations d’enregistrement sont transmises à Marketo.
* **Campagne enfant d’enregistrement** - Une campagne enfant d’enregistrement dans votre événement Marketo doit être créée et configurée correctement pour que votre intégration de partenaire d’événement fonctionne.

## Flux de processus {#process-flow}

Pour créer un événement avec l&#39;adaptateur Marketo On24, procédez comme suit :

1. [Créez votre événement de webinaire dans ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Configuration des paramètres d’événement et synchronisation de Marketo avec votre webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Créer des campagnes enfants et des Assets locales](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Tester votre intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Exemple d’intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Présentation des statuts du programme de webinaire](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [Mises à jour de l’inscription aux événements ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
