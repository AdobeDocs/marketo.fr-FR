---
unique-page-id: 2952678
description: Utilisation de l’option Send Alert Info Token {{SP_Send_Alert_Info}} - Documentation Marketo - Documentation du produit
title: Utiliser le jeton d’information d’alerte Envoyer
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Utiliser le jeton d’information d’alerte Envoyer {#use-the-send-alert-info-token-sp-send-alert-info}

Le jeton `{{SP_Send_Alert_Info}}` est un jeton spécial à utiliser lors de la création d’emails d’alerte pour votre équipe commerciale.

>[!TIP]
>
>Ce jeton ne fonctionne que comme prévu lors de l&#39;envoi de l&#39;email qui le contient avec l&#39;étape de flux [Envoyer une alerte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) . Il ne fonctionnera pas lorsqu’il est utilisé dans une étape de flux Envoyer un courrier électronique .

Exemple d’alerte :

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Tête-toi ! Les URL des alertes ont des dates d’expiration. Assurez-vous donc qu’elles disposent d’une cadence prenant en charge ces types de messages. Les dates d&#39;expiration sont [ configurées par un administrateur](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Les informations suivantes sont incluses dans le `{{SP_Send_Alert_Info}}` :

* Prénom et nom comme lien vers le détail de la personne dans Marketo
* Un lien vers la personne dans votre CRM
* Nom de la campagne dans Marketo qui a envoyé l’alerte
* Heure à laquelle l’alerte a été envoyée

>[!NOTE]
>
>Le lien vers le CRM n&#39;apparaîtra que si la personne se trouve dans le système CRM (actuellement pas disponible avec Dynamics CRM). Le lien est accessible aux utilisateurs Marketo et non Marketo.

## Ajout du jeton SP_Send_Alert_Info à un message électronique {#add-the-sp-send-alert-info-token-to-an-email}

1. Sélectionnez l&#39;email et cliquez sur **Modifier le brouillon**.

   ![](assets/one-3.png)

1. Double-cliquez sur la zone modifiable à laquelle vous souhaitez ajouter le jeton.

   ![](assets/two-3.png)

1. Placez le curseur à l’endroit où vous souhaitez que le jeton soit, puis cliquez sur le bouton **Insérer un jeton** .

   ![](assets/three-3.png)

1. Recherchez et sélectionnez le jeton **`{{SP_Send_Alert_Info}}`** et cliquez sur **Insérer**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>N&#39;oubliez pas d&#39;approuver votre email.

C&#39;est bien ! Ce jeton est très utile et vous devez l’utiliser dans toutes les alertes que vous créez pour votre équipe commerciale.
