---
unique-page-id: 2953243
description: Types de notification - Documents marketing - Documentation du produit
title: Types de notification
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Types de notification {#notification-types}

Il existe plusieurs types de notification.

## Échec de Campaign  {#campaign-failure}

Les échecs Campaign vous signalent des erreurs dans vos campagnes actives.

## CRM Sync {#crm-sync}

Les notifications de synchronisation CRM vous avertissent des problèmes critiques rencontrés avec la synchronisation CRM, tels que des autorisations incorrectes ou la synchronisation en cours d’arrêt.

**Microsoft Dynamics**

Les notifications Dynamics sont envoyées une fois toutes les 24 heures et contiennent des pistes qui n&#39;ont pas été synchronisées au cours de cette période. Les causes habituelles de l’échec sont les pistes de duplicata (comme ci-dessus) ou les erreurs de non-correspondance de longueur de champ.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Si vous utilisez Salesforce, les notifications d’erreur de synchronisation ressemblent à celles présentées ci-dessous. Les erreurs types comprennent les informations d’identification expirées et les limites d’API dépassées.

![](assets/salesforcesyncerror.png)

Engagement

Lorsque les pistes s&#39;épuisent dans un flux, nous envoyons une notification.  La notification comprend le nombre de pistes épuisées et d&#39;autres informations.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Si vous essayez d’envoyer des pistes à Facebook sans accepter les conditions d’utilisation, ou si vous essayez d’envoyer des pistes à Facebook après avoir supprimé l’application Marketo.

Nettoyage Campaign du déclencheur d&#39;inactivité

Désactivez les campagnes dynamiques déclenchées qui n’obtiennent plus d’activité. En savoir plus sur le nettoyage [](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)automatique de la campagne de déclenchement.

LinkedIn

Lorsque Marketo ne parvient pas à créer une nouvelle audience, à se connecter ou à envoyer des courriers électroniques à LinkedIn après trois tentatives.

![](assets/linkedin.png)

Services Web

Vous serez averti lorsque vous atteindrez votre quota quotidien. Le quota est réinitialisé chaque nuit à minuit, heure du centre.

>[!NOTE]
>
>Certains des codes d’erreur que vous pouvez recevoir sont décrits dans notre documentation [](http://developers.marketo.com/rest-api/error-codes/#response_level_error_codes)destinée aux développeurs.

