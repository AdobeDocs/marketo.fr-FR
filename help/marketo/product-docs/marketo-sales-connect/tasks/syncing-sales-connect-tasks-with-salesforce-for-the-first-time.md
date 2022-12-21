---
unique-page-id: 14352541
description: Synchronisation des tâches Sales Connect avec Salesforce pour la première fois - Documents Marketo - Documentation du produit
title: Synchronisation des tâches Sales Connect avec Salesforce pour la première fois
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Synchronisation des tâches Sales Connect avec Salesforce pour la première fois {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Lorsque vous activez la synchronisation pour la première fois entre les tâches Sales Connect et Salesforce, nous importons vos tâches Salesforce. Nous allons **not** Passez en revue toutes les tâches en cours dans Sales Connect à Salesforce. Pour réduire l’encombrement et les doublons, les seules tâches synchronisées de Sales Connect dans Salesforce sont les tâches créées. *after* Vous synchronisez Sales Connect avec SFDC.

Voici ce qui se passe lorsque vous synchronisez les tâches Sales Connect et SFDC :

- Dès que vous cliquez sur Enregistrer lors de la synchronisation des tâches, elles commencent à se synchroniser. Cela prendra du temps au départ.

- Les rappels qui ont été mis à jour ou créés au cours des dernières 24 heures seront extraits de SFDC vers Sales Connect. La synchronisation est basée sur l’échéance et toutes ces tâches seront synchronisées sur le serveur principal. Toutefois, dans le Centre de commandes, seules les tâches prévues aujourd’hui et demain seront visibles.

- Si la synchronisation a été activée précédemment et que vous supprimez des tâches dans SFDC, tout ce qui a été supprimé au cours des 15 derniers jours sera supprimé du Centre de commandes.

- Nous synchroniserons constamment les tâches entre Sales Connect et SFDC tant que la synchronisation est activée.

Après la synchronisation initiale, toutes les tâches que vous créez, modifiez, terminez ou supprimez dans Sales Connect se synchroniseront avec votre liste de tâches dans Salesforce. Et tout élément créé, modifié, terminé ou supprimé dans Salesforce mettra à jour votre liste de tâches dans Sales Connect.

Pour activer cette synchronisation, cochez simplement la case de synchronisation dans votre [Page Paramètres](https://toutapp.com/login) dans l’application web.
