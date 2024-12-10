---
unique-page-id: 1900581
description: Transférer vers un lien d’ami dans les emails - Documents Marketo - Documentation du produit
title: Transférer vers un lien d’ami dans les courriers électroniques
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
feature: Email Editor
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Transférer vers un lien d’ami dans les courriers électroniques {#forward-to-a-friend-link-in-emails}

L&#39;ajout du lien &quot;Transférer à l&#39;ami&quot; à vos emails permet de suivre les personnes qui ont reçu un email transféré via ce lien, et les ajoute automatiquement en tant que nouvelle personne si elle ne se trouve pas déjà dans la base de données.

Par exemple, supposons que Keith utilise le lien &quot;Transférer à l’ami&quot; pour transférer l’email à une personne inconnue, Mark. Mark est automatiquement ajouté en tant que nouvelle personne, se voit attribuer son propre cookie et toute activité email et web qui lui est associée. Cependant, si Keith utilise le bouton de transfert dans son client de messagerie, Mark reçoit un cookie incorrect en tant que Keith et son activité est consignée comme étant celle de Keith.

## Ajout d’un lien à un modèle de courrier électronique {#add-the-link-to-an-email-template}

1. Accédez à **Design Studio**.

   ![](assets/one-8.png)

1. Recherchez et sélectionnez le modèle d&#39;email auquel vous souhaitez ajouter le lien. Cliquez sur **Modifier le brouillon**.

   ![](assets/two-7.png)

1. Collez le code d’HTML suivant où vous souhaitez que le lien &quot;Transférer vers l’ami&quot; s’affiche (si vous avez besoin d’aide sur cette partie, veuillez contacter votre développeur web) :

   `<a href="{{system.forwardToFriendLink}}">Forward to Friend</a>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Vous pouvez ajouter un style au lien pour qu’il ait l’air plus agréable. Par exemple :
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Il est déconseillé d&#39;utiliser le style **position:relative** dans votre modèle de courrier électronique. Il peut créer des problèmes avec la position et l&#39;affichage de la boîte &quot;Transférer à l&#39;ami&quot;.

1. Cliquez sur **Aperçu de la version préliminaire** pour vous assurer que le modèle ressemble à ce que vous souhaitez.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >N&#39;oubliez pas de valider le modèle de brouillon pour appliquer les modifications.

   Désormais, tous les emails qui utilisent ce modèle auront le lien &quot;Transférer à l’ami&quot;. Lorsque le destinataire de l&#39;email clique dessus, il est redirigé vers une version web de l&#39;email avec la boîte &quot;Transférer à un ami&quot; :

   ![](assets/f2afbox.png)

## Ajout d’un lien à un courrier électronique individuel {#add-the-link-to-an-individual-email}

Vous pouvez également ajouter le lien &quot;Transférer à l&#39;ami&quot; directement dans un email.

1. Ouvrez l&#39;email dans lequel vous souhaitez inclure le lien et double-cliquez dans la zone modifiable.

   ![](assets/five-4.png)

1. Placez le curseur à l’endroit où vous souhaitez que le lien s’affiche et cliquez sur le bouton **Insérer un jeton** .

   ![](assets/six-2.png)

1. Sélectionnez le jeton **`{{system.forwardToFriendLink}}`**.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Ce jeton est l&#39;URL de la version web de l&#39;email avec une boîte &quot;Transférer à l&#39;ami&quot;.

1. Écrivez ce que vous souhaitez que le texte affiché du lien soit (par exemple, &quot;Transférer à un ami&quot;).

   ![](assets/seven-1.png)

1. Coupez le jeton **`{{system.forwardToFriendLink}}`** à l’aide de Ctrl+X (Windows) ou Cmd+X (Mac). Sélectionnez &quot;Transférer à un ami&quot; et cliquez sur le bouton **Insérer/Modifier le lien**.

   ![](assets/eight-1.png)

1. Collez le jeton **`{{system.forwardToFriendLink}}`** dans la zone **URL** à l’aide de Ctrl/Cmd+V, puis cliquez sur **Insérer**.

   ![](assets/nine.png)

1. Enregistrez la modification et prévisualisez le nouveau lien !

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Les nouvelles personnes qui sont ajoutées par la réception d’un email &quot;Transférer à un ami&quot; sont par défaut désabonnées aux emails marketing.

## Afficher l’activité de transfert {#view-forwarding-activity}

Vous pouvez voir qui a transféré et reçu les emails dans le journal d’activité de la personne.

1. Accédez au **`Database`**.

   ![](assets/db.png)

1. Double-cliquez sur la personne pour laquelle vous souhaitez afficher l’activité.

   ![](assets/fourteen.png)

1. Accédez à l’onglet **Journal d’activité** . Double-cliquez sur **Reçu pour être envoyé à l’ami par courrier électronique** ou **Envoyé vers l’ami par courrier électronique** pour afficher les détails.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >Pour Reçu comme courrier électronique d’envoi à un ami, l’ID de personne est la personne qui a transféré l’adresse électronique.
   >
   >Pour Envoyer un courrier électronique à un ami, l’ID de personne est la personne qui a reçu le courrier électronique.

   ![](assets/sixteen.png)

1. Pour afficher une personne par identifiant, copiez et collez l’ **ID de personne** à la fin de l’URL (le début de l’URL dépendra de votre instance Marketo) :

   `...marketo.com/Database/loadPersonDetail?personId=`

   >[!NOTE]
   >
   >Nous rendrons le **ID de personne** cliquable et nous le lierons directement à la personne dans un correctif à venir.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Si l’ami recevant le transfert est une personne inconnue, une nouvelle personne est créée avec &quot;Transférer à l’ami&quot; marqué comme **Source** de la personne.
   >Si le courrier électronique est une ressource locale d’un programme, le programme est marqué comme le **Programme d’acquisition** de la personne.

## Déclenchement ou filtrage à l’aide de l’activité de transfert {#trigger-or-filter-using-forwarding-activity}

Il existe six déclencheurs/filtres que vous pouvez utiliser pour déclencher des actions de flux ou filtrer les personnes selon l’activité &quot;Transférer à l’ami&quot; envoyée et reçue.

Dans la liste dynamique d’une campagne dynamique, si vous recherchez &quot;forward&quot;, vous trouverez les déclencheurs et filtres disponibles.

![](assets/nineteen.png)

## Tester vers l’ami {#test-forward-to-friend}

Pour tester &quot;Transférer à l’ami&quot;, envoyez-vous un email avec le lien de transfert. Assurez-vous de l&#39;envoyer par le biais de l&#39;étape de flux **Envoyer le courrier électronique**, *et non* via **Envoyer le courrier électronique de test**.
