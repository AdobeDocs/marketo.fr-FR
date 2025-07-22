---
unique-page-id: 14352541
description: Synchronisation des tâches de Sales Connect avec Salesforce pour la première fois - Documents Marketo - Documentation du produit
title: Synchronisation des tâches Sales Connect avec Salesforce pour la première fois
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Première synchronisation de tâches [!DNL Sales Connect] avec [!DNL Salesforce] {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Lorsque vous activez pour la première fois la synchronisation entre les tâches [!DNL Sales Connect] et [!DNL Salesforce], nous importons vos tâches [!DNL Salesforce]. Nous **transmettrons pas** tâches en cours que vous avez en [!DNL Sales Connect] à [!DNL Salesforce]. Pour réduire l’encombrement et les doublons, les seules tâches synchronisées à partir de [!DNL Sales Connect] dans [!DNL Salesforce] sont les tâches créées *après* vous synchronisez [!DNL Sales Connect] avec SFDC.

Voici ce qui se produit lorsque vous synchronisez des tâches [!DNL Sales Connect] et SFDC :

- Dès que vous cliquez sur Enregistrer sur les tâches en cours de synchronisation, elles commencent à se synchroniser. Cela prendra un certain temps au début.

- Tous les rappels qui ont été mis à jour ou créés au cours des dernières 24 heures seront extraits de SFDC vers [!DNL Sales Connect]. La synchronisation est basée sur la date d’échéance et toutes ces tâches seront synchronisées en arrière-plan, mais dans le centre de commande, vous ne verrez que les tâches dues aujourd’hui et demain.

- Si la synchronisation a été activée précédemment et que vous supprimez des tâches dans SFDC, tout ce qui a été supprimé au cours des 15 derniers jours sera supprimé du Centre de commande.

- Nous synchroniserons constamment les tâches entre [!DNL Sales Connect] et SFDC tant que la synchronisation sera activée.

Après la synchronisation initiale, toutes les tâches que vous créez, modifiez, terminez ou supprimez dans [!DNL Sales Connect] seront synchronisées avec votre liste de tâches dans [!DNL Salesforce]. Et tout ce qui sera créé, modifié, terminé ou supprimé dans [!DNL Salesforce] mettra à jour votre liste de tâches dans [!DNL Sales Connect].

Pour activer cette synchronisation, cochez simplement la case de synchronisation dans la page [Paramètres](https://toutapp.com/login) de l’application web.
