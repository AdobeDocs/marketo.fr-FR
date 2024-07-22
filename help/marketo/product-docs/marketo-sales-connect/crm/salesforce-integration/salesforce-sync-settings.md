---
unique-page-id: 18317669
description: Paramètres de synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Paramètres de synchronisation Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 4%

---

# Paramètres de synchronisation Salesforce {#salesforce-sync-settings}

## Connexion de l’activité de courrier électronique à Salesforce via l’API {#logging-email-activity-to-salesforce-via-api}

Cette fonctionnalité nécessite que vous soyez dans l’édition Enterprise/Illimité de Salesforce ou l’édition Professionnelle si vous avez acheté l’intégration via l’API des services Web.

>[!PREREQUISITES]
>
>Salesforce et Sales Connect doivent être connectés.

1. Dans Sales Connect, cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **Paramètres**.

   ![](assets/one-2.png)

1. Sous Mon compte (paramètres d’administration si vous êtes administrateur), cliquez sur **Salesforce**.

   ![](assets/two-2.png)

1. Cliquez sur l’onglet **Paramètres de synchronisation** .

   ![](assets/three-1.png)

1. Cliquez sur la flèche en regard de Log Email Activity to Salesforce (Enregistrer l’activité de courrier électronique dans Salesforce).

   ![](assets/four-1.png)

1. Cliquez sur l’onglet **API Salesforce** . Dans cette carte, vous pouvez définir vos préférences pour consigner les informations dans Salesforce. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/five.png)

## Connexion de l’activité de courrier électronique à Salesforce par courrier électronique à Salesforce (Cci) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Une fois que vous avez activé &quot;E-mail à Salesforce (Cci)&quot;, vous recevrez un Cci de vos e-mails de vente et vos e-mails seront consignés comme des activités sur les opportunités, les pistes et les contacts.

>[!PREREQUISITES]
>
>Salesforce et Sales Connect doivent être connectés.

**Pour consigner vos emails dans Salesforce par courrier électronique (Cci)**

1. Dans Sales Connect, cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **Paramètres**.

   ![](assets/one-3.png)

1. Sous Mon compte (paramètres d’administration si vous êtes administrateur), cliquez sur **Salesforce**.

   ![](assets/two-3.png)

1. Cliquez sur l’onglet **Paramètres de synchronisation** .

   ![](assets/three-1.png)

1. Cliquez sur l&#39;onglet **Email to Salesforce (BCC)** et cliquez sur **Activer**.

   ![](assets/six-2.png)

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

## Synchroniser les tâches/rappels Sales Connect avec les tâches Salesforce {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **Paramètres**.

   ![](assets/one-3.png)

1. Sous Mon compte (paramètres d’administration si vous êtes administrateur), cliquez sur **Salesforce**.

   ![](assets/two-2.png)

1. Cliquez sur l’onglet **Paramètres de synchronisation** .

   ![](assets/three-1.png)

1. Cliquez sur la flèche en regard de Synchroniser les tâches/rappels de connexion des ventes avec les tâches Salesforce.

   ![](assets/seven-2.png)

1. Choisissez l’option souhaitée (&quot;Ne pas synchroniser avec les tâches Salesforce&quot; est sélectionné par défaut).

   ![](assets/eight.png)
