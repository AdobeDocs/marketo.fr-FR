---
description: Paramètres De Synchronisation De Salesforce - Documentation De Marketo - Documentation Du Produit
title: Paramètres de synchronisation Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 1%

---

# Paramètres de synchronisation [!DNL Salesforce] {#salesforce-sync-settings}

## Journalisation de l’activité E-mail vers [!DNL Salesforce] via l’API {#logging-email-activity-to-salesforce-via-api}

Cette fonctionnalité nécessite que vous soyez dans l’édition Enterprise/Unlimited de [!DNL Salesforce], ou dans l’édition Professional si vous avez acheté Integration via l’API Web Services.

>[!PREREQUISITES]
>
>[!DNL Salesforce] et [!DNL Sales Insight Actions] doivent être connectés.

1. Dans [!DNL Sales Insight Actions], cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/salesforce-sync-settings-1.png)

1. Sous [!UICONTROL Paramètres d’administration] (ou « [!UICONTROL &#x200B; Mon compte &#x200B;] » si vous n’êtes pas administrateur), cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Paramètres de synchronisation]**.

   ![](assets/salesforce-sync-settings-3.png)

1. Cliquez sur la flèche en regard de [!UICONTROL Consigner l’activité d’e-mail] pour [!DNL Salesforce].

   ![](assets/salesforce-sync-settings-4.png)

1. Cliquez sur l’onglet **[!UICONTROL API Salesforce]**. Dans cette carte, vous pouvez configurer vos préférences de journalisation des informations vers [!DNL Salesforce]. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/salesforce-sync-settings-5.png)

## Consignation de l’activité E-mail à [!DNL Salesforce] via E-mail à [!DNL Salesforce] (Cci) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Une fois que vous avez activé « [!UICONTROL E-mail à Salesforce (Cci)] », vous recevez un Cci de vos e-mails de vente et vos e-mails sont consignés en tant qu’activités sur les opportunités, les prospects et les contacts.

>[!PREREQUISITES]
>
>[!DNL Salesforce] et [!DNL Sales Insight Actions] doivent être connectés.

**Pour consigner vos e-mails dans [!DNL Salesforce] par e-mail (Cci)**

1. Dans Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/salesforce-sync-settings-6.png)

