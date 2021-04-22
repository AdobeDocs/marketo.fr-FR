---
unique-page-id: 2359416
description: Réponse automatique par courrier électronique - Documents Marketo - Documentation du produit
title: Réponse e-mail automatique
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 19%

---

# Réponse e-mail automatique {#email-auto-response}

## Mission : Envoyer un e-mail de remerciement lorsqu&#39;une personne remplit un formulaire {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Configurer et Ajouter une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Page de destination avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)


## Étape 1 : Créer un e-mail {#step-create-an-email}

1. Accédez à la zone Activités marketing.

   ![](assets/one-2.png)

1. Sélectionnez Mon Programme dans le menu de gauche, cliquez sur la liste déroulante Nouveau, puis sélectionnez Nouveau fichier local.

   ![](assets/two-3.png)

1. Cliquer sur e-mail.

   ![](assets/three-2.png)

1. Nommez votre adresse électronique &quot;Courriel de réponse automatique&quot;, choisissez un modèle et cliquez sur Créer.

   ![](assets/four-1.png)

   Un éditeur de courrier électronique s’ouvre dans une nouvelle fenêtre ou un nouvel onglet. Si les fenêtres contextuelles sont bloquées, cliquez sur **Modifier le brouillon** dans la page de résumé des ressources pour accéder au courrier électronique.

1. Entrez un objet, puis cliquez sur la zone modifiable du courrier électronique en maintenant le doublon enfoncé.

   ![](assets/five-2.png)

   _Un éditeur de texte enrichi s’ouvre au-dessus de l’éditeur de courrier électronique._

1. Mettez en surbrillance le contenu du courrier électronique existant.

   ![](assets/six-2.png)

1. Saisissez votre contenu de courrier électronique et cliquez sur Enregistrer.

   ![](assets/seven-2.png)

1. Vos modifications sont enregistrées automatiquement. Fermez l’onglet/la fenêtre de l’éditeur de courrier électronique.

   ![](assets/eight-1.png)

1. Sélectionnez votre nouveau courriel. Sous Actions par courrier électronique, cliquez sur Approuver.

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Étape 2 : Créer une campagne intelligente {#step-create-a-smart-campaign}

1. Cliquez avec le bouton droit de la souris sur **Mon Programme** et cliquez sur **Nouvelle Campaign dynamique**.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Attribuez un** nom à la campagne dynamique &quot;Auto Response Campaign&quot; et cliquez sur  **Créer**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Cliquez sur l&#39;onglet **Liste intelligente**.

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Nous configurons cette campagne pour qu’elle s’exécute chaque fois qu’une personne remplit le formulaire que vous avez créé dans [**Landing page avec un formulaire**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md).

1. Recherchez et faites glisser le déclencheur **Remplit le formulaire** sur le canevas de gauche.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Sélectionnez **Mon formulaire** dans la liste déroulante. Cliquez sur l&#39;onglet **Flux**.

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Faites glisser l’action de flux **Envoyer un courrier électronique** vers le canevas de gauche.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Sélectionnez votre **courriel de réponse automatique** et accédez à l&#39;onglet **Planification**.

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Cliquez sur **Modifier**.

   ![](assets/8.png)

1. Sélectionnez **à chaque fois** et cliquez sur **Enregistrer**.

   ![](assets/9.png)

1. Cliquez sur **Activer**.

   ![](assets/10.png)

1. Cliquez sur **Activer** dans l’écran de confirmation.

   ![](assets/11.png)

>[!NOTE]
>
>Une fois principale, cette campagne s’exécute chaque fois qu’une personne remplit le formulaire spécifié. La campagne continue à s’exécuter jusqu’à ce qu’elle soit désactivée.

## Étape 3 : Remplir le formulaire {#step-fill-out-the-form}

1. Sélectionnez **Ma page**. Cela a été créé dans le [Landing page avec un Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) gain rapide.

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Cliquez sur **Afficher la page approuvée**.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   Votre landing page &quot;Essai gratuit&quot; s’ouvre dans un nouvel onglet.

1. Remplissez le formulaire avec votre prénom, votre nom et votre adresse électronique, puis cliquez sur **Envoyer**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Indiquez une adresse e-mail valide pour être sûr de bien recevoir l&#39;e-mail.

## Mission accomplie {#mission-complete}

En quelques minutes, vous devriez voir le courriel de réponse automatique dans votre boîte de réception. Bon boulot !

<br> 

[◄ Mission 3 : Évaluation simple](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Mission 5 : Importer une liste de leads ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
