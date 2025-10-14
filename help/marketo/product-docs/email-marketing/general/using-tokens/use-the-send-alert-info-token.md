---
unique-page-id: 2952678
description: Utilisez le jeton Envoyer le jeton d’information d’alerte {{SP_Send_Alert_Info}} - Documents Marketo - Documentation du produit .
title: Utiliser le jeton d’envoi d’information d’alerte
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 5%

---

# Utiliser le jeton d’envoi d’information d’alerte {#use-the-send-alert-info-token-sp-send-alert-info}

Le jeton `{{SP_Send_Alert_Info}}` est un jeton spécial à utiliser lors de la création d’e-mails d’alerte pour votre équipe commerciale.

>[!TIP]
>
>Ce jeton ne fonctionne que comme prévu lors de l’envoi de l’e-mail le contenant avec l’étape de flux [&#x200B; Envoyer une alerte &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md). Elle ne fonctionne pas lorsqu’elle est utilisée dans une étape de flux Envoyer un e-mail .

Exemple d’alerte :

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Attention ! Les URL figurant dans les alertes ont des dates d’expiration. Veillez donc à ce qu’elles aient une cadence prenant en charge ces types de messages. Les dates d’expiration sont [configurées par un administrateur](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Les informations suivantes sont incluses dans le `{{SP_Send_Alert_Info}}` :

* Prénom et nom comme lien vers les détails de la personne dans Marketo
* Un lien vers la personne dans votre CRM
* Nom de la campagne dans Marketo qui a envoyé l’alerte
* Heure à laquelle l’alerte a été envoyée

>[!NOTE]
>
>Le lien vers le CRM n&#39;apparaîtra que si la personne est dans le système CRM (actuellement non disponible avec Dynamics CRM). Le lien est accessible aux utilisateurs de Marketo et aux autres utilisateurs de Marketo.

## Ajouter le jeton SP_Send_Alert_Info à un e-mail {#add-the-sp-send-alert-info-token-to-an-email}

1. Sélectionnez l’e-mail et cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/one-3.png)

1. Double-cliquez sur la zone modifiable à laquelle vous souhaitez ajouter le jeton.

   ![](assets/two-3.png)

1. Placez le curseur à l’endroit où vous souhaitez placer le jeton, puis cliquez sur le bouton **[!UICONTROL Insérer un jeton]**.

   ![](assets/three-3.png)

1. Recherchez et sélectionnez le jeton de **[!UICONTROL {{SP_Send_Alert_Info}}]** et cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>N’oubliez pas d’approuver votre e-mail.

Bon truc ! Ce jeton est très utile et vous devez l’utiliser dans toutes les alertes que vous créez pour votre équipe commerciale.
