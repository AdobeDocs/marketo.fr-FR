---
unique-page-id: 18317669
description: Paramètres De Synchronisation De Salesforce - Documentation De Marketo - Documentation Du Produit
title: Paramètres de synchronisation Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 3%

---

# Paramètres de synchronisation Salesforce {#salesforce-sync-settings}

## Journalisation de l’activité E-mail dans Salesforce via l’API {#logging-email-activity-to-salesforce-via-api}

Cette fonctionnalité nécessite que vous utilisiez l’édition Enterprise/Unlimited de Salesforce ou l’édition Professional si vous avez acheté Integration via l’API Web Services.

>[!PREREQUISITES]
>
>Salesforce et Sales Connect doivent être connectés.

1. Dans [!DNL Sales Connect], cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/one-2.png)

1. Sous [!UICONTROL Mon compte] ([!UICONTROL Paramètres d’administration] si vous êtes administrateur), cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Paramètres de synchronisation]**.

   ![](assets/three-1.png)

1. Cliquez sur la flèche en regard de Consigner l’activité d’e-mail à [!DNL Salesforce].

   ![](assets/four-1.png)

1. Cliquez sur l’onglet **[!UICONTROL API Salesforce]**. Dans cette carte, vous pouvez configurer vos préférences de journalisation des informations vers [!DNL Salesforce]. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/five.png)

## Consignation de l’activité E-mail dans Salesforce via E-mail vers Salesforce (Cci) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Une fois que vous avez activé « E-mail à Salesforce (Cci) », vous recevez un Cci de vos e-mails de vente et vos e-mails sont consignés en tant qu’activités sur les opportunités, les prospects et les contacts.

>[!PREREQUISITES]
>
>[!DNL Salesforce] et [!DNL Sales Connect] doivent être connectés.

**Pour consigner vos e-mails dans Salesforce via E-mail (Cci)**

1. Dans [!UICONTROL Connexion des ventes], cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/one-3.png)

1. Sous [!UICONTROL Mon compte] ([!UICONTROL Paramètres d’administration] si vous êtes administrateur), cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/two-3.png)

1. Cliquez sur l’onglet **[!UICONTROL Paramètres de synchronisation]**.

   ![](assets/three-1.png)

1. Cliquez sur l’onglet **[!UICONTROL E-mail à Salesforce (Cci)]** puis sur **[!UICONTROL Activer]**.

   ![](assets/six-2.png)

Si, pour une raison quelconque, votre adresse e-mail à [!DNL Salesforce] n’est pas retirée, procédez comme suit pour activer la fonctionnalité Cci dans votre compte [!DNL Salesforce] :

1. Connectez-vous à votre instance [!DNL Salesforce].
1. Recherchez votre nom d’utilisateur dans le coin supérieur droit et sélectionnez la barre déroulante.
1. Sélectionnez **[!UICONTROL Mes paramètres]**.
1. Sélectionnez **[!UICONTROL E-mail]**.
1. Sélectionnez **[!UICONTROL Mon e-mail à Salesforce]**.
1. Sur cette page, un champ intitulé « E-mail à l’adresse Salesforce » s’affiche. Si aucun champ n’est renseigné en regard de celui-ci, faites défiler l’écran jusqu’à « Mes adresses électroniques acceptables ».
1. Saisissez la ou les adresses e-mail à utiliser en Cci.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

**Impossible de trouver mon adresse e-mail à [!DNL Salesforce] dans Mes paramètres**

Si vous ne voyez pas Mon e-mail à Salesforce sous vos paramètres, c’est peut-être que votre administrateur ne l’a pas activé. Cela peut se produire si votre équipe est nouvelle sur [!DNL Salesforce] ou si elle n’a jamais utilisé l’adresse en Cci fournie par [!DNL Salesforce].

>[!NOTE]
>
>Pour configurer ce paramètre, vous aurez besoin de droits d’administrateur.

1. Cliquez sur **[!UICONTROL Configurer]**.
1. Cliquez sur **[!UICONTROL Administration des e-mails]**.
1. Cliquez sur **[!UICONTROL Envoyer par e-mail à Salesforce]**.
1. Cliquez sur **[!UICONTROL Modifier]**.
1. Cochez la case en regard de « [!UICONTROL Actif] ».
1. Cliquez sur **[!UICONTROL Enregistrer]**

## Synchroniser les tâches/rappels Sales Connect avec les tâches [!DNL Salesforce] {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/one-3.png)

1. Sous [!UICONTROL Mon compte] ([!UICONTROL Paramètres d’administration] si vous êtes administrateur), cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Paramètres de synchronisation]**.

   ![](assets/three-1.png)

1. Cliquez sur la flèche en regard de [!UICONTROL Synchroniser les tâches/rappels de Sales Engage avec les tâches Salesforce].

   ![](assets/seven-2.png)

1. Choisissez l’option souhaitée (la case « [!UICONTROL &#x200B; Ne pas synchroniser avec les tâches Salesforce &#x200B;] est sélectionnée par défaut).

   ![](assets/eight.png)
