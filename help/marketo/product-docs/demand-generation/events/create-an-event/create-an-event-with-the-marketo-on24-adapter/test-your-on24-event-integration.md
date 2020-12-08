---
unique-page-id: 10096677
description: Testez votre intégration de Événement ON24 - Docs marketing - Documentation du produit
title: Testez votre intégration de Événement ON24
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Testez votre intégration de Événement ON24 {#test-your-on-event-integration}

Assurez-vous de tester minutieusement l’intégration de votre événement.

## Séquence de test recommandée avant d’exécuter votre première Campaign {#recommended-test-sequence-before-running-your-first-campaign}

1. Remplissez le formulaire d&#39;inscription du événement et utilisez une adresse électronique valide pour le test.
1. Vérifiez que le nom du test s’affiche avec un statut **Enregistré** dans la grille d’adhésion de votre événement Marketo.
1. Vérifiez que le nom du test s’affiche également comme **Enregistré** dans ON24.
1. Vérifiez que l’adresse électronique valide que vous avez utilisée pour enregistrer le nom du test a reçu un courrier électronique de confirmation au Événement et que l’URL unique est résolue dans le courrier électronique.

   >[!NOTE]
   >
   >Vous devez utiliser le `{{member.webinar url}}` jeton dans votre message de confirmation pour que l’URL unique s’affiche dans le message de chaque inscrit.

## Après le Événement {#after-the-event}

Voici comment les données sont mises à jour après le événement :

* Marketo récupère toutes les nuits les données des participants sur ON24.
* Une fois que les données du participant se synchronisent entre Marketo et ON24, Marketo met à jour l’état de l’adhésion en Participation, Participation à la demande ou Pas d’affichage. Dans l’onglet **Résumé** du événement, l’état du événement est mis à jour sur **Événement terminé**.

>[!NOTE]
>
>**Articles connexes**
>
>* [Exemple d’intégration de Événement ON24](example-on24-event-integration.md)
>* [Présentation des Événements d&#39;adaptateurs Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



