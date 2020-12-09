---
unique-page-id: 10096683
description: Mises à jour de l'inscription sur Événement ON24 - Documents marketing - Documentation du produit
title: Mises à jour de l'abonnement Événement ON24
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# Mises à jour de l&#39;abonnement Événement ON24 {#on-event-registration-updates}

## Approbation manuelle des inscrits {#manually-approving-registrants}

Vous pouvez approuver manuellement vos inscrits avant de leur envoyer un courriel de confirmation. Pour ce faire, vous devez configurer vos campagnes pour qu’elles gèrent cette étape supplémentaire :

1. Campaign pour le déclencheur d&#39;inscription :

   * Dans la Liste dynamique, définissez le déclencheur sur **Remplit le formulaire**.
   * Dans le flux, définissez le statut en progression sur Approbation **** en attente.

1. Accédez au Événement et cliquez sur l&#39;onglet **Membres** . Cet onglet affiche toutes les personnes qui ont rempli le formulaire. Leur état doit être défini sur **En attente d’approbation**.
1. Utilisez le filtre en haut de la grille pour n&#39;vue que les personnes dont l&#39;état est Autorisation **** en attente.
1. Sélectionnez les personnes que vous souhaitez enregistrer (en maintenant la touche Maj enfoncée, en maintenant la touche Ctrl enfoncée ou en cliquant sur Sélectionner tout).
1. Dans le menu, cliquez sur **Modifier l’état**. Sélectionnez **Inscrit**, **Refusé** ou tout autre état applicable.

## Gestion des personnes avec une erreur d&#39;inscription {#handling-people-with-a-registration-error}

Si une personne n&#39;est pas enregistrée mais est plutôt définie sur l&#39;état Erreur d&#39;enregistrement, il n&#39;est pas trop tard pour récupérer.

1. Dans l&#39;onglet Membres, filtrez la liste des personnes avec l&#39;état Erreur **d&#39;** inscription.
1. Avant de continuer, vérifiez que vous avez déterminé et corrigé le problème avec l’intégration (vérifiez qu’il n’y a aucune erreur sous Partenaires **** Événement dans l’administration).
1. Une fois le problème résolu, sélectionnez toutes les personnes ayant le statut Erreur d’enregistrement et définissez leur statut sur **Inscrit**. Cela va tenter de les enregistrer à nouveau sur ON24.

## Mise à jour du statut des membres à partir d&#39;ON24 {#updating-member-status-from-on}

Marketo tire automatiquement les informations de présence vers 23h00 dans le Pacifique chaque nuit. Pour mettre à jour manuellement les informations de présence, cliquez sur **Actualiser à partir du fournisseur** de webinaires sous Actions ****&#x200B;Événement.

>[!MORELIKETHIS]
>
>* [Présentation des Événements d&#39;adaptateurs Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



