---
unique-page-id: 14352484
description: Comment corriger "Nous n’avons pas pu authentifier votre requête" lors de la connexion à Salesforce - Documents Marketo - Documentation du produit
title: Comment corriger "Nous n’avons pas pu authentifier votre requête" lors de la connexion à Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Comment corriger &quot;Nous n’avons pas pu authentifier votre requête&quot; lors de la connexion à Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si vous recevez le message d’erreur &quot;Nous n’avons pas pu authentifier votre demande&quot; lors de la tentative de connexion des ventes à Salesforce, il se peut qu’il y ait une restriction de votre accès à l’API de Salesforce. Vérifiez auprès de votre administrateur Salesforce que les éléments suivants sont bien en place.

## Activation de l’API dans les autorisations d’utilisateur {#enable-api-in-user-permissions}

1. Demandez à un administrateur Salesforce de se connecter à SFDC.
1. Sélectionnez **Configuration**.
1. Sélectionnez **Gérer les utilisateurs**.
1. Sélectionnez **Profils**.
1. Recherchez le profil sous lequel se trouvent les utilisateurs ToutApp et cliquez sur **Modifier**.
1. Faites défiler l’écran jusqu’à **Autorisations administratives** et assurez-vous que l’option **API activée** est cochée.

## Vérifiez si Salesforce bloque Sales Connect de la connexion {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Demandez à un administrateur Salesforce de se connecter à SFDC.
1. Sélectionnez **Configuration**.
1. Sélectionnez **Gérer les applications**.
1. Sélectionnez **Utilisation des applications connectées OAuth**.
1. Assurez-vous que la connexion aux ventes affiche &quot;Bloc&quot; à côté de celle-ci. Si &quot;Débloquer&quot; s’affiche, cliquez sur le bouton pour débloquer l’accès de Sales Connect à Salesforce.
