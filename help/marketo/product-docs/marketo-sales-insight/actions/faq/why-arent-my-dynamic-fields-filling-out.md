---
description: Pourquoi mes champs dynamiques ne se remplissent-ils pas ? - Documents Marketo - Documentation du produit
title: Pourquoi mes champs dynamiques ne se remplissent-ils pas ?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Pourquoi mes champs dynamiques ne se remplissent-ils pas ? {#why-arent-my-dynamic-fields-filling-out}

Les champs dynamiques ne fonctionnent que lorsque vous utilisez un modèle. Les emails ponctuels que vous écrivez ne seront pas remplis.

## Eléments à vérifier {#what-to-check}

Il existe trois types de champs dynamiques dans les actions d’aperçu des ventes : de base, personnalisé et Salesforce. De base et personnalisés cherchent tous deux à extraire des informations de l&#39;[application web](https://toutapp.com/login){target="_blank"}. Si les informations n&#39;existent pas dans l&#39;application web, les champs seront vides. Les champs Salesforce extraient des informations de [Salesforce.com](https://salesforce.com){target="_blank"}.

**Dépannage des champs Salesforce**

Champs Salesforce : par exemple `{{sfdc_account_name}}`

* Assurez-vous qu’il est correctement connecté aux actions d’aperçu des ventes. Accédez à la page [Paramètres] (https://toutapp.com/login{target="_blank"} et cliquez sur **Gérer** en regard de votre CRM.

**Dépannage des champs de base et personnalisés**

Actions Marketo Sales Insight Champs de base : par exemple, `{{company}}`

Actions Marketo Sales Insight Champs personnalisés : par exemple, `{{custom_field_favorite_movie}}`

* Le champ correspondant doit être enregistré pour votre contact dans la [page Personnes](https://toutapp.com/next#relationships){target="_blank"} pour que notre champ dynamique soit référencé. Par exemple, si vous envoyez un courrier électronique à Mary et que vous utilisez le champ `{{company}}`, mais que son enregistrement de contact ne répertorie pas d’entreprise, nous ne pourrons pas remplir ce champ.

## Pourquoi Mon Email A-T-Il Été Envoyé Sans Renseigner Tous Les Champs Dynamiques ? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Les actions d’aperçu des ventes empêcheront l’envoi de vos emails si nous ne pouvons pas renseigner tous vos champs dynamiques dans le message électronique. **Cependant**, cette règle comporte quelques exceptions. Certains champs sont renvoyés vides ou renseignent automatiquement une valeur si nous pouvons en trouver une. Ces champs et leur réaction s’ils ne peuvent pas les remplir sont répertoriés ci-dessous.

`{{first_name}}` = BLANC

`{{last_name}}` =BLANC

`{{title}}` = BLANC

`{{company}}` = &quot;votre société&quot;

`{{friendly_company}}` = &quot;votre société&quot;

>[!NOTE]
>
>Le champ `{{first_name}}` recherche des actions Sales Insight et Salesforce pour tenter d’extraire des informations. Tous les autres champs de cette liste ne sont affichés que dans les actions de statistiques sur les ventes pour renseigner le champ.
