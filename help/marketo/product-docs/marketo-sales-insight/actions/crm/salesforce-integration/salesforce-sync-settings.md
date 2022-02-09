---
description: Paramètres de synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Paramètres de synchronisation Salesforce
hide: true
hidefromtoc: true
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: acb077e9d6e9fa4027d660ee182a13820f16ad83
workflow-type: tm+mt
source-wordcount: '443'
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

1. Cliquez sur le bouton **Paramètres de synchronisation** .

   ![](assets/salesforce-sync-settings-3.png)

1. Cliquez sur la flèche en regard de Log Email Activity to Salesforce (Enregistrer l’activité de courrier électronique dans Salesforce).

   ![](assets/salesforce-sync-settings-4.png)

1. Cliquez sur le bouton **API Salesforce** . Dans cette carte, vous pouvez définir vos préférences pour consigner les informations dans Salesforce. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/salesforce-sync-settings-5.png)

## Connexion de l’activité de courrier électronique à Salesforce par courrier électronique à Salesforce (Cci) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Une fois que vous avez activé &quot;E-mail à Salesforce (Cci)&quot;, vous recevrez un Cci de vos e-mails de vente et vos e-mails seront consignés comme des activités sur les opportunités, les pistes et les contacts.

>[!PREREQUISITES]
>
>Les actions Salesforce et Sales Insight doivent être connectées.

**Pour consigner vos emails dans Salesforce par courrier électronique (Cci)**

1. Dans Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/salesforce-sync-settings-6.png)

1. Sous Paramètres d’administration (ou &quot;Mon compte&quot; si vous n’êtes pas administrateur), cliquez sur **Salesforce**.

   ![](assets/salesforce-sync-settings-7.png)

1. Cliquez sur le bouton **Paramètres de synchronisation** .

   ![](assets/salesforce-sync-settings-8.png)

1. Cliquez sur le bouton **Courriel à Salesforce (Cci)** et cliquez sur **Activer**.

   ![](assets/salesforce-sync-settings-9.png)

Si, pour une raison quelconque, l’adresse Email to Salesforce ne s’affiche pas, procédez comme suit pour activer la fonctionnalité Cci dans votre compte Salesforce :

1. Connectez-vous à votre instance Salesforce.
1. Recherchez votre nom d’utilisateur dans le coin supérieur droit et sélectionnez la barre déroulante.
1. Sélectionner **Mes paramètres**.
1. Sélectionner **Email**.
1. Sélectionner **Mon courrier électronique à Salesforce**.
1. Sur cette page, un champ intitulé &quot;Adresse électronique à Salesforce&quot; s’affiche. Si rien n’est renseigné à côté de celui-ci, faites défiler l’écran jusqu’à &quot;Mes adresses électroniques acceptables&quot;.
1. Entrez la ou les adresses électroniques auxquelles vous souhaitez obtenir une copie carbone invisible (Cci).
1. Cliquez sur **Enregistrer les modifications**.

**Impossible de trouver mon courrier électronique à Salesforce dans mes paramètres**

Si vous ne voyez pas Mon courrier électronique à Salesforce sous vos paramètres, il se peut que votre administrateur ne l’ait pas activé. Cela peut se produire si votre équipe est novice à Salesforce, ou si elle n’a jamais utilisé l’adresse Cci fournie par Salesforce.

>[!NOTE]
>
>Vous aurez besoin des privilèges d’administrateur pour configurer cette configuration.

1. Cliquez sur **Configuration**.
1. Cliquez sur **Administration des emails**.
1. Cliquez sur **Courrier électronique à Salesforce**.
1. Cliquez sur **Modifier**.
1. Cochez la case en regard de &quot;Principal&quot;.
1. Cliquez sur **Enregistrer**.

## Synchroniser les tâches/rappels des actions Sales Insight avec les tâches Salesforce {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Dans Actions Sales Insight, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/salesforce-sync-settings-10.png)

1. Sous Paramètres d’administration (ou &quot;Mon compte&quot; si vous n’êtes pas administrateur), cliquez sur **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. Cliquez sur le bouton **Paramètres de synchronisation** .

   ![](assets/salesforce-sync-settings-12.png)

1. Cliquez sur la flèche en regard de Synchroniser les tâches/rappels de ventes Marketo avec les tâches Salesforce.

   ![](assets/salesforce-sync-settings-13.png)

1. Choisissez l’option souhaitée (&quot;Ne pas synchroniser avec les tâches Salesforce&quot; est sélectionné par défaut).

   ![](assets/salesforce-sync-settings-14.png)
