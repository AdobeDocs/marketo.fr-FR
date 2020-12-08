---
unique-page-id: 2359416
description: Réponse automatique par courriel - Documents marketing - Documentation du produit
title: Réponse automatique du courriel
translation-type: tm+mt
source-git-commit: 09dbd3a141fed0525aec8bf1ca6d141be2a6ce46
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Réponse automatique du courriel {#email-auto-response}

## Mission : Envoyer un e-mail de remerciement lorsqu’une personne remplit un formulaire {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>**Conditions préalables**
>
>* [Configurer et Ajouter une personne](get-set-up-and-add-a-person.md)
>* [landing page avec un formulaire](landing-page-with-a-form.md)

>



## Étape 1 : Créer un courriel {#step-create-an-email}

1. Accédez à la zone Activités marketing.

   ![](assets/one-2.png)

1. Sélectionnez Mon Programme dans le menu de gauche, cliquez sur la liste déroulante Nouveau, puis sélectionnez Nouveau fichier local.

   ![](assets/two-3.png)

1. Cliquez sur Courriel.

   ![](assets/three-2.png)

1. Nommez votre adresse électronique &quot;Courriel de réponse automatique&quot;, choisissez un modèle et cliquez sur Créer.

   ![](assets/four-1.png)

   Un éditeur de courrier électronique s’ouvre dans une nouvelle fenêtre ou un nouvel onglet. Si les fenêtres contextuelles sont bloquées, cliquez sur** Modifier le brouillon** sur la page de résumé des ressources pour accéder au courrier électronique.

1. Entrez un objet, puis cliquez sur la zone modifiable du courrier électronique en maintenant le doublon enfoncé.

   ![](assets/five-2.png)

   Un éditeur de texte enrichi s’ouvre au-dessus de l’éditeur de courrier électronique.

1. Mettez en surbrillance le contenu du courrier électronique existant.

   ![](assets/six-2.png)

1. Saisissez votre contenu de courrier électronique et cliquez sur Enregistrer.

   ![](assets/seven-2.png)

1. Vos modifications sont enregistrées automatiquement. Fermez l’onglet/la fenêtre de l’éditeur de courrier électronique.

   ![](assets/eight-1.png)

1. Sélectionnez votre nouveau courriel. Sous Actions par courrier électronique, cliquez sur Approuver.

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Étape 2 : Créer une Campaign intelligente {#step-create-a-smart-campaign}

1. Cliquez avec le bouton droit sur **Mon Programme** et cliquez sur **Nouvelle Campaign** intelligente.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Nommez** votre campagne &quot;Campaign de réponse automatique&quot; et cliquez sur **Créer**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Accédez à l&#39;onglet **Smart Liste **.

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Nous configurons cette campagne pour qu’elle s’exécute chaque fois qu’une personne remplit le formulaire que vous avez créé en [**Landing page avec un formulaire**](landing-page-with-a-form.md).

1. Recherchez et faites glisser le déclencheur **Remplir le formulaire** sur le canevas de gauche.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Sélectionnez **Mon formulaire** dans la liste déroulante. Cliquez sur l&#39;onglet **Flux **.

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Faites glisser l&#39;action **Envoyer un e-mail **flow vers le canevas de gauche.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Sélectionnez votre courriel **de réponse** automatique et accédez à l&#39;onglet **Planification **onglet.

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Cliquez sur **Modifier**.

   ![](assets/8.png)
Sélectionnez chaque fois et cliquez sur Enregistrer.
   ![](assets/9.png)

1. Cliquez sur **Activer**.

   ![](assets/10.png)

1. Cliquez sur **Activer **dans l’écran de confirmation.

   ![](assets/11.png)

>[!NOTE]
>
>Une fois principale, cette campagne s’exécute chaque fois qu’une personne remplit le formulaire spécifié. La campagne continue à s’exécuter jusqu’à ce qu’elle soit désactivée.

## Étape 3 : Remplir le formulaire {#step-fill-out-the-form}

1. Sélectionnez **Ma page**. Cette opération a été créée dans le [Landing page avec une victoire rapide sur le formulaire](landing-page-with-a-form.md) .

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Cliquez sur Page **Approuvée** Vue.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   Votre landing page &quot;Essai gratuit&quot; s’ouvre dans un nouvel onglet.

1. Renseignez le formulaire avec votre prénom, votre nom et votre adresse électronique, puis cliquez sur **Envoyer**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Veillez à utiliser votre adresse électronique réelle pour obtenir le courriel.

## Fin de la mission {#mission-complete}

En quelques minutes, vous devriez voir le courriel de réponse automatique dans votre boîte de réception. Super boulot !

<br> 

[Mission 3 : Score simple](simple-scoring.md) [Mission 5 : Importer une Liste de pistes ►](import-a-list-of-people.md)