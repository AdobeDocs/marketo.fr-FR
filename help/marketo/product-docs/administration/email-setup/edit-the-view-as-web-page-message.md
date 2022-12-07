---
unique-page-id: 2360253
description: Modifier le message "Afficher comme page web" - Documents Marketo - Documentation du produit
title: Modifier le message "Afficher comme page Web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 8%

---

# Modifier le message &quot;Afficher comme page Web&quot; {#edit-the-view-as-web-page-message}

Si vous devez modifier le[Afficher en tant que page web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot; text, voilà comment.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Modifier le message &quot;Afficher comme page Web&quot; {#edit-the-view-as-web-page-message-1}

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Cliquez sur **Email**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Les variables suivantes sont critiques. Ne les supprimez pas !
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La deuxième partie `##MKT_TOK##` est le cookie munchkin de cette personne. Il s’assure qu’ils reçoivent un cookie approprié lorsqu’ils cliquent sur le lien.

1. Modifiez la variable **Afficher comme HTML de page web** et **Afficher comme texte de page Web** versions à votre convenance et cliquez sur **Enregistrer les modifications**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Veillez à éviter :
>
>* Ajout d’URL supplémentaires à l’une des zones de HTML
>* Placement du HTML dans la version texte


Voilà. Envoyez des emails de test pour garantir la mise en forme.

## Texte &quot;Afficher comme page Web&quot; par défaut {#default-view-as-web-page-text}

Si vous devez revenir au système par défaut &quot;Afficher comme page web&quot;, copiez/collez les éléments suivants :

**Afficher sur une Page Internet HTML :**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**Afficher sur une Page Internet Texte:**

Pour afficher cet email en tant que page web, accédez à l&#39;adresse suivante :
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

C&#39;est tout !
