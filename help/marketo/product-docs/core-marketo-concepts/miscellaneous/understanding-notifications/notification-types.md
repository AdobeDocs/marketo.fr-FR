---
unique-page-id: 2953243
description: Types de notification - Documents Marketo - Documentation du produit
title: Types de notification
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 5%

---

# Types de notification {#notification-types}

Il existe plusieurs types de notification.

## Erreur de la campagne  {#campaign-failure}

Les échecs de campagne vous informent des erreurs dans vos campagnes dynamiques.

## Synchronisation CRM {#crm-sync}

Les notifications de synchronisation CRM vous alertent sur les problèmes critiques liés à la synchronisation CRM, tels que les autorisations incorrectes ou la synchronisation en cours.

**[!DNL Microsoft Dynamics]**

Les notifications Dynamics sont envoyées une fois toutes les 24 heures et contiennent des pistes qui n’ont pas été synchronisées pendant cette période. Les raisons classiques de l’échec sont les pistes en double (comme ci-dessus) ou les erreurs de correspondance de longueur de champ.

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

Si vous utilisez Salesforce, les notifications d’erreur de synchronisation ressemblent à celle ci-dessous. Les erreurs types incluent les informations d’identification expirées et les limites d’API dépassées.

![](assets/salesforcesyncerror.png)

## Engagement {#engagement}

Quand les gens s&#39;épuisent dans un flux, nous envoyons une notification. La notification inclut le nombre de personnes qui se sont épuisées et d&#39;autres informations.

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

Si vous essayez d’envoyer des personnes vers Facebook sans accepter les conditions d’utilisation, ou si vous essayez d’envoyer des personnes vers Facebook après avoir supprimé l’application Marketo.

## Nettoyage des campagnes à déclencheurs inexploitées {#idle-trigger-campaign-cleanup}

Désactivez les campagnes dynamiques déclenchées qui n’obtiennent plus aucune activité. En savoir plus sur le [nettoyage de campagne de déclencheur automatique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

## LinkedIn {#linkedin}

Lorsque Marketo ne parvient pas à créer une audience, à se connecter ou à envoyer des emails push à LinkedIn après trois tentatives.

![](assets/linkedin.png)

## Services Web {#web-services}

Vous en serez informé lorsque vous atteindrez votre quota quotidien. Le quota est réinitialisé chaque nuit à minuit, heure du centre.

>[!NOTE]
>
>Certains des codes d’erreur que vous pouvez recevoir sont décrits dans notre [Documentation développeur](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/error-codes).
