---
description: Moments intéressants dans les actions d’aperçu des ventes - Documents Marketo - Documentation du produit
title: Moments intéressants dans les actions d’aperçu commercial
exl-id: b2423fbb-9ce0-4ce9-bc26-93aa69aa9e12
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Moments intéressants dans les actions d’aperçu commercial {#interesting-moments-in-sales-insight-actions}

Les moments intéressants sont essentiels pour communiquer avec votre équipe commerciale au moyen des actions Marketo Sales Insight.

## Quel est un moment intéressant ? {#what-is-an-interesting-moment}

C&#39;est à toi de décider ! Vous décidez quelles informations sont pertinentes pour votre équipe commerciale. Votre équipe commerciale peut vouloir savoir quand une piste :

* Visite la page des tarifs sur votre site web
* Cliquer sur un lien dans un nouvel e-mail d’annonce de produit
* Demande une démonstration de produit

## Comment créer un moment intéressant ? {#how-do-i-create-an-interesting-moment}

1. Choisissez une [campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}, de préférence une campagne que votre équipe commerciale trouvera intéressante si elle est déclenchée.

   ![](assets/interesting-moments-in-sales-insight-actions-1.png)

1. Faites glisser l’étape de flux **Moments intéressants** .

   ![](assets/interesting-moments-in-sales-insight-actions-2.png)

1. Sélectionnez un **type** (Email, Jalon ou Web).

   ![](assets/interesting-moments-in-sales-insight-actions-3.png)

1. Ecrivez un message à votre équipe commerciale dans le champ **Description** qui explique pourquoi cette action est importante.

   ![](assets/interesting-moments-in-sales-insight-actions-4.png)

   >[!NOTE]
   >
   >Marketo ajoute également la date à laquelle il s’est produit et la manière dont le moment intéressant a été ajouté (par exemple, action de piste > étape de flux, API SOAP).

## À quoi ressemble un moment intéressant dans Marketo ?  {#what-does-an-interesting-moment-look-like-in-marketo}

Les moments intéressants seront affichés dans le [journal d’activité de la piste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

![](assets/interesting-moments-in-sales-insight-actions-5.png)

## À quoi ressemble un moment intéressant dans les actions Sales Insight ? {#what-does-an-interesting-moment-look-like-in-sales-insight-actions}

Les moments intéressants s’affichent en temps réel dans le flux en direct d’un utilisateur. Nous utilisons l’identifiant du propriétaire principal dans Salesforce pour montrer aux utilisateurs les moments intéressants de pistes pertinentes dont ils sont propriétaires. Les utilisateurs peuvent rapidement suivre les pistes par email/téléphone/campagne de vente en cliquant sur la liste déroulante en regard du nom de la piste.

![](assets/interesting-moments-in-sales-insight-actions-6.png)
