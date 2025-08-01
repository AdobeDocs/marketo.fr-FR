---
unique-page-id: 2360253
description: Modifiez le message « Afficher en tant que page web » - Documents Marketo - Documentation du produit.
title: Modifier le message « Afficher en tant que page web »
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Modifier le message « Afficher en tant que page web » {#edit-the-view-as-web-page-message}

Si vous devez modifier le texte « [Afficher en tant que page web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) », procédez comme suit.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Modifier le message « Afficher en tant que page web » {#edit-the-view-as-web-page-message-1}

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Les variables suivantes sont critiques. Ne les supprimez pas !
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La deuxième partie `##MKT_TOK##` le cookie [!UICONTROL munchkin] de cette personne. Cela permet de s’assurer qu’ils sont correctement cookies lorsqu’ils cliquent sur le lien.

1. Modifiez les versions **[!UICONTROL Afficher en tant que page Web HTML]** et **[!UICONTROL Afficher en tant que texte de page Web]** selon vos besoins, puis cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Veillez à éviter :
>
>* Ajout d’URL supplémentaires à l’une des zones HTML
>* Mise d’HTML dans la version texte

Voilà, c&#39;est fait. Envoyez des e-mails de test pour garantir la mise en forme.

## Texte « Afficher en tant que page web » par défaut {#default-view-as-web-page-text}

Si vous devez revenir au système par défaut « [!UICONTROL Afficher en tant que page web] », copiez/collez les éléments suivants :

**[!UICONTROL Afficher en tant qu&#39;HTML de page Web]** :

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL Afficher en tant que texte de page web]** :

Pour afficher cet e-mail en tant que page web, accédez à l’adresse suivante :
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`

C&#39;est ça !
