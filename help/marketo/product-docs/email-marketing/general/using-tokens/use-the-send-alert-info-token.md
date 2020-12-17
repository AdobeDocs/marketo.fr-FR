---
unique-page-id: 2952678
description: Utiliser le jeton Envoyer les informations d'alerte {{SP_Send_Alert_Info}} - Documents marketing - Documentation du produit
title: Utiliser le jeton d'informations d'alerte Envoyer
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Utiliser le jeton Envoyer les informations d&#39;alerte {#use-the-send-alert-info-token-sp-send-alert-info}

Le jeton `{{SP_Send_Alert_Info}}` est un jeton spécial à utiliser lors de la création d&#39;e-mails d&#39;alerte pour votre équipe commerciale.

>[!TIP]
>
>Ce jeton ne fonctionne que comme prévu lors de l’envoi du courrier électronique contenant le message avec l’étape de flux [Envoyer l’alerte](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md). Il ne fonctionnera pas lorsqu&#39;il est utilisé dans une étape de flux Envoyer un courrier électronique.

Exemple d&#39;alerte :   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Allez ! Les URL des alertes comportent des dates d’expiration. Assurez-vous donc qu’elles disposent d’une cadence prenant en charge ces types de messages. Les dates d’expiration sont [configurées par un administrateur](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Les informations suivantes font partie du `{{SP_Send_Alert_Info}}` :

* Prénom et nom en tant que lien vers le détail de la personne dans Marketo
* Un lien vers la personne dans votre CRM
* Nom de la campagne dans Marketo qui a envoyé l&#39;alerte
* Heure à laquelle l&#39;alerte a été envoyée

>[!NOTE]
>
>Le lien vers la gestion de la relation client n&#39;apparaîtra que si la personne se trouve dans le système de gestion de la relation client (actuellement indisponible avec Dynamics CRM). Le lien est accessible aux utilisateurs de Marketing et non de Marketing.

## Ajouter le jeton SP_Send_Alert_Info à un courrier électronique {#add-the-sp-send-alert-info-token-to-an-email}

1. Sélectionnez le courriel et cliquez sur **Modifier le brouillon**.

   ![](assets/one-3.png)

1. Cliquez avec le doublon sur la zone modifiable à laquelle vous souhaitez ajouter le jeton.

   ![](assets/two-3.png)

1. Placez le curseur à l’endroit où vous souhaitez placer le jeton, puis cliquez sur le bouton **Insérer un jeton**.

   ![](assets/three-3.png)

1. Recherchez et sélectionnez le jeton **`{{SP_Send_Alert_Info}}`**, puis cliquez sur **Insérer**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**Rappel**
>
>N&#39;oubliez pas d&#39;approuver votre courriel.

C&#39;est bien ! Ce jeton est très utile et vous devez l&#39;utiliser dans toutes les alertes que vous créez pour votre équipe commerciale.