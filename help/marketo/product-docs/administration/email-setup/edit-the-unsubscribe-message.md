---
unique-page-id: 2360251
description: Modifier le message de désabonnement - Documents Marketo - Documentation du produit
title: Modifier le message de désabonnement
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 7%

---

# Modifier le message de désabonnement {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Lorsque vous envoyez des e-mails marketing (non [opérationnels](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), le texte de désabonnement et les liens sont ajoutés en bas. Vous pouvez modifier les valeurs par défaut. Voici comment faire.

## Où effectuer la modification {#where-to-make-the-edit}

1. Accédez à la section **[!UICONTROL Admin]**.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Les variables suivantes sont critiques. Ne les supprimez pas !
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Modifiez les versions **[!UICONTROL Se désabonner d’HTML]** et **[!UICONTROL Se désabonner du texte]** selon vos besoins, puis cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Voilà, c&#39;est fait. _Veillez à effectuer le test._ Vous ne souhaitez pas que vos e-mails marketing aient des liens de désabonnement rompus.

>[!TIP]
>
>Vous pouvez personnaliser la position de l’HTML de désabonnement dans votre e-mail à l’aide de [jetons](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texte de désabonnement par défaut {#default-unsubscribe-text}

Si vous devez revenir au désabonnement système par défaut, copiez/collez les éléments suivants :

[!UICONTROL Désabonnement d’HTML] :
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>` [!UICONTROL Texte de désabonnement] :
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[Modifier le message Afficher en tant que page web »](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
