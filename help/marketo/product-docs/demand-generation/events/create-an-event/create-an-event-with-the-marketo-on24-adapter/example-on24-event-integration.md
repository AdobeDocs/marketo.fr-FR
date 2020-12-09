---
unique-page-id: 10096679
description: Exemple ON24 Événement Integration - Marketo Docs - Documentation du produit
title: Exemple d’intégration de Événement ON24
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Exemple d’intégration de Événement ON24 {#example-on-event-integration}

Voici un exemple de événement, y compris des campagnes, pour un webinaire ON24. Lorsque vous créez votre événement, veillez à tester vos campagnes avant de les exécuter.

## Création d’un Événement dans les Activités marketing {#create-a-new-event-in-marketing-activities}

1. Sélectionnez **Nouveau** > **Nouveau Programme**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Sélectionnez un dossier **** Campaign dans lequel le événement sera installé.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Saisissez un **nom** pour le événement.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Sélectionnez **Événement **comme type **de** Programme.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Sélectionnez **Webinaire **comme **Canal **pour le événement.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Cliquez sur **Créer**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Invitation (Campaign par lot)  {#invite-batch-campaign}

* **Liste** intelligente - Définissez qui vous inviterez au événement.
* **Flux**

   * Envoyer un courrier électronique - S&#39;il s&#39;agit d&#39;un courrier électronique de ressources local, il aura la convention d&#39;affectation de nom suivante : EventName.EmailName. Vous pouvez également utiliser des courriers électroniques globaux.
   * Modifier l’état dans Progression - Définissez sur Webinaire > Invité.

* **Programmation** - Définissez la date d&#39;envoi de l&#39;invitation.

## Inscription/Confirmation (Trigger Campaign) {#registration-confirmation-trigger-campaign}

* **Liste intelligente**

   * Déclenchez la campagne en fonction du formulaire **** Remplit. Veillez à inclure le landing page sur lequel se trouve le formulaire en utilisant la contrainte **d’** Ajoute, en particulier si le formulaire est utilisé sur plusieurs landings page.

>[!CAUTION]
>
>Vous devez utiliser un formulaire Marketo pour enregistrer des personnes pour le événement, ou un formulaire non Marketo avec l’intégration d’API appropriée pour envoyer les données d’enregistrement à Marketo. Ceci est essentiel à la réussite de l&#39;intégration de votre partenaire de Événement. **REMARQUE**: Si vous utilisez un formulaire Marketo sur un landing page non Marketo, votre déclencheur sera **Remplit le formulaire** avec le nom du formulaire.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Flux**

   * **Modifier l’état dans Progression** - Définir sur Webinaire > Inscrit. **ATTENTION**: Cette étape de flux est requise lors de la configuration de votre campagne enfant. Lorsque l’état de progression d’une personne passe à **Registered**, Marketo envoie les informations d’inscription à ON24.

   * **Envoyer un courriel** - Confirmation par courriel (paramétré sur **Opérationnel** pour que les personnes qui se sont inscrites désabonnées le reçoivent toujours).

![](assets/image2015-12-22-15-3a52-3a9.png)

**REMARQUE**: Si la personne est renvoyée avec une erreur d’enregistrement, elle ne recevra pas la confirmation par courrier électronique.

## Rappel (Campaign par lot) {#reminder-batch-campaign}

* **Liste** intelligente - Filtrez en utilisant **Membre du Programme** et définissez le statut sur **Inscrit**.

* **Flux** - Envoyer un courriel (rappel).

**REMARQUE**: Vous pouvez utiliser une campagne similaire pour envoyer un courriel de suivi *différent* aux personnes qui ont été invitées mais qui ne se sont pas encore inscrites.

## Campaign de suivi (par lot ou Trigger Campaign) {#follow-up-campaign-batch-or-trigger-campaign}

* **Liste** intelligente - Déclenche en fonction des modifications de l’état du programme.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Flux** - Envoyer un courriel. Utilisez les choix pour envoyer différents courriers électroniques en fonction de l’état du programme.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>* [Présentation des Événements d&#39;adaptateurs Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



