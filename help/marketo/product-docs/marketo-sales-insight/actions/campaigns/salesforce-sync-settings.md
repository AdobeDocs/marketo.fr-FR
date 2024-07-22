---
description: Paramètres de synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Paramètres de synchronisation Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 350490c93d8f2bcc278f9f3e82018a1db91a1146
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---

# Paramètres de synchronisation Salesforce {#salesforce-sync-settings}

## Connexion de l’activité de courrier électronique à Salesforce via l’API {#logging-email-activity-to-salesforce-via-api}

Cette fonctionnalité nécessite que vous soyez dans l’édition Enterprise/Illimité de Salesforce ou l’édition Professionnelle si vous avez acheté l’intégration via l’API des services Web.

>[!PREREQUISITES]
>
>Les actions Salesforce et Sales Insight doivent être connectées.

1. Dans Actions Sales Insight, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/salesforce-sync-settings-1.png)

1. Sous Paramètres d’administration (ou &quot;Mon compte&quot; si vous n’êtes pas administrateur), cliquez sur **Salesforce**.

   ![](assets/salesforce-sync-settings-2.png)

1. Cliquez sur l’onglet **Paramètres de synchronisation** .

   ![](assets/salesforce-sync-settings-3.png)

1. Cliquez sur la flèche en regard de Log Email Activity to Salesforce (Enregistrer l’activité de courrier électronique dans Salesforce).

   ![](assets/salesforce-sync-settings-4.png)

1. Cliquez sur l’onglet **API Salesforce** . Dans cette carte, vous pouvez définir vos préférences pour consigner les informations dans Salesforce. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/salesforce-sync-settings-5.png)

## Connexion de l’activité de courrier électronique à Salesforce par courrier électronique à Salesforce (Cci) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Une fois que vous avez activé &quot;E-mail à Salesforce (Cci)&quot;, vous recevrez un Cci de vos e-mails de vente et vos e-mails seront consignés comme des activités sur les opportunités, les pistes et les contacts.

>[!PREREQUISITES]
>
>Les actions Salesforce et Sales Insight doivent être connectées.

**Pour consigner vos emails dans Salesforce par courrier électronique (Cci)**

1. Dans Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **Settings**.

   ![](assets/salesforce-sync-settings-6.png)

1. Sous Paramètres d’administration (ou &quot;Mon compte&quot; si vous n’êtes pas administrateur), cliquez sur **Salesforce**.

   ![](assets/salesforce-sync-settings-7.png)

1. Cliquez sur l’onglet **Paramètres de synchronisation** .

   ![](assets/salesforce-sync-settings-8.png)

1. Cliquez sur l&#39;onglet **Email to Salesforce (BCC)** et cliquez sur **Activer**.

   ![](assets/salesforce-sync-settings-9.png)

Si, pour une raison quelconque, l’adresse Email to Salesforce ne s’affiche pas, procédez comme suit pour activer la fonctionnalité Cci dans votre compte Salesforce :

1. Connectez-vous à votre instance Salesforce.
1. Recherchez votre nom d’utilisateur dans le coin supérieur droit et sélectionnez la barre déroulante.
1. Sélectionnez **Mes paramètres**.
1. Sélectionnez **Email**.
1. Sélectionnez **Mon e-mail à Salesforce**.
1. Sur cette page, un champ intitulé &quot;Adresse électronique à Salesforce&quot; s’affiche. Si rien n’est renseigné à côté de celui-ci, faites défiler l’écran jusqu’à &quot;Mes adresses électroniques acceptables&quot;.
1. Entrez la ou les adresses électroniques auxquelles vous souhaitez obtenir une copie carbone invisible (Cci).
1. Cliquez sur **Enregistrer les modifications**.

**Impossible de trouver mon courrier électronique à Salesforce dans mes paramètres**

Si vous ne voyez pas Mon courrier électronique à Salesforce sous vos paramètres, votre administrateur ne l’a peut-être pas activé. Cela peut se produire si votre équipe est novice à Salesforce, ou si elle n’a jamais utilisé l’adresse Cci fournie par Salesforce.

>[!NOTE]
>
>Vous aurez besoin des privilèges d’administrateur pour configurer cette configuration.

1. Cliquez sur **Configuration**.
1. Cliquez sur **Administration des emails**.
1. Cliquez sur **E-mail à Salesforce**.
1. Cliquez sur **Modifier**.
1. Cochez la case en regard de &quot;Actif&quot;.
1. Cliquez sur **Enregistrer**.

## Synchroniser les tâches/rappels des actions Sales Insight avec les tâches Salesforce {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Dans Actions Sales Insight, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/salesforce-sync-settings-10.png)

1. Sous Paramètres d’administration (ou &quot;Mon compte&quot; si vous n’êtes pas administrateur), cliquez sur **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. Cliquez sur l’onglet **Paramètres de synchronisation** .

   ![](assets/salesforce-sync-settings-12.png)

1. Cliquez sur la flèche en regard de Synchroniser les tâches/rappels de ventes Marketo avec les tâches Salesforce.

   ![](assets/salesforce-sync-settings-13.png)

1. Choisissez l’option souhaitée (&quot;Ne pas synchroniser avec les tâches Salesforce&quot; est sélectionné par défaut).

   ![](assets/salesforce-sync-settings-14.png)

## Synchronisation des tâches d’actions Sales Insight avec Salesforce pour la première fois {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Lorsque vous activez la synchronisation pour la première fois entre les actions Sales Insight et les tâches Salesforce, nous importons vos tâches Salesforce. Nous ne transférons aucune tâche en cours dans les actions Sales Insight à Salesforce. Pour réduire les encombres et les doublons, les seules tâches qui sont synchronisées des actions Sales Insight dans Salesforce sont les tâches créées après la synchronisation des actions Sales Insight avec SFDC.

Voici ce qui se passe lorsque vous synchronisez les actions Sales Insight et les tâches SFDC :

Dès que vous cliquez sur Enregistrer lors de la synchronisation des tâches, elles commencent à se synchroniser. Cela prendra du temps au départ.

Les rappels qui ont été mis à jour ou créés au cours des dernières 24 heures seront transférés de SFDC aux actions Sales Insight . La synchronisation est basée sur l’échéance et toutes ces tâches seront synchronisées sur le serveur principal. Toutefois, dans le Centre de commandes, seules les tâches prévues aujourd’hui et demain seront visibles.

Si la synchronisation a été activée précédemment et que vous supprimez des tâches dans SFDC, tout ce qui a été supprimé au cours des 15 derniers jours sera supprimé du Centre de commandes.

Nous synchroniserons constamment les tâches entre les actions Sales Insight et SFDC tant que la synchronisation est activée.

Après la synchronisation initiale, toutes les tâches que vous créez, modifiez, terminez ou supprimez dans les actions Sales Insight se synchronisent avec votre liste de tâches dans Salesforce. De plus, tout élément créé, modifié, terminé ou supprimé dans Salesforce mettra à jour votre liste de tâches dans les actions Sales Insight.

Pour activer cette synchronisation, cochez simplement la case de synchronisation dans la page Paramètres de l’application web.
