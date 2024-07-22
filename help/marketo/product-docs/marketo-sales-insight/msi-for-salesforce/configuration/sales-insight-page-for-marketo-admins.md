---
unique-page-id: 42762409
description: Page d’aperçu des ventes pour les administrateurs Marketo - Documents Marketo - Documentation du produit
title: Page d’aperçu des ventes pour les administrateurs Marketo
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 1%

---

# Page d’aperçu des ventes pour les administrateurs Marketo {#sales-insight-page-for-marketo-admins}

Les administrateurs Marketo disposent de certains privilèges dans Sales Insight. Apprenez ce qu&#39;ils sont ci-dessous.

## Configuration de l’API Soap {#soap-api-configuration}

Ces informations d’identification sont utilisées pour connecter votre compte Salesforce à votre instance Marketo afin d’utiliser MSI dans Salesforce.

![](assets/one-1.png)

## Configuration de l’API REST {#rest-api-configuration}

Ces informations d’identification sont utilisées pour connecter votre compte Salesforce à votre instance Marketo afin d’utiliser le tableau de bord des statistiques MSI dans Salesforce.

![](assets/two-1.png)

## Paramètres de score de personne {#person-score-settings}

* **Stars** : les étoiles représentent le score de piste total par rapport aux autres pistes.
* **Flammes** : les flammes représentent l’urgence - le score d’un prospect a récemment changé.

Par défaut, Marketo Sales Insight utilise le champ Lead Score pour calculer les étoiles et les flammes. Mais si vous souhaitez sélectionner un autre champ, voici comment :

1. Dans la zone **Admin** de Marketo, cliquez sur **Sales Insight**.

   ![](assets/four.png)

1. Sous Paramètres de score de piste, cliquez sur **Modifier**.

   ![](assets/five.png)

1. Sélectionnez le champ à utiliser pour les étoiles.

   ![](assets/six.png)

1. Sélectionnez le champ à utiliser pour les flammes.

   ![](assets/seven.png)

1. Cliquez sur **Enregistrer**. Les statistiques sur les ventes prendront un certain temps pour être recalculées. Vous pouvez vérifier votre CRM plus tard pour voir les étoiles et les flammes.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Si vous ne disposez pas déjà de vos champs de score personnalisés, voici comment [les créer](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Étoiles et flammes](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Paramètres {#settings}

![](assets/nine.png)

**Paramètres de désabonnement :**

Vous pouvez choisir parmi les paramètres de désabonnement suivants pour Aucun modèle, Courriers électroniques standard et e-mails opérationnels.

* Respect du paramètre Unsubscribe
* Respecter les paramètres de désabonnement lorsque plus d’un destinataire
* Respecter les paramètres de désabonnement lorsque plus de 5 destinataires
* Ignorer les paramètres de désabonnement

**Activer la possibilité de verrouiller des modèles :**

Lorsque cette option est activée, les utilisateurs MSI ne peuvent pas modifier les modèles lors de l’envoi d’emails à partir de Salesforce.

**Activer le flux RSS :**

Lorsqu’ils sont activés, les utilisateurs MSI peuvent afficher leur flux de piste dans un flux RSS (en plus du flux de piste dans Salesforce). Le flux RSS ne peut fonctionner que si la fonction &quot;Expiration des jetons&quot; est désactivée.

**Expiration du jeton :**

L’expiration du jeton est contrôlée dans le Gestionnaire de fonctionnalités. Pour l’activer/désactiver, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Lorsque cette option est activée, tous les jetons Marketo expirent dans les 10 minutes. Lorsque cette option est désactivée, les jetons Marketo n’expirent pas.

Les jetons générés avant l’activation de l’expiration des jetons n’auront pas de délai d’expiration pour la validation. Ils n’expireront donc pas même si la fonctionnalité est actuellement activée.

Les jetons générés après l’activation de l’expiration des jetons ont un délai d’expiration de 10 minutes. Ils expirent donc dans 10 minutes, même lorsque la fonction est désactivée.

Le comportement du jeton dépend du moment où il a été généré (lorsque la fonction Expiration du jeton a été activée/désactivée, plutôt que de son état actuel).
