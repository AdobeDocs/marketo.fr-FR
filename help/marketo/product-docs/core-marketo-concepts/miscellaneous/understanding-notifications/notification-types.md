---
unique-page-id: 2953243
description: Types de notifications - Documents Marketo - Documentation du produit
title: Types de notifications
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 7%

---

# Types de notifications {#notification-types}

Il existe plusieurs types de notification.

## Erreur de la campagne  {#campaign-failure}

Les échecs de campagne vous informent des erreurs survenues dans vos campagnes intelligentes.

## Synchronisation CRM {#crm-sync}

Les notifications de synchronisation CRM vous avertissent des problèmes critiques rencontrés avec la synchronisation CRM, tels que des autorisations incorrectes ou une synchronisation en cours d’interruption.

**[!DNL Microsoft Dynamics]**

Les notifications [!DNL Dynamics] sont envoyées une fois toutes les 24 heures et contiennent les prospects dont la synchronisation a échoué au cours de cette période. Les raisons typiques de l’échec sont les prospects dupliqués (comme ci-dessus) ou les erreurs de non-correspondance de longueur de champ.

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

Si vous utilisez [!DNL Salesforce], les notifications d’erreur de synchronisation ressemblent à celle ci-dessous. Les erreurs standard incluent les informations d’identification expirées et les limites d’API dépassées.

![](assets/salesforcesyncerror.png)

## Engagement {#engagement}

Lorsque les gens s&#39;épuisent dans un flux, nous envoyons une notification. La notification comprend le nombre de personnes qui se sont épuisées et d’autres informations.

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

Si vous tentez d&#39;envoyer des personnes sur Facebook sans accepter les Conditions d&#39;utilisation, ou si vous tentez d&#39;envoyer des personnes sur Facebook après avoir supprimé l&#39;application Marketo.

## Nettoyage des campagnes à déclencheurs inexploitées {#idle-trigger-campaign-cleanup}

Désactivez les campagnes intelligentes déclenchées qui n’obtiennent plus d’activité. En savoir plus sur le [nettoyage automatique des campagnes de déclenchement](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

## LinkedIn {#linkedin}

Lorsque Marketo ne parvient pas à créer une nouvelle audience, connectez-vous ou envoyez des e-mails à LinkedIn après trois tentatives.

![](assets/linkedin.png)

## Services Web {#web-services}

Vous serez averti lorsque vous atteindrez votre quota quotidien. Le quota est réinitialisé chaque nuit à minuit, heure du Centre.

>[!NOTE]
>
>Certains des codes d’erreur que vous pouvez recevoir sont décrits dans notre [Documentation destinée aux développeurs](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/error-codes).
