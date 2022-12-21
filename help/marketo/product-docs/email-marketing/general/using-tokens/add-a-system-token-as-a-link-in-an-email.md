---
unique-page-id: 1900573
description: Ajout d’un jeton système en tant que lien dans un courrier électronique - Documents Marketo - Documentation du produit
title: Ajout d’un jeton système en tant que lien dans un courrier électronique
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
source-git-commit: 65caed388ac33fc9f3142102343fe43ebc186e6e
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Ajout d’un jeton système en tant que lien dans un courrier électronique {#add-a-system-token-as-a-link-in-an-email}

Vous pouvez utiliser ces jetons système pour personnaliser la position des liens spéciaux dans vos emails.

Les jetons suivants peuvent être utilisés comme liens dans un email ou un modèle de courrier électronique :

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Ces jetons seront **not** peut être cliqué, sauf dans un lien d’ancrage. Ils peuvent également **not** être incorporé dans un jeton My Token.

Pour les ajouter à un email, procédez comme suit :

1. Recherchez et sélectionnez votre email, puis cliquez sur **Modifier le brouillon**.

   ![](assets/one-1.png)

1. Double-cliquez dans une zone modifiable.

   ![](assets/two-1.png)

1. Mettez en surbrillance le texte que vous souhaitez convertir en lien qui contiendra le jeton et cliquez sur le bouton **Insérer/Modifier un lien** bouton .

   ![](assets/three-1.png)

1. Saisissez le jeton dans l’URL du lien, puis cliquez sur **Insérer**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Copiez/collez le jeton de votre choix : **`{{system.forwardToFriendLink}}`** ou **`{{system.unsubscribeLink}}`** ou **`{{system.viewAsWebpageLink}}`**

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Si vous utilisez cette approche pour ajouter le jeton système &quot;viewAsWebpageLink&quot;, vous pouvez **not** le remplacer à l’aide de jetons. À la place, utilisez [Ajout d’une vue comme lien de page web à un courrier électronique](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) qui permet de remplacer &quot;viewAsWebPageLink&quot; à l’aide de jetons.

>[!NOTE]
>
>N&#39;oublie pas de [valider votre email](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) une fois terminé.

C&#39;est joli ! Vous savez maintenant comment ajouter un jeton système en tant que lien dans un email.
