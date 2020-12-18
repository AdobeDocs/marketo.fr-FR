---
unique-page-id: 14352477
description: Connexion aux ventes - Documents marketing - Documentation sur les produits
title: Connexion client
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Envoyer à la connexion commerciale {#push-to-sales-connect}

Notre bouton Push to Tout prendra une liste de vos pistes/contacts dans Salesforce et les poussera dans un groupe dans Sales Connect. Vous pouvez ensuite envoyer rapidement un courriel de groupe personnalisable avec le suivi Tout en pièce jointe.

## Exigences {#requirements}

* Sales Connect [Package Salesforce](http://docs.marketo.com/x/C4PS) installé par `Salesforce Admin`

* `Push to Sales Connect`bouton installé sur la vue de liste par  `Salesforce Admin`

* Connexion Salesforce créée avec Sales Connect pour l&#39;utilisateur qui effectue le Push

## Comment {#how-to}

1. Cliquez sur l&#39;onglet **Piste/Contact** dans Salesforce.
1. Basculez vers la Vue de Liste que vous souhaitez utiliser pour envoyer à Sales Connect en regard du bouton Go (Atteindre).
1. Cliquez sur **Aller**.
1. Sélectionnez tous les prospects/contacts que vous souhaitez pousser à diffuser.
1. Sélectionnez **Push to MSE**.
1. Une nouvelle fenêtre s&#39;affiche pour vérifier le nombre de pistes/contacts que vous souhaitez transférer. Sélectionnez **Passez au groupe**. Sales Connect `will not push over` tous les contacts marqués comme `Email Opt Out` dans Salesforce ou `Unsubscribed` dans Sales Connect.

   >[!NOTE]
   >
   >Sales Connect ajoutera ce groupe intitulé &quot;SFDC-..&quot;. à la page Relations de l&#39;[application Web](http://toutapp.com/login).

1. Sélectionnez **E-mail Groupe entier** pour envoyer le courriel de ce groupe.

