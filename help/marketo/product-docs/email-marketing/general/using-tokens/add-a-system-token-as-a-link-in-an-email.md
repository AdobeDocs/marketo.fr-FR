---
unique-page-id: 1900573
description: Ajout d’un jeton système en tant que lien dans un e-mail - Documents Marketo - Documentation du produit
title: Ajouter un jeton système en tant que lien dans un e-mail
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Ajouter un jeton système en tant que lien dans un e-mail {#add-a-system-token-as-a-link-in-an-email}

Vous pouvez utiliser ces jetons système pour personnaliser la position des liens spéciaux dans vos e-mails.

Les jetons suivants peuvent être utilisés comme liens dans un e-mail ou un modèle d’e-mail :

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>Il n’est **possible de cliquer sur ces jetons** sauf dans un lien d’ancrage. En outre, ils ne peuvent **pas** être incorporés dans un jeton Mon jeton.

Voici comment les ajouter à un e-mail :

1. Recherchez et sélectionnez votre e-mail, puis cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/one-1.png)

1. Double-cliquez dans une zone modifiable.

   ![](assets/two-1.png)

1. Mettez en surbrillance le texte à convertir en lien qui contiendra le jeton et cliquez sur le bouton **[!UICONTROL Insérer/Modifier le lien]**.

   ![](assets/three-1.png)

1. Saisissez le jeton dans URL du lien et cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >Copiez/collez le jeton de votre choix : **`{{system.forwardToFriendLink}}`**, **`{{system.unsubscribeLink}}`** ou **`{{system.viewAsWebpageLink}}`**

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>Si vous utilisez cette approche pour ajouter le jeton système « viewAsWebpageLink », vous ne pouvez **pas** le remplacer à l’aide de jetons. Utilisez plutôt l’approche [Ajouter un lien Afficher en tant que page web à un e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) qui permet de remplacer « viewAsWebPageLink » à l’aide de jetons.

>[!NOTE]
>
>N’oubliez pas de [approuver l’e-mail](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) lorsque vous avez terminé.

Bien joué ! Vous savez maintenant comment ajouter un jeton système sous la forme d’un lien dans un e-mail.
