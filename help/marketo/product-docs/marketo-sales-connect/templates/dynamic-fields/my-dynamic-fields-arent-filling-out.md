---
unique-page-id: 14352602
description: Mes champs dynamiques ne sont pas remplis - Documents marketing - Documentation du produit
title: Mes champs dynamiques ne sont pas remplis
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# Mes champs dynamiques ne sont pas remplis {#my-dynamic-fields-arent-filling-out}

Les champs dynamiques ne fonctionnent que lorsque vous utilisez un modèle. Les e-mails ponctuels que vous écrivez ne les rempliront pas.

## Que vérifier {#what-to-check}

Il existe trois types de champs dynamiques dans Sales Connect : Simple, Personnalisé et Salesforce. Basic et Custom cherchent tous deux à extraire des informations de l&#39;[application Web](https://toutapp.com/login). Si les informations n’existent pas dans l’application Web, les champs sont vides. Les champs Salesforce extraient les informations de [Salesforce.com](https://salesforce.com).

**Dépannage des champs Salesforce**

Champs Salesforce : par ex. `{{sfdc_account_name}}`

* Assurez-vous qu&#39;il est correctement connecté avec Sales Connect. Accédez à la page [Paramètres](https://toutapp.com/login) et cliquez sur **Gérer** en regard de votre gestion de la relation client.

**Dépannage des champs de base et personnalisés**

Tout champs de base : par ex. `{{company}}`

Tout champ personnalisé : par ex. `{{custom_field_favorite_movie}}`

* Le champ correspondant doit être enregistré pour votre contact dans la [page Personnes](https://toutapp.com/next#relationships) pour que le champ dynamique puisse être référencé. Par exemple, si vous envoyez un courrier électronique à Mary et que vous utilisez le champ `{{company}}`, mais que son enregistrement de contact ne liste pas de société, nous ne pourrons pas le remplir.

## Pourquoi Mon Courrier Électronique A-T-Il Été Envoyé Sans Remplir Tous Les Champs Dynamiques ? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect empêchera l&#39;envoi de vos courriers électroniques si nous ne pouvons pas renseigner tous vos champs dynamiques dans le courrier électronique. **Cependant**, cette règle comporte quelques exceptions. Certains champs sont renvoyés vides ou renseignent automatiquement une valeur si nous en trouvons une. Ces champs et comment ils réagiront s’ils ne peuvent pas remplir le champ sont répertoriés ci-dessous.

`{{first_name}}` = BLANC

`{{last_name}}` =VIERGE

`{{title}}` = BLANC

`{{company}}` = &quot;votre société&quot;

`{{friendly_company}}` = &quot;votre société&quot;

>[!NOTE]
>
>Le champ `{{first_name}}` recherche les informations dans Sales Connect et Salesforce. Tous les autres champs de cette liste sont uniquement à la recherche dans Sales Connect pour renseigner le champ.
