---
unique-page-id: 10096679
description: Exemple d’intégration d’événement ON24 - Documents Marketo - Documentation du produit
title: Exemple d’intégration d’événement ON24
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Exemple d’intégration d’événement ON24 {#example-on-event-integration}

Voici un exemple d’événement, y compris des campagnes, pour un webinaire ON24. Lorsque vous créez votre événement, veillez à tester vos campagnes avant de les exécuter.

## Création d’un événement dans les activités marketing {#create-a-new-event-in-marketing-activities}

1. Sélectionnez **Nouveau** > **Nouveau programme**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Sélectionnez un **dossier de campagne** où l’événement se tiendra.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Saisissez un **Nom** pour l’événement.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Sélectionnez **Event** comme **Program Type**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Sélectionnez **Webinaire** comme **Canal** pour l’événement.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Cliquez sur **Créer**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Invitation (campagne par lots)  {#invite-batch-campaign}

* **Liste dynamique** - Définissez qui vous inviterez à l’événement.
* **Flux**

   * Envoyer un courrier électronique : s’il s’agit d’un courrier électronique de ressource local, il aura la convention d’affectation des noms suivante : EventName.EmailName. Vous pouvez également utiliser des emails globaux.
   * Changez l’état dans Progression - Défini sur Webinaire > Invité.

* **Planning** - Définissez la date d’envoi de l’invitation.

## Enregistrement/Confirmation (campagne de déclenchement) {#registration-confirmation-trigger-campaign}

* **Liste dynamique**

   * Déclenchez la campagne en fonction du **formulaire de remplissage**. Veillez à inclure la page d’entrée sur laquelle le formulaire réside en utilisant **Ajouter la contrainte**, en particulier si le formulaire est utilisé sur plusieurs pages d’entrée.

>[!CAUTION]
>
>Vous devez utiliser un formulaire Marketo pour enregistrer des personnes pour l’événement, ou un formulaire non Marketo avec l’intégration d’API appropriée pour transmettre les données d’enregistrement à Marketo. C’est essentiel au succès de l’intégration de votre partenaire d’événement. **REMARQUE** : si vous utilisez un formulaire Marketo sur une page d’entrée autre que Marketo, votre déclencheur sera **Remplit le formulaire** avec le nom du formulaire.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flux**

   * **Changement d’état dans la progression** - Défini sur Webinaire > Enregistré. **ATTENTION** : cette étape de flux est requise lors de la configuration de votre campagne enfant. Lorsque l’état de progression d’une personne passe à **Registered**, Marketo envoie les informations d’enregistrement à ON24.

   * **Envoyer un courrier électronique** - Confirmation par courrier électronique (définie sur **Operational** de sorte que les personnes désabonnées qui se sont enregistrées continuent de le recevoir).

![](assets/image2015-12-22-15-3a52-3a9.png)

**REMARQUE** : si la personne est renvoyée avec une erreur d’enregistrement, elle ne reçoit pas la confirmation par courrier électronique.

## Rappel (campagne par lots) {#reminder-batch-campaign}

* **Liste dynamique** - Filtrez à l’aide de **Member of Program** et définissez l’état sur **Registered**.

* **Flux** - Envoyer un courrier électronique (rappel).

**REMARQUE** : vous pouvez utiliser une campagne similaire pour envoyer un email de relance *différent* aux personnes qui ont été invitées mais qui ne se sont pas encore enregistrées.

## Campagne de relance (campagne par lot ou de déclenchement) {#follow-up-campaign-batch-or-trigger-campaign}

* **Liste dynamique** - Déclenchez en fonction des modifications de l’état du programme.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flux** - Envoyer un courrier électronique. Utilisez les choix pour envoyer différents emails en fonction de l’état du programme.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Compréhension des événements d’adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
