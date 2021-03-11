---
unique-page-id: 42762409
description: Page d'informations sur les ventes pour les administrateurs du marketing - Documents marketing - Documentation du produit
title: Page d'informations commerciales pour les administrateurs du marketing
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---


# Page d&#39;informations commerciales pour les administrateurs du marketing {#sales-insight-page-for-marketo-admins}

Les administrateurs du marketing disposent de certains privilèges dans Sales Insight. Apprenez ce qu&#39;ils sont ci-dessous.

## Configuration de l&#39;API Soap {#soap-api-configuration}

Ces informations d’identification sont utilisées pour connecter votre compte Salesforce à votre instance Marketo afin d’utiliser MSI dans Salesforce.

![](assets/one-1.png)

## Configuration de l&#39;API REST {#rest-api-configuration}

Ces informations d’identification sont utilisées pour connecter votre compte Salesforce à votre instance Marketo, afin d’utiliser le Tableau de bord MSI Insights dans Salesforce.

![](assets/two-1.png)

Vous pouvez choisir de supprimer les informations d’identification de l’API REST dans SFDC et d’utiliser uniquement les API Soap. Ceci désactivera le Tableau de bord Insights

![](assets/three-1.png)

## Paramètres de note personnelle {#person-score-settings}

* **Etoiles** : Les étoiles représentent le score de piste total par rapport aux autres pistes.
* **Flammes** : Les flammes représentent l&#39;urgence - à quel point le score d&#39;un prospect a changé récemment.

Par défaut, le module Marketing Sales Insight utilise le champ Score de piste pour calculer les étoiles et les flammes. Mais si vous voulez choisir un autre champ, voici comment :

1. Dans la zone **Admin** de Marketo, cliquez sur **Sales Insight**.

   ![](assets/four.png)

1. Sous Paramètres de score de piste, cliquez sur **Modifier**.

   ![](assets/five.png)

1. Sélectionnez le champ à utiliser pour les étoiles.

   ![](assets/six.png)

1. Sélectionnez le champ à utiliser pour les flammes.

   ![](assets/seven.png)

1. Cliquez sur **Enregistrer**. Il faudra un certain temps pour calculer à nouveau les statistiques des ventes. Vous pourrez vérifier votre CRM ultérieurement pour voir les étoiles et les flammes.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Si vous ne disposez pas déjà de vos champs de score personnalisés, voici comment [les créer](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Etoiles et flammes](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Paramètres {#settings}

![](assets/nine.png)

**Paramètres de désabonnement :**

Vous pouvez choisir parmi les paramètres de désabonnement suivants pour Aucun modèle, Courriers électroniques standard et E-mails opérationnels.

* Paramètre Respecter la désinscription
* Respecter les paramètres de désabonnement lorsque plus d’un destinataire
* Respecter les paramètres de désabonnement lorsque plus de 5 destinataires
* Ignorer les paramètres de désabonnement

**Permet de verrouiller des modèles :**

Lorsqu&#39;ils sont activés, les utilisateurs MSI ne pourront pas modifier les modèles lors de l&#39;envoi de courriers électroniques à partir de Salesforce.

**Activer le flux RSS :**

Une fois activé, les utilisateurs MSI peuvent vue leur flux de piste dans un flux RSS (en plus du flux de piste dans Salesforce). Le flux RSS ne peut fonctionner que si la fonction &quot;Token Expiration&quot; est désactivée.

**Expiration du jeton :**

L’expiration du jeton est contrôlée dans le Gestionnaire de fonctionnalités. Pour l’activer/désactiver, contactez le [Support marketing](https://nation.marketo.com/t5/Support/ct-p/Support). Lorsque cette option est activée, tous les jetons Marketo expirent dans les 10 minutes. Lorsque cette option est désactivée, les jetons Marketo n’expirent pas.

Les jetons générés avant l&#39;activation de l&#39;expiration des jetons n&#39;auront pas de délai d&#39;expiration pour la validation. Ils n&#39;expireront donc pas même si la fonction est actuellement activée.

Les jetons générés après l&#39;activation de l&#39;expiration des jetons auront un délai d&#39;expiration de 10 minutes. Ils expireront donc dans 10 minutes, même après la désactivation de la fonction.

Le comportement du jeton dépend du moment où il a été généré (lorsque la fonction d&#39;expiration du jeton a été activée/désactivée, plutôt que de son état actuel).
