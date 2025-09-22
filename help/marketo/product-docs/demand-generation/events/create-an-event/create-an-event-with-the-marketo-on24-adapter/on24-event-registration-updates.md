---
unique-page-id: 10096683
description: Mises à jour de l’inscription aux événements ON24 - Documents Marketo - Documentation du produit
title: Mises à jour de l’inscription aux événements ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 2%

---

# Mises à jour de l’inscription aux événements ON24 {#on-event-registration-updates}

## Approuver manuellement des personnes inscrites {#manually-approving-registrants}

Vous pouvez approuver manuellement vos inscrits avant de leur envoyer un e-mail de confirmation. Pour ce faire, vous devez configurer vos campagnes pour gérer cette étape supplémentaire :

1. Pour la campagne Déclencheur d’enregistrement :

   * Dans la [!UICONTROL Liste dynamique], définissez le déclencheur sur **[!UICONTROL Remplit le formulaire]**.
   * Dans le flux, définissez le [!UICONTROL Statut en progression] sur **[!UICONTROL Approbation en attente]**.

1. Accédez à l’événement et cliquez sur l’onglet **[!UICONTROL Membres]**. Cet onglet affiche toutes les personnes qui ont rempli le formulaire. Leur statut doit être défini sur **[!UICONTROL Approbation en attente]**.
1. Utilisez le filtre en haut de la grille pour afficher uniquement les personnes dont le statut est **[!UICONTROL Approbation en attente]**.
1. Sélectionnez les personnes à enregistrer (Maj-clic, Ctrl-clic ou Tout sélectionner).
1. Dans le menu, cliquez sur **[!UICONTROL Modifier le statut]**. Sélectionnez **[!UICONTROL Enregistré]**, **[!UICONTROL Rejeté]** ou tout autre statut applicable.

## Gérer les personnes ayant rencontré une erreur d’enregistrement {#handling-people-with-a-registration-error}

Si une personne ne s’enregistre pas, mais qu’elle adopte le statut [!UICONTROL Erreur d’enregistrement], il n’est pas trop tard pour se remettre.

1. Dans l’onglet [!UICONTROL Membres], filtrez la liste des personnes dont le statut est **[!UICONTROL Erreur d’enregistrement]**.
1. Avant de poursuivre, assurez-vous d’avoir déterminé et corrigé le problème avec l’intégration (vérifiez qu’il n’y a aucune erreur sous **[!UICONTROL Partenaires d’événement]** dans Admin).
1. Une fois le problème résolu, sélectionnez toutes les personnes dont le statut est [!UICONTROL &#x200B; Erreur d’enregistrement &#x200B;] et modifiez leur statut en **[!UICONTROL Enregistré]**. Cette opération va tenter de les enregistrer à nouveau avec ON24.

## Mise à jour du statut de membre à partir d’ON24 {#updating-member-status-from-on}

Marketo extrait automatiquement les informations de présence vers 23h Pacifique chaque soir. Pour mettre à jour manuellement les informations de présence, cliquez sur **[!UICONTROL Actualiser à partir du fournisseur de webinaires]** sous **[!UICONTROL Actions d’événement]**.

>[!MORELIKETHIS]
>
>[Présentation des événements de l&#39;adaptateur Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
