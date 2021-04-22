---
unique-page-id: 2360253
description: Modifier le message "Vue en tant que page Web" - Marketo Docs - Documentation du produit
title: Modifier le message "Vue en tant que page Web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 5%

---

# Modifier le message &quot;Vue en tant que page Web&quot; {#edit-the-view-as-web-page-message}

Si vous devez modifier le texte &quot;[Vue as a Webpage](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;, voici comment procéder.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Modifier le message &quot;Vue en tant que page Web&quot; {#edit-the-view-as-web-page-message-1}

1. Sous **Admin**, cliquez sur **Courriel**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >Les variables suivantes sont essentielles. Ne les supprimez pas !
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La deuxième partie `##MKT_TOK##` est le cookie commun de cette personne. Il s’assure qu’ils reçoivent un cookie approprié lorsqu’ils cliquent sur le lien.

1. Modifiez la **Vue en tant que page Web HTML** et **Vue en tant que texte de page Web** versions et cliquez sur **Enregistrer les modifications**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Veillez à éviter :
>
>* Ajoute d’URL supplémentaires dans l’une ou l’autre des zones HTML
>* Placement de code HTML dans la version de texte


Voilà. Envoyer des courriers électroniques de test pour assurer la mise en forme.

## Texte par défaut &quot;Vue en tant que page Web&quot; {#default-view-as-web-page-text}

Si vous devez revenir au système par défaut &quot;Vue en tant que page Web&quot;, copiez/collez les éléments suivants :

**Afficher sur une Page Internet HTML :**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**Afficher sur une Page Internet Texte:**

Pour vue de ce courrier électronique en tant que page Web, accédez à l’adresse suivante :
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` Boom ! Vous avez terminé.
