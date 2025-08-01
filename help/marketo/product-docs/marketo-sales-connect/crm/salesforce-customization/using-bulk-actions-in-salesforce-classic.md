---
unique-page-id: 42762794
description: Utilisation d’actions en bloc dans  [!DNL Salesforce]  Classic - Documents Marketo - Documentation du produit
title: Utilisation d’actions en bloc dans  [!DNL Salesforce]  Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 2%

---

# Utilisation d’actions en bloc dans [!DNL Salesforce] Classic {#using-bulk-actions-in-salesforce-classic}

Découvrez comment effectuer des actions en bloc, telles que l’ajout de prospects à une campagne, l’envoi d’un e-mail en bloc ou le transfert de prospects de [!DNL Salesforce] à [!DNL Sales Connect].

>[!PREREQUISITES]
>
>Mettez à jour vers la dernière version du package [!DNL Sales Connect] et installez les boutons d’action en masse dans la vue de votre prospect/contact. [Cliquez ici pour obtenir des instructions](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Avant de suivre les étapes décrites, assurez-vous d’être connecté à votre compte Marketo Sales Connect.

## Bulk Email {#bulk-email}

1. Dans [!DNL Salesforce], cliquez sur l’onglet **[!UICONTROL Leads]**, puis sur le bouton **[!UICONTROL Aller]**.

   ![](assets/one-5.png)

1. Choisissez les leads souhaités et cliquez sur le bouton **[!UICONTROL E-mail avec MSC (Classic)]**.

   ![](assets/two-5.png)

1. Un e-mail du MSC s’affiche. Il comprend les fonctionnalités suivantes :

   a. Le champ « [!UICONTROL À] » affiche « [!UICONTROL Tous les destinataires] » ; il correspond à la liste des prospects que vous avez choisie dans la vue Liste des prospects
b. Cette liste est visible dans le panneau de gauche sous le nom « [!UICONTROL Composition en bloc] ». Vous pouvez ajouter ou supprimer des destinataires ici
c. Vous pouvez choisir un modèle ou créer votre propre e-mail
d. Vous pouvez prévisualiser les champs dynamiques qui seront renseignés dans votre e-mail.
e. Vous pouvez envoyer l’e-mail immédiatement ou planifier son envoi à une date ultérieure

   ![](assets/three-4.png)

## Ajouter à la campagne {#add-to-campaign}

1. Dans [!DNL Salesforce], cliquez sur l’onglet **[!UICONTROL Leads]**, puis sur le bouton **[!UICONTROL Aller]**.

   ![](assets/four-3.png)

1. Choisissez les leads souhaités et cliquez sur le bouton **[!UICONTROL Ajouter à MSC Campaign (Classic)]**.

   ![](assets/five-3.png)

1. Un pop-up « [!UICONTROL &#x200B; Ajouter des personnes à votre campagne &#x200B;] » s’affiche. Cliquez sur **[!UICONTROL Suivant]** et parcourez le flux de campagne type pour déclencher une campagne MSC.

   ![](assets/six.png)

## Intégrer à Marketo Sales Connect {#push-to-marketo-sales-connect}

1. Dans [!DNL Salesforce], cliquez sur l’onglet **[!UICONTROL Leads]**, puis sur le bouton **[!UICONTROL Aller]**.

   ![](assets/seven-1.png)

1. Choisissez les leads souhaités et cliquez sur le bouton **[!UICONTROL Push to MSC (Classic)]**.

   ![](assets/eight-1.png)

1. Un nouvel onglet appelé « [!UICONTROL Salesforce Bridge] » s’ouvre. Cliquez sur le bouton **[!UICONTROL Accéder au groupe→]**.

   ![](assets/nine-1.png)

1. Vous serez envoyé à votre compte MSC où vous verrez un groupe créé avec un horodatage. Vous recevrez une notification une fois la synchronisation terminée et le groupe inclura les prospects synchronisés à partir de [!DNL Salesforce].

   ![](assets/ten.png)

>[!NOTE]
>
>Vous pouvez également suivre les mêmes étapes pour utiliser des actions en bloc dans la vue Liste de contacts.

>[!MORELIKETHIS]
>
>* [Envoi d’e-mails via l’e-mail du groupe](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composition d’e-mails en bloc avec sélection et envoi](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
