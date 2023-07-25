---
unique-page-id: 2360251
description: Modification du message de désabonnement - Documents Marketo - Documentation du produit
title: Modification du message de désabonnement
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Modification du message de désabonnement {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Lorsque vous envoyez des emails marketing (non[opérationnel](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), le texte de désabonnement et les liens sont ajoutés au bas de la page. Vous pouvez modifier les valeurs par défaut. Voici comment.

## Où effectuer la modification {#where-to-make-the-edit}

1. Accédez au **[!UICONTROL Administration]** .

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Les variables suivantes sont critiques. Ne les supprimez pas !
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Modifiez la variable **[!UICONTROL Désabonner le HTML]** et **[!UICONTROL Désabonner le texte]** versions à votre convenance et cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Voilà. _Assurez-vous de tester !_ Vous ne souhaitez pas que vos emails marketing aient rompu les liens de désabonnement.

>[!TIP]
>
>Vous pouvez personnaliser la position du HTML de désabonnement dans votre email à l’aide de l’option [jetons](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texte de désabonnement par défaut {#default-unsubscribe-text}

Si vous devez revenir au désabonnement du système par défaut, copiez/collez les éléments suivants :

[!UICONTROL Désabonner le HTML]:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` [!UICONTROL Désabonner le texte]:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Modifier le message &quot;Afficher comme page Web&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
