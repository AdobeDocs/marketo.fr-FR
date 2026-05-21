---
unique-page-id: 2360251
description: Modifiez le texte de désabonnement par défaut et les liens ajoutés aux e-mails marketing dans les e-mails d’administration.
title: Modifier le message de désabonnement
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
TQID: https://experienceleague.adobe.com/2wAcUvsELVvNhk0HpdNdkWJLopFn3IC4X-lUSQlCs5Q
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 140
ht-degree: 9%

---

# Modifier le message de désabonnement {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Autorisations d’administration requises**

Lorsque vous envoyez des e-mails marketing (non [opérationnels](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), le texte de désabonnement et les liens sont ajoutés en bas. Vous pouvez modifier les valeurs par défaut.

## Où effectuer la modification {#where-to-make-the-edit}

1. Accédez à la section **[!UICONTROL Admin]**.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Cliquez sur **[!UICONTROL E-mail]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Les variables suivantes sont critiques. Ne les supprimez pas !
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Modifiez les versions **[!UICONTROL Se désabonner d’HTML]** et **[!UICONTROL Se désabonner du texte]** selon vos besoins, puis cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

>[!TIP]
>
>* N’oubliez pas de tester. Vous ne souhaitez pas que vos e-mails marketing aient des liens de désabonnement rompus.
>
>* Vous pouvez personnaliser la position de l’HTML de désabonnement dans votre e-mail à l’aide de [jetons](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texte de désabonnement par défaut {#default-unsubscribe-text}

Si vous devez revenir au message de désabonnement système par défaut, copiez/collez les éléments suivants :

[!UICONTROL Désabonnement d’HTML] :
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>`
<br>
[!UICONTROL Texte de désabonnement] :
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[Modifier le message Afficher en tant que page web »](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
