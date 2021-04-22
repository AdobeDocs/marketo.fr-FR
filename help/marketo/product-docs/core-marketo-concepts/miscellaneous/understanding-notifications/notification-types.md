---
unique-page-id: 2953243
description: Types de notification - Documents Marketo - Documentation du produit
title: Types de notification
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 5%

---

# Types de notification {#notification-types}

Il existe plusieurs types de notification.

## Erreur de la campagne {#campaign-failure}

Les échecs Campaign vous signalent des erreurs dans vos campagnes actives.

## Synchronisation CRM {#crm-sync}

Les notifications de synchronisation CRM vous avertissent des problèmes critiques rencontrés avec la synchronisation CRM, tels que des autorisations incorrectes ou la synchronisation en cours d’arrêt.

**Microsoft Dynamics **

Les notifications Dynamics sont envoyées une fois toutes les 24 heures et contiennent des pistes qui n&#39;ont pas été synchronisées au cours de cette période. Les causes habituelles de l’échec sont les pistes de duplicata (comme ci-dessus) ou les erreurs de non-correspondance de longueur de champ.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Si vous utilisez Salesforce, les notifications d’erreur de synchronisation ressemblent à celles présentées ci-dessous. Les erreurs types comprennent les informations d’identification expirées et les limites d’API dépassées.

![](assets/salesforcesyncerror.png)

Engagement

Lorsque les pistes s&#39;épuisent dans un flux, nous envoyons une notification.  La notification comprend le nombre de pistes épuisées et d&#39;autres informations.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Si vous essayez d&#39;envoyer des pistes à Facebook sans accepter les conditions d&#39;utilisation, ou si vous essayez d&#39;envoyer des pistes à Facebook après avoir supprimé l&#39;application Marketo.

Nettoyage des campagnes à déclencheurs inexploitées

Désactivez les campagnes dynamiques déclenchées qui n’obtiennent plus d’activité. En savoir plus sur le [nettoyage de campagne de déclenchement automatique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

LinkedIn

Lorsque Marketo ne parvient pas à créer une nouvelle audience, à ouvrir une session ou à envoyer des courriers électroniques à LinkedIn après trois tentatives.

![](assets/linkedin.png)

Services Web

Vous serez averti lorsque vous atteindrez votre quota quotidien. Le quota est réinitialisé chaque nuit à minuit, heure du centre.

>[!NOTE]
>
>Certains des codes d&#39;erreur que vous pouvez recevoir sont décrits dans notre [Documentation du développeur](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes).
