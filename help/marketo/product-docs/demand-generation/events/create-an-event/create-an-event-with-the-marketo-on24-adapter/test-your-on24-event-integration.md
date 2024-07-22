---
unique-page-id: 10096677
description: Test de votre intégration d’événement ON24 - Documents Marketo - Documentation du produit
title: Test de votre intégration d’événement ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Test de votre intégration d’événement ON24 {#test-your-on-event-integration}

Veillez à tester minutieusement votre intégration d’événement.

## Séquence De Test Recommandée Avant D’Exécuter Votre Première Campagne {#recommended-test-sequence-before-running-your-first-campaign}

1. Remplissez le formulaire d’enregistrement de l’événement et utilisez une adresse électronique valide pour le test.
1. Confirmez que le nom du test s’affiche avec un état **Registered** dans la grille Adhésion de votre événement Marketo.
1. Confirmez que le nom du test s’affiche également comme **Registered** dans ON24.
1. Vérifiez que l’adresse électronique valide que vous avez utilisée pour enregistrer le nom du test a reçu un email de confirmation pour l’événement et que l’URL unique est résolue dans l’email.

   >[!NOTE]
   >
   >Vous devez utiliser le jeton `{{member.webinar url}}` dans votre email de confirmation pour que l’URL unique s’affiche dans l’email de chaque inscrit.

## Après l’événement {#after-the-event}

Voici comment les données sont mises à jour après l’événement :

* Marketo récupère toutes les nuits les données des participants sur ON24.
* Une fois que les données du participant sont synchronisées entre Marketo et ON24, Marketo met à jour l’état de l’adhésion sur Participé, Participé à la demande ou Aucun affichage. Dans l’onglet **Summary** de l’événement, l’état de l’événement est mis à jour vers **Event Complete**.

>[!MORELIKETHIS]
>
>* [Exemple d’intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Compréhension des événements d’adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
