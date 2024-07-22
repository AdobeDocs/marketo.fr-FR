---
description: Mettre à jour le champ Type d’activité lors de la connexion des activités à Salesforce - Documents Marketo - Documentation du produit
title: Mettre à jour le champ Type d’activité lors de la connexion des activités à Salesforce
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 1%

---

# Mettre à jour le champ Type d’activité lors de la connexion des activités à Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

Les actions peuvent synchroniser automatiquement votre email et appeler les activités vers Salesforce afin qu’elles soient utilisées pour la création de rapports et accroître la visibilité dans l’historique des activités. Lors de la journalisation des activités, assurez-vous que le champ Type d’activité est correctement mis à jour vers Email, Call ou Reply, selon le type d’activité consigné.

>[!NOTE]
>
>La journalisation des emails via Cci ne se tourne pas vers la liste de sélection Type de tâche et remplit automatiquement le champ Type en tant qu’&quot;email&quot; puisqu’ils sont envoyés à Salesforce via votre adresse en Cci.

## Informations à connaître {#things-to-know}

* Une connexion avec Salesforce est requise pour que le type de tâche soit mis à jour.
* Aucune valeur Type par défaut ne doit être sélectionnée dans la liste de sélection Type de tâche.
* L’appel, la réponse et l’e-mail doivent tous exister dans la liste de sélection Type de tâche (les majuscules et les minuscules sont importantes).
* Les workflows ou les Triggers dans Salesforce qui mettent à jour le champ Type de tâche peuvent interférer avec ce processus.

## Configuration {#setup}

Vérifiez d’abord que les valeurs correctes de liste de sélection sont en place. Vous aurez besoin de l’aide de votre administrateur Salesforce pour apporter des modifications à votre liste de sélection.

Vérifiez d’abord les valeurs manquantes dans votre liste de sélecteur de type de tâche (par e-mail, appel et réponse). Vous aurez peut-être besoin de l’aide de votre administrateur Salesforce pour passer en revue cette question et apporter des modifications à votre liste de sélection de type d’activité. Pour apporter ces modifications, votre administrateur Salesforce peut suivre les étapes ci-dessous.

### Dans Salesforce Lightning {#salesforce-lightning}

1. Accédez à [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Cliquez sur l’icône d’engrenage dans le coin supérieur droit et sélectionnez **Configuration** > **Gestionnaire d’objets**.
1. Saisissez &quot;task&quot; dans la zone &quot;Recherche rapide&quot;.
1. Dans le panneau de gauche, cliquez sur **Fields &amp; Relationships**.
1. Cliquez sur le libellé du champ **Type**.
1. Sous Valeur de liste de sélection de type de tâche, cliquez sur **New**.
1. Saisissez le nom des valeurs de liste de sélection du type de tâche manquantes (&quot;Email, &quot;Call&quot;, &quot;Reply&quot;).
1. Cliquez sur **Enregistrer**.

### Dans Salesforce Classic {#salesforce-classic}

1. Accédez à [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Cliquez sur **Configuration** > **Build** > **Customize** > **Activities** > **Task Fields**.
1. Cliquez sur **Type**.
1. Sous Valeur de liste de sélection de type de tâche, cliquez sur **New**.
1. Saisissez le nom des valeurs de liste de sélection du type de tâche manquantes (&quot;Email, &quot;Call&quot;, &quot;Reply&quot;).
1. Cliquez sur **Enregistrer**.

Maintenant que ce champ est en place, vous allez commencer à voir le champ Type renseigner la valeur correspondante pour les emails, les appels et les réponses consignés. Ces valeurs seront _not_ renseignées dans les tâches de rappel des actions de statistiques sur les ventes .

>[!NOTE]
>
>Si vous ne voyez pas &quot;Répondre&quot; comme valeur, ajoutez-la en cliquant sur **Nouveau**. &quot;Reply&quot; n’est pas une valeur standard dans Salesforce.

>[!MORELIKETHIS]
>
>* [ Connexion des attributs d’activité de vente à Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Configurer la personnalisation des détails de l’activité Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Synchroniser les activités de vente avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
