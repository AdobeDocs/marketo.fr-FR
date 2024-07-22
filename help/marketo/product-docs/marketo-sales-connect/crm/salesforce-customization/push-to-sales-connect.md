---
unique-page-id: 14352477
description: Push to Sales Connect - Marketo Docs - Documentation du produit
title: Push to Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Push to Sales Connect {#push-to-sales-connect}

Notre bouton Push to Tout (Envoyer à tout) contiendra une liste de vos prospects/contacts dans Salesforce et les placera dans un groupe dans Sales Connect (Connexion aux ventes). Vous pouvez ensuite envoyer rapidement un e-mail de groupe personnalisable en pièce jointe du suivi Tout.

## Exigences {#requirements}

* Package Salesforce Sales Connect installé par l’administrateur Salesforce

* Bouton Push to Sales Connect (Envoyer à la connexion aux ventes) installé en mode Liste par l’administrateur Salesforce

* Connexion Salesforce établie avec Sales Connect pour un utilisateur qui effectue les notifications push

## Comment {#how-to}

1. Cliquez sur l’onglet **Lead/Contact** dans Salesforce.
1. Basculez vers le mode Liste que vous souhaitez passer à la connexion aux ventes en regard du bouton Atteindre .
1. Cliquez sur **Go**.
1. Sélectionnez tous les pistes/contacts que vous souhaitez transférer.
1. Sélectionnez **Push to MSE**.
1. Une nouvelle fenêtre s’affiche pour vérifier le nombre de pistes/contacts que vous souhaitez transférer. Sélectionnez **Passez au groupe**. Sales Connect ne redirigera pas les contacts marqués comme Email Opt Out dans Salesforce ou Désabonné dans Sales Connect.

   >[!NOTE]
   >
   >Sales Connect ajoutera ce groupe intitulé &quot;SFDC-...&quot; à la page Relationships sur l’ [application web](https://toutapp.com/login).

1. Sélectionnez **Email Entire Group** pour envoyer l’e-mail de ce groupe.
