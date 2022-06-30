---
unique-page-id: 2359416
description: Réponse automatique aux courriers électroniques - Documents Marketo - Documentation du produit
title: Réponse e-mail automatique
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 16%

---

# Réponse e-mail automatique {#email-auto-response}

## Mission : Envoyer un email de remerciement lorsqu’une personne remplit un formulaire {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configuration et ajout d’une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Étape 1 : Créer un e-mail {#step-create-an-email}

1. Accédez à la zone Activités marketing .

   ![](assets/one-2.png)

1. Sélectionnez Mon programme dans le menu de gauche, cliquez sur la liste déroulante Nouveau , puis sélectionnez Nouvelle ressource locale.

   ![](assets/two-3.png)

1. Cliquer sur e-mail.

   ![](assets/three-2.png)

1. Nommez votre email &quot;Email de réponse automatique&quot;, choisissez un modèle, puis cliquez sur Créer.

   ![](assets/four-1.png)

   Un éditeur de courrier électronique s’ouvre dans une nouvelle fenêtre ou un nouvel onglet. Si les fenêtres contextuelles sont bloquées, cliquez sur **Modifier le brouillon** sur la page de résumé de la ressource pour accéder au courrier électronique.

1. Entrez un objet, puis double-cliquez sur la zone modifiable de l’email.

   ![](assets/five-2.png)

   _Un éditeur de texte enrichi s’ouvre en haut de l’éditeur d’email._

1. Mettre en surbrillance le contenu de l&#39;email existant.

   ![](assets/six-2.png)

1. Saisissez le contenu de votre email et cliquez sur Enregistrer.

   ![](assets/seven-2.png)

1. Vos modifications sont automatiquement enregistrées. Fermez l&#39;onglet/la fenêtre de l&#39;éditeur d&#39;email.

   ![](assets/eight-1.png)

1. Sélectionnez votre nouvel email. Sous Actions par courrier électronique, cliquez sur Approuver.

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Étape 2 : Créer une campagne intelligente {#step-create-a-smart-campaign}

1. Clic droit **Mon programme** et cliquez sur **Nouvelle campagne dynamique**.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Nom** votre campagne dynamique &quot;Campagne de réponse automatique&quot;, puis cliquez sur **Créer**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Cliquez sur l&#39;onglet **Liste intelligente**.

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Nous configurons cette campagne pour qu’elle s’exécute chaque fois qu’une personne remplit le formulaire que vous avez créé dans [**Page d’entrée avec un formulaire**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}.

1. Recherchez et faites glisser le **Remplir le formulaire** se déclenche dans la zone de travail de gauche.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Sélectionner **Mon formulaire** dans la liste déroulante. Cliquez sur l&#39;onglet **Flux**.

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Faites glisser le **Envoyer un courrier électronique** action de flux vers le canevas de gauche.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Sélectionnez votre **Email de réponse automatique** et accédez au **Planification** .

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Cliquez sur **Modifier**.

   ![](assets/8.png)

1. Sélectionnez **à chaque fois** et cliquez sur **Enregistrer**.

   ![](assets/9.png)

1. Cliquez sur **Activer**.

   ![](assets/10.png)

1. Cliquez sur **Activer** sur l’écran de confirmation.

   ![](assets/11.png)

>[!NOTE]
>
>Une fois principale, cette campagne s’exécute chaque fois qu’une personne remplit le formulaire spécifié. La campagne continue à s’exécuter jusqu’à ce qu’elle soit désactivée.

## Étape 3 : Remplir le formulaire {#step-fill-out-the-form}

1. Sélectionner **Ma page**. Il a été créé dans la variable [Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} gain rapide.

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Cliquez sur **Afficher la page approuvée**.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   Votre page d’entrée &quot;Essai gratuit&quot; s’ouvre dans un nouvel onglet.

1. Remplissez le formulaire avec votre prénom, votre nom et votre adresse électronique, puis cliquez sur **Envoyer**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Indiquez une adresse e-mail valide pour être sûr de bien recevoir l&#39;e-mail.

## Mission accomplie {#mission-complete}

Dans quelques minutes, vous devriez voir l’e-mail de réponse automatique dans votre boîte de réception. Bon boulot !

<br> 

[◄ Mission 3 : Évaluation simple](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Mission 5 : Importation d’une liste de personnes ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
