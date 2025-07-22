---
description: Moments intéressants dans les actions de Sales Insight - Documents Marketo - Documentation du produit
title: Moments intéressants dans les actions Sales Insight
exl-id: b2423fbb-9ce0-4ce9-bc26-93aa69aa9e12
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Moments significatifs de la [!DNL Sales Insight Actions] {#interesting-moments-in-sales-insight-actions}

Les moments intéressants sont la clé pour communiquer avec votre équipe de vente à travers [!DNL Marketo Sales Insight Actions].

## Qu&#39;est-ce qu&#39;un moment intéressant ? {#what-is-an-interesting-moment}

C&#39;est à toi de voir ! Vous décidez quelles informations sont pertinentes pour votre équipe de vente. Votre équipe de vente peut vouloir savoir quand un prospect :

* Visite la page de tarification de votre site web
* Clique sur un lien dans un e-mail d’annonce de nouveau produit.
* Demande une démonstration du produit

## Comment créer un moment intéressant ? {#how-do-i-create-an-interesting-moment}

1. Choisissez une [campagne intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}, de préférence une campagne que votre équipe de vente trouverait intéressante si elle était déclenchée.

   ![](assets/interesting-moments-in-sales-insight-actions-1.png)

1. Faites glisser sur l’étape de flux **[!UICONTROL Moments significatifs]**.

   ![](assets/interesting-moments-in-sales-insight-actions-2.png)

1. Sélectionnez un **type** (e-mail, jalon ou web).

   ![](assets/interesting-moments-in-sales-insight-actions-3.png)

1. Dans le champ **[!UICONTROL Description]**, envoyez un message à votre équipe commerciale pour expliquer l’importance de cette action.

   ![](assets/interesting-moments-in-sales-insight-actions-4.png)

   >[!NOTE]
   >
   >Marketo ajoutera également la date à laquelle il s’est produit et la manière dont le moment intéressant a été ajouté (c’est-à-dire action de lead > étape de flux, API SOAP).

## À quoi ressemble un moment intéressant dans Marketo ?  {#what-does-an-interesting-moment-look-like-in-marketo}

Les moments significatifs seront affichés dans le [journal d’activité du prospect](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

![](assets/interesting-moments-in-sales-insight-actions-5.png)

## À quoi ressemble un moment intéressant en [!DNL Sales Insight Actions] ? {#what-does-an-interesting-moment-look-like-in-sales-insight-actions}

Les moments significatifs seront affichés en temps réel dans le flux dynamique d’un utilisateur. Nous utilisons l’ID du propriétaire du prospect dans [!DNL Salesforce] pour afficher les moments intéressants des prospects pertinents dont ils sont propriétaires. Les utilisateurs peuvent rapidement suivre les prospects par e-mail, téléphone ou campagne commerciale en cliquant sur la liste déroulante en regard du nom du prospect.

![](assets/interesting-moments-in-sales-insight-actions-6.png)
