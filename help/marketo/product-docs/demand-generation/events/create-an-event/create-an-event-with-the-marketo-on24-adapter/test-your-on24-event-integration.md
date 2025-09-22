---
unique-page-id: 10096677
description: Testez votre intégration d’événement ON24 - Documents Marketo - Documentation du produit
title: Tester votre intégration d’événement ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 5%

---

# Tester votre intégration d’événement ON24 {#test-your-on-event-integration}

Veillez à tester minutieusement votre intégration d’événement.

## Séquence De Test Recommandée Avant L’Exécution De Votre Première Campagne {#recommended-test-sequence-before-running-your-first-campaign}

1. Remplissez le formulaire d’inscription à l’événement et utilisez une adresse e-mail valide pour effectuer le test.
1. Confirmez que le nom du test s’affiche avec un statut **Enregistré** dans la grille Abonnement de votre événement Marketo.
1. Vérifiez que le nom du test s’affiche également comme **Enregistré** dans ON24.
1. Vérifiez que l’adresse e-mail valide que vous avez utilisée pour enregistrer le nom du test a reçu un e-mail de confirmation pour l’événement et que l’URL unique est résolue dans l’e-mail.

   >[!NOTE]
   >
   >Vous devez utiliser le jeton `{{member.webinar url}}` dans votre e-mail de confirmation pour que l’URL unique s’affiche dans l’e-mail de chaque personne inscrite.

## Après l’événement {#after-the-event}

Voici comment les données sont mises à jour après que l’événement a lieu :

* Marketo récupère les données des participants d’ON24 toutes les nuits.
* Une fois que les données du participant se synchronisent entre Marketo et ON24, Marketo met à jour le statut d’abonnement sur [!UICONTROL Terminé], [!UICONTROL Terminé à la demande] ou [!UICONTROL Aucun affichage]. Dans l’onglet **[!UICONTROL Résumé]** de l’événement, le statut de l’événement est mis à jour sur **[!UICONTROL Événement terminé]**.

>[!MORELIKETHIS]
>
>* [Exemple d’intégration d’événement ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Présentation des événements de l&#39;adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
