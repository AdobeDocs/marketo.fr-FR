---
unique-page-id: 10096683
description: Mises à jour de l’enregistrement des événements ON24 - Documents Marketo - Documentation du produit
title: Mises à jour de l’enregistrement d’événement ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Mises à jour de l’enregistrement d’événement ON24 {#on-event-registration-updates}

## Validation manuelle des inscrits {#manually-approving-registrants}

Vous pouvez approuver manuellement vos inscrits avant de leur envoyer un email de confirmation. Pour ce faire, vous devez configurer vos campagnes afin de gérer cette étape supplémentaire :

1. Pour la campagne de déclenchement d&#39;enregistrement :

   * Dans la liste dynamique, définissez le déclencheur sur **Remplit le formulaire**.
   * Dans le flux, définissez l’état de progression sur **Autorisation en attente**.

1. Accédez à l’événement et cliquez sur l’onglet **Membres** . Cet onglet affiche toutes les personnes qui ont rempli le formulaire. Leur état doit être défini sur **Autorisation en attente**.
1. Utilisez le filtre en haut de la grille pour afficher uniquement les personnes dont l’état est **En attente d’approbation**.
1. Sélectionnez les personnes que vous souhaitez enregistrer (cliquez tout ou cliquez en maintenant la touche Maj enfoncée).
1. Dans le menu, cliquez sur **Modifier l’état**. Sélectionnez **Registered**, **Rejected** ou tout autre état applicable.

## Gestion des personnes avec une erreur d’enregistrement {#handling-people-with-a-registration-error}

Si une personne n’est pas enregistrée, mais plutôt définie sur l’état Erreur d’enregistrement, il n’est pas trop tard pour récupérer.

1. Dans l&#39;onglet Membres , filtrez la liste des personnes ayant le statut **Erreur d&#39;enregistrement**.
1. Avant de poursuivre, assurez-vous d’avoir déterminé et corrigé le problème avec l’intégration (vérifiez qu’il n’y a aucune erreur sous **Event Partners** dans Admin).
1. Une fois le problème résolu, sélectionnez toutes les personnes ayant le statut Erreur d’enregistrement et remplacez leur statut par **Registered**. Cela tentera de les enregistrer à nouveau auprès de ON24.

## Mise à jour de l’état du membre à partir d’ON24 {#updating-member-status-from-on}

Marketo récupère automatiquement les informations de présence aux alentours de 23h dans le Pacifique chaque nuit. Pour mettre à jour manuellement les informations de fréquentation, cliquez sur **Actualiser à partir du fournisseur de webinaires** sous **Actions d’événement**.

>[!MORELIKETHIS]
>
>[Compréhension des événements d’adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
