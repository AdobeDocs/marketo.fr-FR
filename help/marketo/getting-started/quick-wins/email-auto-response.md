---
unique-page-id: 2359416
description: Réponse automatique aux courriers électroniques - Documents Marketo - Documentation du produit
title: Réponse e-mail automatique
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 10%

---

# Réponse e-mail automatique {#email-auto-response}

## Mission : envoyer un email de remerciement lorsqu’une personne remplit un formulaire {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configurer et ajouter une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Étape 1 : Créer un e-mail {#step-create-an-email}

1. Accédez à la zone **[!UICONTROL Activités marketing]**.

   ![](assets/email-auto-response-1.png)

1. Sélectionnez votre programme dans le menu de gauche, cliquez sur la liste déroulante **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouvelle ressource locale]**.

   ![](assets/email-auto-response-2.png)

1. Sélectionnez **[!UICONTROL Email]**.

   ![](assets/email-auto-response-3.png)

1. Nommez votre email &quot;Email de réponse automatique&quot;, choisissez un modèle, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/email-auto-response-4.png)

   Un éditeur de courrier électronique s’ouvre dans une nouvelle fenêtre ou un nouvel onglet. Si les fenêtres contextuelles sont bloquées, cliquez sur **[!UICONTROL Modifier la version préliminaire]** sur la page de résumé de la ressource pour accéder au courrier électronique.

1. Entrez un objet, puis double-cliquez sur la zone modifiable de l’email.

   ![](assets/email-auto-response-5.png)

   _Un éditeur de texte enrichi s’ouvre en haut de l’éditeur de courrier électronique._

1. Mettre en surbrillance le contenu de l&#39;email existant.

   ![](assets/email-auto-response-6.png)

1. Saisissez votre contenu d&#39;email et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/email-auto-response-7.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Actions de courrier électronique]** et sélectionnez **[!UICONTROL Approuver et fermer]**.

   ![](assets/email-auto-response-8.png)

## Étape 2 : Créer une campagne intelligente {#step-create-a-smart-campaign}

1. Sélectionnez votre programme, cliquez sur la liste déroulante **[!UICONTROL New]** et sélectionnez **[!UICONTROL New Smart Campaign]**.

   ![](assets/email-auto-response-9.png)

1. **Nommez** votre campagne dynamique &quot;Campagne de réponse automatique&quot; et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/email-auto-response-10.png)

1. Accédez à l’onglet **[!UICONTROL Liste dynamique]** .

   ![](assets/email-auto-response-11.png)

   Nous configurons cette campagne pour qu’elle s’exécute chaque fois qu’une personne remplit le formulaire que vous avez créé dans [**Landing Page with a Form**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

1. Recherchez et faites glisser le déclencheur **[!UICONTROL Remplit le formulaire]** sur la zone de travail.

   ![](assets/email-auto-response-12.png)

1. Sélectionnez **[!UICONTROL Mon formulaire]** dans la liste déroulante. Cliquez ensuite sur l’onglet **[!UICONTROL Flux]** .

   ![](assets/email-auto-response-13.png)

1. Faites glisser l’action de flux **[!UICONTROL Envoyer un courrier électronique]** vers le canevas de gauche.

   ![](assets/email-auto-response-14.png)

1. Sélectionnez votre **courriel de réponse automatique**. Cliquez ensuite sur l’onglet **[!UICONTROL Planning]** .

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
>Une fois active, cette campagne s’exécute chaque fois qu’une personne remplit le formulaire spécifié. La campagne continue à s’exécuter jusqu’à ce qu’elle soit désactivée.

## Étape 3 : Remplir le formulaire {#step-fill-out-the-form}

1. Sélectionnez **Ma page** (cela a été créé dans la [Landing Page with a Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} quick win) et cliquez sur **[!UICONTROL Preview]** (Aperçu).

   ![](assets/email-auto-response-20.png)

   _Votre page d’entrée &quot;Essai gratuit&quot; s’ouvre dans un nouvel onglet._

1. Remplissez le formulaire avec votre prénom, votre nom et votre adresse électronique, puis cliquez sur **[!UICONTROL Submit]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Indiquez une adresse e-mail valide pour être sûr de bien recevoir l&#39;e-mail.

## Mission accomplie {#mission-complete}

Dans quelques minutes, vous devriez voir l’e-mail de réponse automatique dans votre boîte de réception. Bon boulot !

<br> 

[◄ Mission 3 : notation simple](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Mission 5 : Importer une liste de personnes ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
