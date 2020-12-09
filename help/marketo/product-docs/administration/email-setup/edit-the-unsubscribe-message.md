---
unique-page-id: 2360251
description: Modifier le message de désabonnement - Documents marketing - Documentation du produit
title: Modifier le message de désabonnement
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---


# Modifier le message de désabonnement {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Lorsque vous envoyez des courriels marketing (non [opérationnels](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), le texte de désabonnement et les liens sont ajoutés au bas de la page. Vous pouvez modifier les valeurs par défaut. Voici comment.

## Modifier le message de désabonnement {#edit-the-unsubscribe-message-1}

1. Sous **Admin**, cliquez sur **Courriel**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >
   >Les variables suivantes sont essentielles. Ne les supprimez pas !
   >
   >    
   >    
   >    * **%mkt_opt_out_prefix%**
   >    * **mkt_unsubscription=1&amp;mkt_tok=##MKT_TOK##**


1. Modifiez les versions HTML **** Désabonner et Texte **** Désabonner à votre convenance, puis cliquez sur **Enregistrer les modifications**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Voilà. **Assurez-vous de tester !** Vous ne souhaitez pas que vos courriels marketing aient rompu les liens de désabonnement.

>[!TIP]
>
>Vous pouvez personnaliser la position du code HTML de désabonnement dans votre courrier électronique à l’aide de [jetons](../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Texte de désabonnement par défaut {#default-unsubscribe-text}

Si vous devez revenir au système par défaut de désabonnement, copiez/collez les éléments suivants :

Désabonner HTML :
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Désabonner le texte :
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>* [Modifier le message &quot;Vue en tant que page Web&quot;](edit-the-view-as-web-page-message.md)

>



