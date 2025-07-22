---
unique-page-id: 14352480
description: Journalisation Des Réponses (SFDC) - Documents Marketo - Documentation Du Produit
title: Journalisation des réponses (SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Journalisation des réponses (SFDC) {#reply-logging-sfdc}

Sales Connect vous offre la possibilité de consigner automatiquement les réponses de vos prospects à Salesforce. La structure qui vous permet de le faire est basée sur notre suivi des réponses aux e-mails. Si nous pouvons suivre la réponse d’un prospect, nous pouvons consigner cette réponse dans Salesforce.

## Exigences {#requirements}

* Doit consigner les e-mails via la journalisation de l’API
* Doit pouvoir [suivre une réponse](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Doit être connecté à [!DNL Salesforce]
* [!DNL Salesforce] [appels API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) doit être disponible

## Activer la journalisation des réponses {#enable-reply-logging}

1. Pour activer la journalisation des réponses, vous pouvez accéder à la page des paramètres de [!DNL Salesforce]. Une fois la journalisation de l’API cochée, l’option permettant de vérifier _Consigner les réponses_ s’affiche.

   >[!NOTE]
   >
   >La journalisation des réponses suit les mêmes règles que celles en place pour la journalisation des e-mails envoyés. Cela inclut la manière dont les e-mails sont consignés ; dans les leads et contacts ; lorsqu’il existe un enregistrement en double ; si aucun enregistrement correspondant n’est trouvé.

## Définition du type de réponse dans [!DNL Salesforce] {#setting-type-to-reply-in-salesforce}

Il est important d’obtenir des données significatives à partir de vos rapports [!DNL Salesforce]. La possibilité de renseigner le champ Type en tant que « Réponse » vous permet d’obtenir ces données par le biais de vos rapports. Faites équipe avec votre `[!DNL Salesforce] admin` pour obtenir cette configuration.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Personnaliser]** > **[!UICONTROL Activités]** > **[!UICONTROL Champs de tâche]**.
1. Cliquez sur **[!UICONTROL Type]**.
1. Sous Valeurs de la liste de sélection du type de tâche, cliquez sur **[!UICONTROL Nouveau]**.
1. Saisissez « Répondre » dans la zone vide. Veillez à mettre le caractère « R » en majuscules et à cliquer sur **[!UICONTROL Enregistrer]**.

   >[!NOTE]
   >
   >Il n’est pas nécessaire de sélectionner une valeur par défaut dans la liste de sélection Type. [!DNL Sales Connect] verrez que ce type d’activité est disponible dans votre instance [!DNL Salesforce] et renseignez le champ de tâche sur vos activités entrantes en conséquence.
