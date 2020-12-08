---
unique-page-id: 14352541
description: Synchronisation des Tâches Sales Connect avec Salesforce pour la première fois - Marketo Docs - Documentation sur les produits
title: Synchronisation des Tâches Sales Connect avec Salesforce pour la première fois
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Synchronisation des Tâches Sales Connect avec Salesforce pour la première fois {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Lorsque vous activez pour la première fois la synchronisation entre les tâches Sales Connect et Salesforce, nous importons vos tâches Salesforce. Nous **n&#39;écraserons** aucune tâche en cours dans Sales Connect to Salesforce. Pour réduire les encombrements et les duplicata, les seules tâches synchronisées de Sales Connect dans Salesforce sont les tâches créées *après* la synchronisation de Sales Connect avec SFDC.

Voici ce qui se passe lorsque vous synchronisez les tâches Sales Connect et SFDC :

- Dès que vous cliquez sur Enregistrer lors de la synchronisation des tâches, elles commencent à se synchroniser. Cela prendra un certain temps au départ.

- Tout rappel mis à jour ou créé dans le `last 24 hours` sera extrait de SFDC vers Sales Connect. La synchronisation est basée sur `due date` et toutes ces tâches seront synchronisées sur l&#39;arrière-plan, mais dans le Centre de commandes, vous ne verrez que les tâches à venir aujourd&#39;hui et demain.

- Si la synchronisation a été activée précédemment et que vous supprimez des tâches dans la collecte de données régionale, tout ce qui a été supprimé au cours des 15 derniers jours sera supprimé du Centre de commandes.

- Nous synchroniserons constamment les tâches entre Sales Connect et SFDC tant que la synchronisation sera activée.

Après la synchronisation initiale, toutes les tâches que vous créez, modifiez, terminez ou supprimez dans Sales Connect seront synchronisées avec votre liste de tâches dans Salesforce. Et tout élément créé, modifié, terminé ou supprimé dans Salesforce mettra à jour votre liste de tâches dans Sales Connect.

Pour activer cette synchronisation, il vous suffit de cocher la case de synchronisation dans la page [](http://toutapp.com/next#settings/crm/salesforce/configure) Paramètres de l’application Web.

