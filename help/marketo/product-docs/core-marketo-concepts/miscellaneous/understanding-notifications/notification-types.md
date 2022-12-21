---
unique-page-id: 2953243
description: Types de notification - Documents Marketo - Documentation du produit
title: Types de notification
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 5%

---

# Types de notification {#notification-types}

Il existe plusieurs types de notification.

## Erreur de la campagne   {#campaign-failure}

Les échecs de campagne vous informent des erreurs dans vos campagnes dynamiques.

## Synchronisation CRM {#crm-sync}

Les notifications de synchronisation CRM vous alertent sur les problèmes critiques liés à la synchronisation CRM, tels que les autorisations incorrectes ou la synchronisation en cours.

**Microsoft Dynamics**

Les notifications Dynamics sont envoyées une fois toutes les 24 heures et contiennent des pistes qui n’ont pas été synchronisées pendant cette période. Les raisons classiques de l’échec sont les pistes en double (comme ci-dessus) ou les erreurs de correspondance de longueur de champ.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Si vous utilisez Salesforce, les notifications d’erreur de synchronisation ressemblent à celle ci-dessous. Les erreurs types comprennent les informations d’identification expirées et les limites d’API dépassées.

![](assets/salesforcesyncerror.png)

Engagement

Lorsque les pistes s’épuisent dans un flux, nous envoyons une notification.  La notification inclut le nombre de pistes qui se sont épuisées et d’autres informations.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Si vous tentez d’envoyer des prospects vers Facebook sans accepter les conditions d’utilisation, ou si vous essayez d’envoyer des prospects vers Facebook après avoir supprimé l’application Marketo.

Nettoyage des campagnes à déclencheurs inexploitées

Désactivez les campagnes dynamiques déclenchées qui n’obtiennent plus aucune activité. En savoir plus sur  [nettoyage automatique de la campagne de déclenchement](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

LinkedIn

Lorsque Marketo ne parvient pas à créer une audience, à se connecter ou à envoyer des emails push à LinkedIn après trois tentatives.

![](assets/linkedin.png)

Services web

Vous en serez informé lorsque vous atteindrez votre quota quotidien. Le quota est réinitialisé chaque nuit à minuit, heure du centre.

>[!NOTE]
>
>Certains des codes d’erreur que vous pouvez recevoir sont décrits dans notre [Documentation destinée aux développeurs](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes).
