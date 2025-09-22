---
description: Mettre à jour le champ Type d’activité lors de la journalisation des activités dans Salesforce - Documents Marketo - Documentation du produit
title: Mettre à jour le champ Type d’activité lors de la journalisation des activités dans Salesforce
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 6%

---

# Mettre à jour le champ Type d’activité lors de la journalisation des activités dans Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

Les actions peuvent synchroniser automatiquement vos activités d’e-mail et d’appel avec Salesforce à utiliser pour les rapports et augmenter la visibilité sur l’historique des activités. Lors de la journalisation des activités, assurez-vous que le champ Type d’activité est correctement mis à jour vers E-mail, Appel ou Réponse, en fonction du type d’activité consignée.

>[!NOTE]
>
>La journalisation des e-mails en Cci ne s’effectue pas dans la liste de sélection Type de tâche et remplit automatiquement le champ de type en tant qu’« e-mail », car ils sont envoyés à Salesforce via votre adresse en Cci.

## Choses à savoir {#things-to-know}

* Une connexion à Salesforce est requise pour que le type de tâche soit mis à jour.
* Aucune valeur Type par défaut ne doit être sélectionnée dans la liste de sélection Type de tâche.
* L’appel, la réponse et l’e-mail doivent tous figurer dans la liste de sélection du type de tâche (les majuscules sont importantes).
* Les workflows ou les triggers de Salesforce qui mettent à jour le champ Type de tâche peuvent interférer avec ce processus.

## Configuration {#setup}

Vérifiez d’abord que vous avez mis en place les valeurs correctes dans la liste de sélection. Vous aurez besoin de l’aide de votre administrateur Salesforce pour apporter des modifications à votre liste de sélection.

Commencez par vérifier les valeurs manquantes dans votre liste de sélection de type de tâche (e-mail, appel et réponse absents). Vous aurez peut-être besoin de l’aide de votre administrateur Salesforce pour vérifier ceci et apporter des modifications à votre liste de sélection de type d’activité. Pour apporter ces modifications, votre administrateur Salesforce peut suivre les étapes ci-dessous.

### Dans Salesforce Lightning {#salesforce-lightning}

1. Accédez à [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Cliquez sur l’icône d’engrenage dans le coin supérieur droit et sélectionnez **Configuration** > **Gestionnaire d’objets**.
1. Tapez « task » dans la zone « Quick Find ».
1. Dans le panneau de gauche, cliquez sur **Champs et relations**.
1. Cliquez sur le libellé du champ **Type**.
1. Sous Valeur de la liste de sélection du type de tâche, cliquez sur **Nouveau**.
1. Tapez le nom des valeurs de la liste de sélection de type de tâche manquantes (« E-mail », « Appel », « Réponse »).
1. Cliquez sur **Enregistrer**

### Dans Salesforce Classic {#salesforce-classic}

1. Accédez à [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Cliquez sur **Configuration** > **Créer** > **Personnaliser** > **Activités** > **Champs de tâche**.
1. Cliquez sur **Type**.
1. Sous Valeur de la liste de sélection du type de tâche, cliquez sur **Nouveau**.
1. Tapez le nom des valeurs de la liste de sélection de type de tâche manquantes (« E-mail », « Appel », « Réponse »).
1. Cliquez sur **Enregistrer**

Maintenant que cela est en place, vous allez commencer à voir le champ Type remplir la valeur correspondante pour les e-mails, appels et réponses consignés. Ces valeurs ne seront _pas_ renseignées sur les tâches de rappel des actions Sales Insight.

>[!NOTE]
>
>Si vous ne voyez pas &#39;Répondre&#39; comme valeur, ajoutez-la en cliquant sur **Nouveau**. &#39;Répondre&#39; n&#39;est pas une valeur standard dans Salesforce.

>[!MORELIKETHIS]
>
>* [Journalisation des attributs d’activité commerciale dans Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Configurer la personnalisation des détails de l’activité Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Synchroniser les activités de vente avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
