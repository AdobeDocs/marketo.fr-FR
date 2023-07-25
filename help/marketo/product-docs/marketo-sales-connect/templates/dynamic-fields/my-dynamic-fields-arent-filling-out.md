---
unique-page-id: 14352602
description: Mes champs dynamiques ne sont pas remplis - Documents Marketo - Documentation du produit
title: Mes champs dynamiques ne se remplissent pas
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---

# Mes champs dynamiques ne se remplissent pas {#my-dynamic-fields-arent-filling-out}

Les champs dynamiques ne fonctionnent que lorsque vous utilisez un modèle. Les emails ponctuels que vous écrivez ne seront pas remplis.

## Eléments à vérifier {#what-to-check}

Il existe trois types de champs dynamiques dans Sales Connect : De base, personnalisés et Salesforce. De base et personnalisés cherchent tous deux à extraire des informations de [application web](https://toutapp.com/login). Si les informations n&#39;existent pas dans l&#39;application web, les champs seront vides. Les champs Salesforce extraient des informations de [Salesforce.com](https://salesforce.com).

**Dépannage des champs Salesforce**

Champs Salesforce : Par exemple : `{{sfdc_account_name}}`

* Assurez-vous qu’il est correctement connecté à Sales Connect. Accédez au [Paramètres](https://toutapp.com/login) page et clic **Gérer** en regard de votre CRM.

**Dépannage des champs de base et personnalisés**

Tout Basic Fields : Par exemple : `{{company}}`

Tout champ personnalisé : Par exemple : `{{custom_field_favorite_movie}}`

* Le champ correspondant doit être enregistré pour votre contact dans le [Page Personnes](https://toutapp.com/next#relationships) pour référencer notre champ dynamique. Par exemple, si vous envoyez un courrier électronique à Mary et que vous utilisez la variable `{{company}}` , mais son enregistrement de contact ne donne pas de liste d’entreprises, nous ne pourrons pas le remplir.

## Pourquoi Mon Email A-T-Il Été Envoyé Sans Renseigner Tous Les Champs Dynamiques ? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect empêchera l’envoi de vos emails si nous ne pouvons pas renseigner tous vos champs dynamiques dans le message électronique. **Cependant**, il existe quelques exceptions à cette règle. Certains champs sont renvoyés vides ou renseignent automatiquement une valeur si nous pouvons en trouver une. Ces champs et leur réaction s’ils ne peuvent pas les remplir sont répertoriés ci-dessous.

`{{first_name}}` = BLANC

`{{last_name}}` =BLANC

`{{title}}` = BLANC

`{{company}}` = &quot;votre société&quot;

`{{friendly_company}}` = &quot;votre société&quot;

>[!NOTE]
>
>Le `{{first_name}}` pour rechercher des informations dans Sales Connect et Salesforce. Tous les autres champs de cette liste ne recherchent que dans Sales Connect pour renseigner ce champ.
