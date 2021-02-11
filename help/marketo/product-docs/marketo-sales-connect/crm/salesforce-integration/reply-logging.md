---
unique-page-id: 14352480
description: Journalisation des réponses (SFDC) - Documents marketing - Documentation du produit
title: Journalisation des réponses (SFDC)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Journalisation des réponses (SFDC) {#reply-logging-sfdc}

Sales Connect vous permet de consigner automatiquement les réponses de vos prospects à Salesforce. La structure qui vous permet de faire cela est basée sur notre suivi des réponses par courrier électronique. Si nous pouvons suivre la réponse d&#39;une prospect, nous pouvons consigner cette réponse à Salesforce.

## Exigences {#requirements}

* doit consigner les courriers électroniques par le biais de la journalisation des API.
* Doit être en mesure de [suivre une réponse](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Doit être connecté à Salesforce
* Salesforce [appels d&#39;API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) doit être disponible

## Activer la journalisation des réponses {#enable-reply-logging}

1. Pour activer la journalisation des réponses, vous pouvez passer à la page des paramètres de Salesforce. Une fois la journalisation de l&#39;API désactivée, vous pouvez vérifier _Log Réponses_.

   >[!NOTE]
   >
   >La journalisation des réponses suit les mêmes règles que celles en vigueur pour la journalisation des courriers électroniques envoyés. notamment la manière dont les courriers électroniques sont consignés ; aux dirigeants et aux contacts ; lorsqu&#39;il y a un dossier de duplicata; si aucun enregistrement correspondant n&#39;est trouvé.

## Définition du type sur Répondre dans Salesforce {#setting-type-to-reply-in-salesforce}

Il est important d&#39;obtenir des données significatives à partir de vos rapports Salesforce. La possibilité de renseigner le champ Type sous la forme &quot;Répondre&quot; vous permet d&#39;obtenir ces données dans vos rapports. Associez-vous à votre `Salesforce admin` pour obtenir cette configuration.

1. Accédez à **Configuration** > **Personnaliser** > **Activités** > **Champs de Tâche**.
1. Cliquez sur **Type**.
1. Sous Valeurs de liste de sélection de type de Tâche, cliquez sur **Nouveau**.
1. Tapez &quot;Répondre&quot; dans la zone vide. Assurez-vous de mettre la valeur &quot;R&quot; en majuscule et cliquez sur **Enregistrer**.

   >[!NOTE]
   >
   >Il n’est pas nécessaire de sélectionner une valeur par défaut dans la liste de sélection Type. Sales Connect verra que ce type d&#39;Activité est disponible dans votre instance Salesforce et renseignera le champ tâche de vos activités entrantes en conséquence.
