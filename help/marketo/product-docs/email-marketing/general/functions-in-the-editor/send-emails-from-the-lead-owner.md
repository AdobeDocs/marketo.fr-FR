---
unique-page-id: 1147340
description: Envoyer des e-mails du propriétaire du lead - Documents Marketo - Documentation du produit
title: Envoyer des e-mails depuis l’entité propriétaire du lead
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 7%

---

# Envoyer des e-mails depuis l’entité propriétaire du lead {#send-emails-from-the-lead-owner}

Que se passe-t-il si vous souhaitez envoyer un e-mail à un prospect au nom du propriétaire du prospect ?  Voici comment faire.

1. Recherchez votre e-mail, sélectionnez-le et cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/one.png)

1. Cliquez dans le champ **[!UICONTROL De]** (supprimez tout nom existant), puis cliquez sur le bouton **Insérer un jeton**.

   ![](assets/two.png)

1. Commencez à saisir « `{{lead.Lead Owner` » et sélectionnez le jeton **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Saisissez une valeur par défaut au cas où le prospect n’a pas encore de propriétaire, puis cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Cliquez après le premier jeton, ajoutez un espace, puis cliquez sur le bouton **Insérer un jeton**.

   ![](assets/five.png)

1. Commencez à saisir « `{{lead.Lead Owner` » et sélectionnez le jeton **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Saisissez une valeur par défaut au cas où le prospect n’a pas encore de propriétaire, puis cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Veillez à ajouter un espace entre les jetons de prénom et de nom.

1. Cliquez dans le champ **[!UICONTROL Adresse de l’expéditeur]** (supprimez toute adresse e-mail existante), puis cliquez sur le bouton **Insérer un jeton**.

   ![](assets/eight.png)

1. Commencez à saisir « `{{lead.Lead Owner` » et sélectionnez le jeton **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Saisissez une valeur par défaut au cas où le prospect n’a pas encore de propriétaire, puis cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/ten.png)

1. Assurez-vous que les champs **[!UICONTROL Répondre à]** et **[!UICONTROL Objet]** sont renseignés, et vous avez terminé !

   ![](assets/eleven.png)
