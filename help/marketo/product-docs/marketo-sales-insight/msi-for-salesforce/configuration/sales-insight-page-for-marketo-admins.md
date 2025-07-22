---
unique-page-id: 42762409
description: Page Ventes Insight pour les administrateurs Marketo - Documentation de Marketo - Documentation du produit
title: Page Ventes Insight pour les administrateurs Marketo
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Page [!DNL Sales Insight] pour les administrateurs Marketo {#sales-insight-page-for-marketo-admins}

Les administrateurs Marketo disposent de certains privilèges dans [!DNL Sales Insight]. Découvrez-les ci-dessous.

## Configuration de l’API Soap {#soap-api-configuration}

Ces informations d’identification sont utilisées pour connecter votre compte [!DNL Salesforce] à votre instance Marketo, afin d’utiliser MSI dans [!DNL Salesforce].

![](assets/one-1.png)

## Configuration de l’API REST {#rest-api-configuration}

Ces informations d’identification sont utilisées pour connecter votre compte [!DNL Salesforce] à votre instance Marketo, afin d’utiliser le tableau de bord MSI Insights dans [!DNL Salesforce].

![](assets/two-1.png)

## Paramètres de score de la personne {#person-score-settings}

* **[!UICONTROL Étoiles]** : les étoiles représentent le score total des prospects par rapport aux autres prospects.
* **[!UICONTROL Flames]** : les flammes représentent l’urgence - jusqu’à quel point le score d’un prospect a changé récemment.

Par défaut, [!DNL Marketo Sales Insight] utilise le champ Score du lead pour calculer les étoiles et les flammes. Mais si vous souhaitez sélectionner un autre champ, procédez comme suit :

1. Dans la zone **[!UICONTROL Admin]** de Marketo, cliquez sur **[!UICONTROL Insight des ventes]**.

   ![](assets/four.png)

1. Sous [!UICONTROL Paramètres de notation des leads], cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/five.png)

1. Sélectionnez le champ à utiliser pour les étoiles.

   ![](assets/six.png)

1. Sélectionnez le champ à utiliser pour les flammes.

   ![](assets/seven.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**. Le recalcul de Sales insight prendra un certain temps. Vous pouvez vérifier votre CRM plus tard pour voir les étoiles et les flammes.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Si vous ne disposez pas déjà de vos champs de score personnalisés, voici comment les [créer](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Étoiles et flammes ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Paramètres {#settings}

![](assets/nine.png)

**Paramètres de désabonnement :**

Vous pouvez choisir parmi les paramètres de désabonnement suivants pour [!UICONTROL Aucun modèle], [!UICONTROL E-mails standard] et [!UICONTROL E-mails opérationnels]

* [!UICONTROL Respecter le paramètre de désabonnement]
* [!UICONTROL Respectez les paramètres de désabonnement lorsque plus d’un destinataire]
* [!UICONTROL Respectez les paramètres de désabonnement lorsque plus de 5 destinataires]
* [!UICONTROL Ignorer les paramètres de désabonnement]

**Activer la possibilité de verrouiller des modèles :**

Lorsque cette option est activée, les utilisateurs MSI ne peuvent pas modifier les modèles lors de l&#39;envoi d&#39;e-mails depuis [!DNL Salesforce]

**Activer le flux RSS :**

Lorsque cette option est activée, les utilisateurs MSI peuvent afficher leur flux de leads dans un flux RSS (en plus du flux de leads dans [!DNL Salesforce]). Le flux RSS ne peut fonctionner que si la fonction « [!UICONTROL Expiration du jeton] » est désactivée.

**Expiration du jeton :**

L’expiration des jetons est contrôlée dans le Gestionnaire de fonctionnalités. Pour l’activer/désactiver, contactez l’assistance technique de [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Lorsqu’ils sont activés, tous les jetons Marketo expirent dans les 10 minutes. Lorsqu’ils sont désactivés, les jetons Marketo n’expirent pas.

Les jetons générés avant l’activation de l’expiration des jetons ne disposeront pas d’un délai d’expiration en fonction duquel effectuer une validation, ils n’expireront donc pas même si la fonctionnalité est actuellement activée.

Les jetons générés après l’activation de l’expiration des jetons auront un délai d’expiration de 10 minutes ; ils expireront donc toujours dans 10 minutes même après la désactivation de la fonctionnalité.

Le comportement du jeton dépendra de la date à laquelle il a été généré (lorsque la fonction d’expiration du jeton a été activée/désactivée, plutôt que de son statut actuel de fonction).
