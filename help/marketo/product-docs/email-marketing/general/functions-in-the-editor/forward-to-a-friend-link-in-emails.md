---
unique-page-id: 1900581
description: Transférer vers un lien d’ami dans les e-mails - Documents Marketo - Documentation du produit
title: Lien de transfert à un ami ou une amie dans les e-mails
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 2%

---

# Lien de transfert à un ami ou une amie dans les e-mails {#forward-to-a-friend-link-in-emails}

L&#39;ajout du lien « Transférer à un ami » à vos e-mails permet de suivre les personnes qui ont reçu un e-mail transféré via ce lien et de les ajouter automatiquement en tant que nouvelles personnes si elles ne figurent pas déjà dans la base de données.

Supposons, par exemple, que Keith utilise le lien « Transférer à un ami » pour transférer l’e-mail à une personne inconnue, Mark. Mark est automatiquement ajouté en tant que nouvelle personne, se voit attribuer son propre cookie et toute son activité e-mail et web lui est liée. Cependant, si Keith utilise le bouton de transfert dans son client de messagerie, Mark est incorrectement cookie en tant que Keith et son activité est consignée en tant que Keith.

## Ajouter un lien vers un modèle d’e-mail {#add-the-link-to-an-email-template}

1. Accédez au **[!UICONTROL Design Studio]**.

   ![](assets/one-8.png)

1. Recherchez et sélectionnez le modèle d’e-mail auquel vous souhaitez ajouter le lien. Cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/two-7.png)

1. Collez le code HTML suivant à l&#39;endroit où vous souhaitez que le lien &#39;Transférer à un ami&#39; apparaisse (si vous avez besoin d&#39;aide sur cette partie, veuillez vous rapprocher de votre développeur web) :

   `<a href="{{system.forwardToFriendLink}}">Forward to Friend</a>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Vous pouvez ajouter un style au lien pour le rendre plus attrayant. Par exemple :
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Il est déconseillé d’utiliser le style **position:relative** dans votre modèle d’e-mail. Cela peut créer des problèmes de position et d&#39;affichage de la zone « Transférer à un ami ».

1. Cliquez sur **[!UICONTROL Prévisualiser le brouillon]** pour vous assurer que le modèle a l’aspect souhaité.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >N’oubliez pas d’approuver le brouillon du modèle pour appliquer les modifications.

   Désormais, tous les e-mails qui utilisent ce modèle auront le lien « Transférer à un ami ». Lorsque le destinataire de l’e-mail clique dessus, il est redirigé vers une version web de l’e-mail avec la case « Transférer à un ami » :

   ![](assets/f2afbox.png)

## Ajouter le lien vers un e-mail individuel {#add-the-link-to-an-individual-email}

Vous pouvez également ajouter le lien « Transférer à un ami » directement dans un e-mail.

1. Ouvrez l’e-mail dans lequel vous souhaitez inclure le lien, puis double-cliquez dans la zone modifiable.

   ![](assets/five-4.png)

1. Placez le curseur à l’endroit où vous souhaitez que le lien apparaisse, puis cliquez sur le bouton **Insérer un jeton**.

   ![](assets/six-2.png)

1. Sélectionnez le jeton de **`{{system.forwardToFriendLink}}`**.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Ce jeton est l’URL de la version web de l’e-mail avec une zone « Transférer à un ami ».

1. Écrivez ce que vous souhaitez que le texte affiché du lien soit (par exemple, « Transférer à un ami »).

   ![](assets/seven-1.png)

1. Coupez le jeton **`{{system.forwardToFriendLink}}`** en utilisant Ctrl+X (Windows) ou Cmd+X (Mac). Sélectionnez « Transférer à un ami » et cliquez sur le bouton **Insérer/Modifier le lien**.

   ![](assets/eight-1.png)

1. Collez le jeton **`{{system.forwardToFriendLink}}`** dans la zone **URL** en utilisant Ctrl/Cmd+V, puis cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/nine.png)

1. Enregistrez la modification et prévisualisez votre nouveau lien.

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Les nouvelles personnes qui sont ajoutées par le biais d’un e-mail « Transférer à un ami » sont par défaut désabonnées des e-mails marketing.

## Afficher l&#39;activité de transfert {#view-forwarding-activity}

Vous pouvez voir qui a transféré et reçu les e-mails dans le journal d’activité de la personne.

1. Accédez à la **[!UICONTROL Base de données]**.

   ![](assets/db.png)

1. Double-cliquez sur la personne pour laquelle vous souhaitez afficher l’activité.

   ![](assets/fourteen.png)

1. Accédez à l’onglet **[!UICONTROL Journal d’activité]**. Double-cliquez sur **[!UICONTROL E-mail transféré à un ami]** ou **[!UICONTROL E-mail transféré à un ami]** pour afficher les détails.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >Pour l’e-mail Transférer à un ami reçu, l’ID de personne est la personne qui a transféré l’e-mail.
   >
   >Pour l’e-mail Transféré à un ami, l’ID de personne correspond à la personne qui a reçu l’e-mail.

   ![](assets/sixteen.png)

1. Pour afficher une personne par ID, copiez et collez l’**ID de personne** à la fin de l’URL (le début de l’URL dépendra de votre instance Marketo) :

   `...marketo.com/Database/loadPersonDetail?personId=`

   >[!NOTE]
   >
   >Nous rendrons le **[!UICONTROL ID de personne]** cliquable et créerons un lien direct vers la personne dans un correctif à venir.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Si l&#39;ami recevant le transfert est une personne inconnue, une nouvelle personne est créée avec « Transférer à un ami » marqué comme **Source de la personne**.
   >Si l’e-mail est une ressource locale d’un programme, le programme est marqué comme le **Programme d’acquisition** de la personne.

## Déclencheur ou filtre utilisant l’activité de transfert {#trigger-or-filter-using-forwarding-activity}

Vous pouvez utiliser six déclencheurs/filtres pour déclencher des actions de flux ou filtrer des personnes en fonction de l’activité « Transférer à un ami » envoyée et reçue.

Dans la liste dynamique d’une campagne intelligente, si vous recherchez « forward », vous trouverez les déclencheurs et filtres disponibles.

![](assets/nineteen.png)

## Tester vers l&#39;avant pour un ami {#test-forward-to-friend}

Pour tester « Transférer à un ami », envoyez-vous un e-mail contenant le lien de transfert. Veillez à l’envoyer par le biais de l’étape de flux **Envoyer un e-mail**, *pas* par le biais de **Envoyer un e-mail de test**.
