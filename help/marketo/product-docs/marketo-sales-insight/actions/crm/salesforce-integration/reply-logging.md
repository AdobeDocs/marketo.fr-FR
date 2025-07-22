---
description: Journalisation Des Réponses - Documents Marketo - Documentation Du Produit
title: Journalisation des réponses
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Journalisation des réponses {#reply-logging}

Les actions Sales Insight vous offrent la possibilité de consigner automatiquement les réponses de vos prospects aux [!DNL Salesforce]. La structure qui vous permet de le faire est basée sur notre suivi des réponses aux e-mails. Si nous pouvons suivre la réponse d’un prospect, nous pouvons consigner cette réponse dans le fichier [!DNL Salesforce].

## Exigences {#requirements}

* Doit consigner les e-mails via la journalisation de l’API
* Doit pouvoir [suivre une réponse](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
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
1. Sous [!UICONTROL Valeurs de la liste de sélection du type de tâche], cliquez sur **[!UICONTROL Nouveau]**.
1. Saisissez « Répondre » dans la zone vide. Veillez à mettre le caractère « R » en majuscules et à cliquer sur **[!UICONTROL Enregistrer]**.

   >[!NOTE]
   >
   >Il n’est pas nécessaire de sélectionner une valeur par défaut dans la liste de sélection Type. [!DNL Sales Insight Actions] verrez que ce type d’activité est disponible dans votre instance [!DNL Salesforce] et renseignez le champ de tâche sur vos activités entrantes en conséquence.
