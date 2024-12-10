---
unique-page-id: 2360251
description: Modification du message de désabonnement - Documents Marketo - Documentation du produit
title: Modification du message de désabonnement
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Modification du message de désabonnement {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Lorsque vous envoyez des emails marketing (non-[opérationnel](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), le texte de désabonnement et les liens sont ajoutés en bas de la page. Vous pouvez modifier les valeurs par défaut. Voici comment.

## Où modifier {#where-to-make-the-edit}

1. Accédez à la section **[!UICONTROL Admin]** .

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Les variables suivantes sont critiques. Ne les supprimez pas !
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Modifiez les versions **[!UICONTROL Désabonner l’HTML]** et **[!UICONTROL Désabonner le texte]** à votre convenance et cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Voilà. _Assurez-vous de tester !_ Vous ne souhaitez pas que vos emails marketing aient des liens de désabonnement rompus.

>[!TIP]
>
>Vous pouvez personnaliser la position de l’HTML de désabonnement dans votre email à l’aide de [jetons](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texte de désabonnement par défaut {#default-unsubscribe-text}

Si vous devez revenir au désabonnement du système par défaut, copiez/collez les éléments suivants :

[!UICONTROL Désabonner l’HTML] :
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>` [!UICONTROL Désabonner le texte] :
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[Modifier le message &quot;Afficher comme page web&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
