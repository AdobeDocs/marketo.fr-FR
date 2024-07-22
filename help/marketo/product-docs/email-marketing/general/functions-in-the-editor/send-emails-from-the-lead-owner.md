---
unique-page-id: 1147340
description: Envoi d’emails à partir du propriétaire de piste - Documents Marketo - Documentation du produit
title: Envoi d’emails par le propriétaire du prospect
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Envoi d’emails par le propriétaire du prospect {#send-emails-from-the-lead-owner}

Que se passe-t-il si vous souhaitez envoyer un email à un prospect au nom du propriétaire du prospect ?  Voici comment.

1. Recherchez votre email, sélectionnez-le et cliquez sur **Modifier le brouillon**.

   ![](assets/one.png)

1. Cliquez dans le champ **De** (supprimez tout nom existant), puis cliquez sur le bouton **Insérer un jeton** .

   ![](assets/two.png)

1. Commencez à saisir &quot;`{{lead.Lead Owner`&quot; et sélectionnez le jeton **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Saisissez une valeur par défaut si le prospect n&#39;a pas encore de propriétaire de prospect et cliquez sur **Insérer**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Cliquez sur après le premier jeton, ajoutez un espace, puis cliquez sur le bouton **Insérer un jeton**.

   ![](assets/five.png)

1. Commencez à saisir &quot;`{{lead.Lead Owner`&quot; et sélectionnez le jeton **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Saisissez une valeur par défaut si le prospect n&#39;a pas encore de propriétaire de prospect et cliquez sur **Insérer**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Veillez à ajouter un espace entre les jetons de prénom et de nom.

1. Cliquez dans le champ De l’e-mail (supprimez toute adresse électronique existante), puis cliquez sur le bouton Insérer un jeton .

   ![](assets/eight.png)

1. Commencez à saisir &quot;`{{lead.Lead Owner`&quot; et sélectionnez le jeton **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Saisissez une valeur par défaut si le prospect n&#39;a pas encore de propriétaire de prospect et cliquez sur **Insérer**.

   ![](assets/ten.png)

1. Assurez-vous que les champs **Réponse** et **Objet** sont renseignés et que vous avez terminé !

   ![](assets/eleven.png)
