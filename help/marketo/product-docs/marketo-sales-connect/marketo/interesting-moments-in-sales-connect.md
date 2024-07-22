---
unique-page-id: 30082174
description: Moments intéressants dans Sales Connect - Documents Marketo - Documentation du produit
title: Moments intéressants dans Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 3a3287ed20962a052e0015161e34e33a95dd450a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Moments intéressants dans Sales Connect {#interesting-moments-in-sales-connect}

Les moments intéressants sont essentiels pour communiquer avec votre équipe commerciale via Marketo Sales Connect.

>[!AVAILABILITY]
>
>Ils sont disponibles uniquement pour les clients [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) et Marketo Sales Connect.

>[!PREREQUISITES]
>
>* Vous devez avoir une [connexion à Salesforce CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"}
>* Vous devez être le responsable ou le propriétaire du contact dans Salesforce.
>* Vous devez avoir accès à [accorder l’accès à la connexion du Marketo Engage](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"}

## Quel est un moment intéressant ? {#what-is-an-interesting-moment}

C&#39;est à toi de décider ! Vous décidez quelles informations sont pertinentes pour votre équipe commerciale. Votre équipe commerciale peut vouloir savoir quand une piste :

* Visite la page des tarifs sur votre site web
* Cliquer sur un lien dans un nouvel e-mail d’annonce de produit
* Demande une démonstration de produit

## Comment créer un moment intéressant ? {#how-do-i-create-an-interesting-moment}

1. Choisissez une [campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), de préférence une campagne que votre équipe commerciale trouvera intéressante si elle est déclenchée.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Faites glisser l’étape de flux **Moments intéressants** .

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Sélectionnez un **type** (Email, Jalon ou Web).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Ecrivez un message à votre équipe commerciale dans le champ **Description** qui explique pourquoi cette action est importante.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo ajoute également la date à laquelle il s’est produit et la manière dont le moment intéressant a été ajouté (par exemple, action de piste > étape de flux, API SOAP).

## À quoi ressemble un moment intéressant dans Marketo ?  {#what-does-an-interesting-moment-look-like-in-marketo}

Les moments intéressants seront affichés dans le [journal d’activité de la piste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## À quoi ressemble un moment intéressant dans Sales Connect ? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Les moments intéressants s’affichent en temps réel dans le flux en direct d’un utilisateur. Nous utilisons l’identifiant du propriétaire principal dans Salesforce pour montrer aux utilisateurs les moments intéressants de pistes pertinentes dont ils sont propriétaires. Les utilisateurs peuvent rapidement suivre les pistes par email/téléphone/campagne de vente en cliquant sur la liste déroulante en regard du nom de la piste.

![](assets/engagement.jpg)
