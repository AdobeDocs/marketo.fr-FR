---
unique-page-id: 1147340
description: Envoi d’emails à partir du propriétaire de piste - Documents Marketo - Documentation du produit
title: Envoi d’emails par le propriétaire du prospect
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Envoi d’emails par le propriétaire du prospect {#send-emails-from-the-lead-owner}

Que se passe-t-il si vous souhaitez envoyer un email à un prospect au nom du propriétaire du prospect ?  Voici comment.

1. Recherchez votre email, sélectionnez-le, puis cliquez sur **Modifier le brouillon**.

   ![](assets/one.png)

1. Cliquez sur dans le **De** (supprimez tout nom existant), puis cliquez sur le bouton **Insérer un jeton** bouton .

   ![](assets/two.png)

1. Commencez à taper &quot;`{{lead.Lead Owner`&quot; et sélectionnez la variable **`{{lead.Lead Owner First Name}}`** jeton.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Saisissez une valeur par défaut si le prospect ne dispose pas encore d’un propriétaire de piste et cliquez sur **Insérer**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Cliquez sur après le premier jeton, ajoutez un espace, puis cliquez sur le bouton **Insérer un jeton** bouton .

   ![](assets/five.png)

1. Commencez à taper &quot;`{{lead.Lead Owner`&quot; et sélectionnez la variable **`{{lead.Lead Owner Last Name}}`** jeton.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Saisissez une valeur par défaut si le prospect ne dispose pas encore d’un propriétaire de piste et cliquez sur **Insérer**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Veillez à ajouter un espace entre les jetons de prénom et de nom.

1. Cliquez dans le champ De l’e-mail (supprimez toute adresse électronique existante), puis cliquez sur le bouton Insérer un jeton .

   ![](assets/eight.png)

1. Commencez à taper &quot;`{{lead.Lead Owner`&quot; et sélectionnez la variable **`{{lead.Lead Owner Email Address}}`** jeton.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Saisissez une valeur par défaut si le prospect ne dispose pas encore d’un propriétaire de piste et cliquez sur **Insérer**.

   ![](assets/ten.png)

1. Assurez-vous que la variable **Réponse** et **Objet** sont renseignés, et vous avez terminé !

   ![](assets/eleven.png)
