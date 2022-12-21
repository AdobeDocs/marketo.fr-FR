---
description: Pourquoi mes champs dynamiques ne se remplissent-ils pas - Documents Marketo - Documentation du produit
title: Pourquoi mes champs dynamiques ne se remplissent-ils pas ?
hide: true
hidefromtoc: true
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: f77a076c243c25f3bff98a82751f51c464712795
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# Pourquoi mes champs dynamiques ne se remplissent-ils pas ? {#why-arent-my-dynamic-fields-filling-out}

Les champs dynamiques ne fonctionnent que lorsque vous utilisez un modèle. Les emails ponctuels que vous écrivez ne seront pas remplis.

## Eléments à vérifier {#what-to-check}

Il existe trois types de champs dynamiques dans les actions d’aperçu des ventes : De base, personnalisés et Salesforce. De base et personnalisés cherchent tous deux à extraire des informations de [application web](https://toutapp.com/login). Si les informations n&#39;existent pas dans l&#39;application web, les champs seront vides. Les champs Salesforce extraient des informations de [Salesforce.com](https://salesforce.com).

**Dépannage des champs Salesforce**

Champs Salesforce : Par exemple : `{{sfdc_account_name}}`

* Assurez-vous qu’il est correctement connecté aux actions d’aperçu des ventes. Accédez au [Paramètres](https://toutapp.com/login) page et clic **Gérer** en regard de votre CRM.

**Dépannage des champs de base et personnalisés**

Tout Basic Fields : Par exemple : `{{company}}`

Tout champ personnalisé : Par exemple : `{{custom_field_favorite_movie}}`

* Le champ correspondant doit être enregistré pour votre contact dans le [Page Personnes](https://toutapp.com/next#relationships) pour référencer notre champ dynamique. Par exemple, si vous envoyez un courrier électronique à Mary et que vous utilisez la variable `{{company}}` , mais son enregistrement de contact ne donne pas de liste d’entreprises, nous ne pourrons pas le remplir.

## Pourquoi Mon Email A-T-Il Été Envoyé Sans Renseigner Tous Les Champs Dynamiques ? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Les actions d’aperçu des ventes empêcheront l’envoi de vos emails si nous ne pouvons pas renseigner tous vos champs dynamiques dans le message électronique. **Cependant**, il existe quelques exceptions à cette règle. Certains champs sont renvoyés vides ou renseignent automatiquement une valeur si nous pouvons en trouver une. Ces champs et leur réaction s’ils ne peuvent pas les remplir sont répertoriés ci-dessous.

`{{first_name}}` = BLANC

`{{last_name}}` =BLANC

`{{title}}` = BLANC

`{{company}}` = &quot;votre société&quot;

`{{friendly_company}}` = &quot;votre société&quot;

>[!NOTE]
>
>Le `{{first_name}}` pour rechercher des informations dans les actions Sales Insight et Salesforce. Tous les autres champs de cette liste ne sont affichés que dans les actions de statistiques sur les ventes pour renseigner le champ.