1. Sous [!UICONTROL Paramètres d’administration] (ou « [!UICONTROL &#x200B; Mon compte &#x200B;] » si vous n’êtes pas administrateur), cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-7.png)

1. Cliquez sur l’onglet **[!UICONTROL Paramètres de synchronisation]**.

   ![](assets/salesforce-sync-settings-8.png)

1. Cliquez sur l’onglet **[!UICONTROL E-mail à Salesforce (Cci)]** puis sur **[!UICONTROL Activer]**.

   ![](assets/salesforce-sync-settings-9.png)

Si, pour une raison quelconque, votre adresse e-mail à [!DNL Salesforce] n’est pas retirée, procédez comme suit pour activer la fonctionnalité Cci dans votre compte [!DNL Salesforce] :

1. Connectez-vous à votre instance [!DNL Salesforce].
1. Recherchez votre nom d’utilisateur dans le coin supérieur droit et sélectionnez la barre déroulante.
1. Sélectionnez **[!UICONTROL Mes paramètres]**.
1. Sélectionnez **[!UICONTROL E-mail]**.
1. Sélectionnez **[!UICONTROL Mon e-mail à Salesforce]**.
1. Sur cette page, un champ intitulé « [!UICONTROL E-mail à l’adresse Salesforce] s’affiche. » Si aucun champ n’est renseigné en regard de celui-ci, faites défiler l’écran jusqu’à « [!UICONTROL Mes adresses e-mail acceptables] ».
1. Saisissez la ou les adresses e-mail à utiliser en Cci.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

**Impossible de trouver mon adresse e-mail à [!DNL Salesforce] dans Mes paramètres**

Si vous ne voyez pas Mon e-mail à [!DNL Salesforce] sous vos paramètres, il se peut que votre administrateur ne l’ait pas activé. Cela peut se produire si votre équipe est nouvelle sur [!DNL Salesforce] ou si elle n’a jamais utilisé l’adresse en Cci fournie par [!DNL Salesforce].

>[!NOTE]
>
>Pour configurer ce paramètre, vous aurez besoin de droits d’administrateur.

1. Cliquez sur **[!UICONTROL Configurer]**.
1. Cliquez sur **[!UICONTROL Administration des e-mails]**.
1. Cliquez sur **[!UICONTROL Envoyer par e-mail à Salesforce]**.
1. Cliquez sur **[!UICONTROL Modifier]**.
1. Cochez la case en regard de « Actif ».
1. Cliquez sur **[!UICONTROL Enregistrer]**.

## Synchroniser [!DNL Sales Insight Actions] tâches/rappels avec [!DNL Salesforce] tâches {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Dans [!DNL Sales Insight Actions], cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/salesforce-sync-settings-10.png)

1. Sous [!UICONTROL Paramètres d’administration] (ou « [!UICONTROL &#x200B; Mon compte &#x200B;] » si vous n’êtes pas administrateur), cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-11.png)

1. Cliquez sur l’onglet **[!UICONTROL Paramètres de synchronisation]**.

   ![](assets/salesforce-sync-settings-12.png)

1. Cliquez sur la flèche en regard de Synchroniser les tâches de vente/rappels Marketo pour [!DNL Salesforce] les tâches.

   ![](assets/salesforce-sync-settings-13.png)

1. Sélectionnez l’option souhaitée (l’option « Ne pas synchroniser avec [!DNL Salesforce] tâches » est sélectionnée par défaut).

   ![](assets/salesforce-sync-settings-14.png)

## Première synchronisation de tâches [!DNL Sales Insight Actions] avec [!DNL Salesforce] {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Lorsque vous activez pour la première fois la synchronisation entre les tâches [!DNL Sales Insight Actions] et [!DNL Salesforce], nous importons vos tâches [!DNL Salesforce]. Nous ne transmettrons pas les tâches en cours que vous avez en [!DNL Sales Insight Actions] à [!DNL Salesforce]. Pour réduire l’encombrement et les doublons, les seules tâches synchronisées à partir de [!DNL Sales Insight Actions] dans [!DNL Salesforce] sont les tâches créées après la synchronisation de [!DNL Sales Insight Actions] avec SFDC.

Voici ce qui se produit lorsque vous synchronisez les tâches [!DNL Sales Insight Actions] et SFDC :

Dès que vous cliquez sur Enregistrer sur les tâches en cours de synchronisation, elles commencent à se synchroniser. Cela prendra un certain temps au début.

Tous les rappels qui ont été mis à jour ou créés au cours des dernières 24 heures seront extraits de SFDC vers [!DNL Sales Insight Actions]. La synchronisation est basée sur la date d’échéance et toutes ces tâches seront synchronisées en arrière-plan, mais dans le centre de commande, vous ne verrez que les tâches dues aujourd’hui et demain.

Si la synchronisation a été activée précédemment et que vous supprimez des tâches dans SFDC, tout ce qui a été supprimé au cours des 15 derniers jours sera supprimé du Centre de commande.

Nous synchroniserons constamment les tâches entre [!DNL Sales Insight Actions] et SFDC tant que la synchronisation est activée.

Après la synchronisation initiale, toutes les tâches que vous créez, modifiez, terminez ou supprimez dans [!DNL Sales Insight Actions] seront synchronisées avec votre liste de tâches dans [!DNL Salesforce]. Et tout ce qui sera créé, modifié, terminé ou supprimé dans [!DNL Salesforce] mettra à jour votre liste de tâches dans [!DNL Sales Insight Actions].

Pour activer cette synchronisation, cochez simplement la case de synchronisation dans votre page [!UICONTROL Paramètres] de l’application web.
