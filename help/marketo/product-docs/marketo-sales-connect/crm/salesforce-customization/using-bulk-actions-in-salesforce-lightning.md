---
unique-page-id: 42762825
description: Utilisation d’actions en bloc dans Salesforce Lightning - Documentation de Marketo - Documentation du produit
title: Utilisation d’actions en bloc dans Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Utilisation d’actions en bloc dans [!DNL Salesforce Lightning] {#using-bulk-actions-in-salesforce-lightning}

Découvrez comment effectuer des actions en bloc, telles que l’ajout de prospects à une campagne, l’envoi d’un e-mail en bloc ou le transfert de prospects de [!DNL Salesforce] à [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Mettez à jour vers la dernière version du package [!DNL Sales Connect] et installez les boutons d’action en masse dans la vue de votre prospect/contact. [Cliquez ici pour obtenir des instructions](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Avant de suivre les étapes ci-dessous, assurez-vous d’être connecté à votre compte [!DNL Marketo Sales Connect].

## Bulk Email {#bulk-email}

1. Dans [!DNL Salesforce], cliquez sur l’onglet **[!UICONTROL Prospects]**, puis choisissez la liste des prospects souhaités.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Si vous êtes déjà sur la liste que vous utiliserez, vous devrez l&#39;exécuter à nouveau en la sélectionnant dans la liste déroulante afin de vous assurer que les boutons d&#39;action en masse du MSC s&#39;affichent. Il s’agit d’[!DNL Salesforce] comportement qui ne peut pas être modifié.

1. Cliquez sur la liste déroulante fléchée (à l’extrémité droite de l’écran) et sélectionnez **[!UICONTROL E-mail avec MSC]**.

   ![](assets/two-6.png)

1. Un e-mail du MSC s’affiche. Il comprend les fonctionnalités suivantes :

   a. Le champ « [!UICONTROL À] » affiche « Tous les accusés de réception » ; il correspond à la liste des prospects que vous avez choisie dans la vue Liste des prospects
b. Cette liste est visible dans le panneau de gauche sous le nom « Composition en bloc ». Vous pouvez ajouter ou supprimer des destinataires ici
c. Vous pouvez choisir un modèle ou créer votre propre e-mail
d. Vous pouvez envoyer l’e-mail immédiatement ou planifier son envoi à une date ultérieure

   ![](assets/three-5.png)

## Ajouter à la campagne {#add-to-campaign}

1. Dans [!DNL Salesforce], cliquez sur l’onglet **[!UICONTROL Prospects]**, puis choisissez la liste des prospects souhaités.

   ![](assets/four-4.png)

1. Cliquez sur la liste déroulante fléchée (à l’extrémité droite de l’écran) et sélectionnez **[!UICONTROL Ajouter à MSC Campaign]**.

   ![](assets/five-4.png)

1. Un pop-up « [!UICONTROL &#x200B; Ajouter des personnes à votre campagne &#x200B;] » s’affiche. Cliquez sur **[!UICONTROL Suivant]** et parcourez le flux de campagne type pour déclencher une campagne MSC.

   ![](assets/six-1.png)

## Intégrer à [!DNL Marketo Sales Connect] {#push-to-marketo-sales-connect}

1. Dans [!DNL Salesforce], cliquez sur l’onglet **[!UICONTROL Prospects]**, puis choisissez la liste des prospects souhaités.

   ![](assets/seven-2.png)

1. Cliquez sur la liste déroulante Flèche (à l’extrémité droite de l’écran) et sélectionnez **[!UICONTROL Push to MSC]**.

   ![](assets/eight-2.png)

1. Un nouvel onglet appelé « [!DNL Salesforce] Bridge » s’ouvre. Cliquez sur le bouton **[!UICONTROL Passer au groupe] →**.

   ![](assets/nine-2.png)

1. Vous serez envoyé à votre compte MSC où vous verrez un groupe créé avec un horodatage. Vous recevrez une notification une fois la synchronisation terminée et le groupe inclura les prospects synchronisés à partir de [!DNL Salesforce].

   ![](assets/ten-1.png)

>[!NOTE]
>
>Vous pouvez également suivre les mêmes étapes pour utiliser des actions en bloc dans la vue Liste de contacts.

>[!MORELIKETHIS]
>
>* [Envoi d’e-mails via l’e-mail du groupe](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composition d’e-mails en bloc avec sélection et envoi](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
