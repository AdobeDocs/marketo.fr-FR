---
unique-page-id: 42762794
description: Utilisation d’actions en bloc dans Salesforce Classic - Documents Marketo - Documentation du produit
title: Utilisation d’actions en bloc dans Salesforce Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 2%

---

# Utilisation d’actions en bloc dans Salesforce Classic {#using-bulk-actions-in-salesforce-classic}

Découvrez comment exécuter des actions en bloc, comme ajouter des pistes à une campagne, envoyer un courrier électronique en bloc ou envoyer des pistes de Salesforce à Sales Connect.

>[!PREREQUISITES]
>
>Mettez à jour vers la dernière version du package Sales Connect et installez les boutons d’action en bloc dans votre vue de prospect/contact. [Cliquez ici pour obtenir des instructions](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Avant de suivre les étapes décrites, vérifiez que vous êtes connecté à votre compte Marketo Sales Connect.

## Courrier électronique en bloc {#bulk-email}

1. Dans Salesforce, cliquez sur l’icône **Pistes** , puis le **Aller** bouton .

   ![](assets/one-5.png)

1. Sélectionnez les pistes souhaitées et cliquez sur le bouton **Courrier électronique avec MSC (Classic)** bouton .

   ![](assets/two-5.png)

1. Un e-mail du MSC apparaîtra. Elle comprend les fonctionnalités suivantes :

   a. Le champ &quot;À&quot; affiche &quot;Tous les accusés de réception&quot;, ce qui correspond à la liste des prospects que vous avez sélectionnés en mode Liste de pistes.\
   b. Cette liste est visible dans le panneau de gauche intitulé &quot;Compression en masse&quot;. Vous pouvez y ajouter/supprimer des destinataires.\
   c. Vous pouvez choisir un modèle ou créer votre propre email\
   d. Vous pouvez prévisualiser les champs dynamiques qui seront renseignés dans votre email\
   e. Vous pouvez envoyer l’email immédiatement ou programmer son envoi ultérieurement.

   ![](assets/three-4.png)

## Ajouter à la campagne  {#add-to-campaign}

1. Dans Salesforce, cliquez sur l’icône **Pistes** , puis le **Aller** bouton .

   ![](assets/four-3.png)

1. Sélectionnez les pistes souhaitées et cliquez sur le bouton **Ajouter à MSC Campaign (Classic)** bouton .

   ![](assets/five-3.png)

1. Une fenêtre contextuelle &quot;Ajouter des personnes à votre campagne&quot; s’affiche. Cliquez sur **Suivant** et parcourir le flux de campagne type pour déclencher une campagne du MSC.

   ![](assets/six.png)

## Intégrer à Marketo Sales Connect {#push-to-marketo-sales-connect}

1. Dans Salesforce, cliquez sur l’icône **Pistes** , puis le **Aller** bouton .

   ![](assets/seven-1.png)

1. Sélectionnez les pistes souhaitées et cliquez sur le bouton **Push to MSC (Classic)** bouton .

   ![](assets/eight-1.png)

1. Un nouvel onglet appelé &quot;Salesforce Bridge&quot; s’ouvre. Cliquez sur le bouton **Passez à la → Groupe** bouton .

   ![](assets/nine-1.png)

1. Vous serez envoyé à votre compte MSC où un groupe sera créé avec l’horodatage. Vous recevrez une notification une fois la synchronisation terminée et le groupe inclura les pistes synchronisées à partir de Salesforce.

   ![](assets/ten.png)

>[!NOTE]
>
>Vous pouvez également suivre les mêmes étapes pour utiliser des actions en bloc en mode Liste des contacts.

>[!MORELIKETHIS]
>
>* [Envoi d’emails par courrier électronique de groupe](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composition d’emails en bloc avec sélection et envoi](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

