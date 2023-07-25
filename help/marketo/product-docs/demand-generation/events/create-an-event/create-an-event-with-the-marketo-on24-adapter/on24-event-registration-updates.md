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

Vous pouvez approuver manuellement vos inscrits avant de leur envoyer un email de confirmation. Pour ce faire, vous devrez configurer vos campagnes pour gérer cette étape supplémentaire :

1. Pour la campagne de déclenchement d&#39;enregistrement :

   * Dans la liste dynamique, définissez le déclencheur sur **Remplir le formulaire**.
   * Dans le flux, définissez l’état de progression sur **En attente d’approbation**.

1. Accédez à l’événement et cliquez sur le bouton **Membres** . Cet onglet affiche toutes les personnes qui ont rempli le formulaire. Leur état doit être défini sur **En attente d’approbation**.
1. Utilisez le filtre en haut de la grille pour afficher uniquement les personnes dont l’état est **En attente d’approbation**.
1. Sélectionnez les personnes que vous souhaitez enregistrer (cliquez tout ou cliquez en maintenant la touche Maj enfoncée).
1. Dans le menu, cliquez sur **Modifier l’état**. Sélectionner **Inscrits**, **Rejetés** ou tout autre état applicable.

## Gestion des personnes avec une erreur d’enregistrement {#handling-people-with-a-registration-error}

Si une personne n’est pas enregistrée, mais plutôt définie sur l’état Erreur d’enregistrement, il n’est pas trop tard pour récupérer.

1. Depuis l&#39;onglet Membres , filtrez la liste des personnes ayant le statut **Erreur d’enregistrement**.
1. Avant de poursuivre, assurez-vous d’avoir déterminé et corrigé le problème avec l’intégration (vérifiez qu’il n’y a aucune erreur sous **Partenaires d’événement** dans Admin).
1. Une fois le problème résolu, sélectionnez toutes les personnes ayant le statut Erreur d’enregistrement et définissez leur statut sur **Inscrits**. Cela va tenter de les enregistrer à nouveau sur ON24.

## Mise à jour de l’état du membre à partir d’ON24 {#updating-member-status-from-on}

Marketo récupère automatiquement les informations de présence aux alentours de 23h dans le Pacifique chaque nuit. Pour mettre manuellement à jour les informations de présence, cliquez sur **Actualisation à partir du fournisseur de webinaire** under **Actions d’événement**.

>[!MORELIKETHIS]
>
>[Présentation des événements de l’adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
