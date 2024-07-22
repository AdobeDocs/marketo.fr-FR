---
unique-page-id: 14352480
description: Journalisation des réponses (SFDC) - Documents Marketo - Documentation du produit
title: Journalisation des réponses (SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Journalisation des réponses (SFDC) {#reply-logging-sfdc}

Sales Connect vous permet de consigner automatiquement les réponses de vos prospects dans Salesforce. La structure qui vous permet de le faire est basée sur notre suivi des réponses par email. Si nous pouvons suivre la réponse d’un prospect, nous pouvons enregistrer cette réponse à Salesforce.

## Exigences {#requirements}

* Doit consigner les emails via la journalisation de l’API
* Doit être en mesure de [suivre une réponse](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Doit être connecté à Salesforce
* Salesforce [ appels API ](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) doivent être disponibles

## Activation de la journalisation des réponses {#enable-reply-logging}

1. Pour activer la journalisation des réponses, vous pouvez passer à la page des paramètres Salesforce. Une fois la journalisation de l’API désactivée, vous verrez l’option permettant de cocher _Log Replies_.

   >[!NOTE]
   >
   >La journalisation des réponses suit les mêmes règles que celles que vous avez mises en place pour consigner les emails envoyés. Cela inclut la façon dont les emails sont consignés ; aux Leads et aux contacts ; en cas d’enregistrement en double ; si aucun enregistrement correspondant n’est trouvé.

## Définition du type pour répondre dans Salesforce {#setting-type-to-reply-in-salesforce}

Il est important d’obtenir des données significatives à partir de vos rapports Salesforce. La possibilité de renseigner le champ Type en tant que &quot;Répondre&quot; vous permet d’obtenir ces données par le biais de vos rapports. Associez-vous à votre `Salesforce admin` pour obtenir cette configuration.

1. Accédez à **Configuration** > **Personnaliser** > **Activités** > **Champs de la tâche**.
1. Cliquez sur **Type**.
1. Sous Tâche Type Picklist Values, cliquez sur **New**.
1. Saisissez &quot;Répondre&quot; dans la zone vide. Assurez-vous de mettre la &quot;R&quot; en majuscule et cliquez sur **Enregistrer**.

   >[!NOTE]
   >
   >Il n’est pas nécessaire de sélectionner une valeur par défaut dans la liste de sélection Type . Sales Connect verra que ce type d’activité est disponible dans votre instance Salesforce et renseigne le champ de tâche sur vos activités entrantes en conséquence.
