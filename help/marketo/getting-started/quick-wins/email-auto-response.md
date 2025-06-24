---
unique-page-id: 2359416
description: Réponse automatique aux e-mails - Documents Marketo - Documentation du produit
title: Réponse e-mail automatique
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 10%

---

# Réponse e-mail automatique {#email-auto-response}

## Mission : envoyer un e-mail de remerciement lorsqu’une personne remplit un formulaire {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configuration et ajout d’une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [ Page de destination avec un formulaire ](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Étape 1 : Créer un e-mail {#step-create-an-email}

1. Accédez à la zone [!UICONTROL Activités marketing].

   ![](assets/email-auto-response-1.png)

1. Sélectionnez votre programme dans le menu de gauche, cliquez sur le menu déroulant **[!UICONTROL Nouveau]**, puis sélectionnez **[!UICONTROL Nouvelle ressource locale]**.

   ![](assets/email-auto-response-2.png)

1. Sélectionnez **[!UICONTROL E-mail]**.

   ![](assets/email-auto-response-3.png)

1. Nommez votre e-mail « Réponse automatique », choisissez un modèle, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/email-auto-response-4.png)

   Un éditeur d’e-mail s’ouvre dans une nouvelle fenêtre ou un nouvel onglet. Si les pop-ups sont bloqués, cliquez sur **[!UICONTROL Modifier le brouillon]** sur la page de résumé de la ressource pour accéder à l’e-mail.

1. Saisissez l’objet, puis double-cliquez sur la zone modifiable de l’e-mail.

   ![](assets/email-auto-response-5.png)

   _Un éditeur de texte enrichi s’ouvre au-dessus de l’éditeur d’e-mail._

1. Mettez en surbrillance le contenu de l’e-mail existant.

   ![](assets/email-auto-response-6.png)

1. Saisissez le contenu de l’e-mail, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/email-auto-response-7.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Actions liées à l’e-mail]** et sélectionnez **[!UICONTROL Approuver et fermer]**.

   ![](assets/email-auto-response-8.png)

## Étape 2 : Créer une campagne intelligente {#step-create-a-smart-campaign}

1. Sélectionnez votre programme, cliquez sur la liste déroulante **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouvelle campagne intelligente]**.

   ![](assets/email-auto-response-9.png)

1. **Nommez** la campagne intelligente « Campagne de réponse automatique », puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/email-auto-response-10.png)

1. Accédez à l’onglet **[!UICONTROL Liste dynamique]**.

   ![](assets/email-auto-response-11.png)

   Nous configurons cette campagne pour qu’elle s’exécute chaque fois qu’une personne remplit le formulaire que vous avez créé dans [**Page de destination avec un formulaire**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

1. Recherchez le déclencheur **[!UICONTROL Remplit le formulaire]** et faites-le glisser vers la zone de travail.

   ![](assets/email-auto-response-12.png)

1. Sélectionnez **[!UICONTROL Mon formulaire]** dans la liste déroulante. Cliquez ensuite sur l’onglet **[!UICONTROL Flux]**.

   ![](assets/email-auto-response-13.png)

1. Faites glisser l’action de flux **[!UICONTROL Envoyer un e-mail]** vers la zone de travail de gauche.

   ![](assets/email-auto-response-14.png)

1. Sélectionnez l’option **Réponse automatique aux e-mails**. Cliquez ensuite sur l’onglet **[!UICONTROL Planifier]**.

   ![](assets/email-auto-response-15.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/email-auto-response-16.png)

1. Sélectionnez **[!UICONTROL à chaque fois]** et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/email-auto-response-17.png)

1. Cliquez sur **[!UICONTROL Activer]**.

   ![](assets/email-auto-response-18.png)

1. Cliquez sur **[!UICONTROL Activer]** dans l’écran de confirmation.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Une fois active, cette campagne s’exécute chaque fois qu’une personne remplit le formulaire spécifié. La campagne continue de s’exécuter jusqu’à ce qu’elle soit désactivée.

## Étape 3 : Remplir le formulaire {#step-fill-out-the-form}

1. Sélectionnez **Ma page** (cela a été créé dans le [Page de destination avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} gain rapide) et cliquez sur **[!UICONTROL Aperçu]**.

   ![](assets/email-auto-response-20.png)

   _Votre page de destination « Essai gratuit » s’ouvre dans un nouvel onglet._

1. Remplissez le formulaire avec votre prénom, votre nom et votre adresse e-mail, puis cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Indiquez une adresse e-mail valide pour être sûr de bien recevoir l&#39;e-mail.

## Mission accomplie {#mission-complete}

En quelques minutes, l’e-mail de réponse automatique devrait s’afficher dans votre boîte de réception.

[◄ Mission 3 : Score Simple](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Mission 5 : Importer une liste de personnes ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
