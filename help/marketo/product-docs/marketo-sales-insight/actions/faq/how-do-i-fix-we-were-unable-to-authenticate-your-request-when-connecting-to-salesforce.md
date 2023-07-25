---
description: Comment résoudre le problème "Nous n’avons pas pu authentifier votre requête" lors de la connexion à Salesforce - Documents Marketo - Documentation du produit
title: Comment résoudre le problème "Nous n’avons pas pu authentifier votre requête" lors de la connexion à Salesforce
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Comment résoudre le problème &quot;Nous n’avons pas pu authentifier votre requête&quot; lors de la connexion à Salesforce {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si vous recevez le message d’erreur &quot;Nous n’avons pas pu authentifier votre demande&quot; lors de la tentative de connexion des actions d’aperçu des ventes à Salesforce, il se peut qu’il y ait une restriction de votre accès à l’API de Salesforce. Vérifiez auprès de votre administrateur Salesforce que les éléments suivants sont bien en place.

## Activation de l’API dans les autorisations d’utilisateur {#enable-api-in-user-permissions}

1. Demandez à un administrateur Salesforce de se connecter à SFDC.
1. Sélectionner **Configuration**.
1. Sélectionner **Gestion des utilisateurs**.
1. Sélectionner **Profils**.
1. Recherchez le profil sous lequel se trouvent les utilisateurs ToutApp et cliquez sur **Modifier**.
1. Faites défiler jusqu’à **Autorisations administratives** et assurez-vous de **API activée** est cochée.

## Vérifiez si Salesforce bloque les actions Sales Insight de la connexion {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Demandez à un administrateur Salesforce de se connecter à SFDC.
1. Sélectionner **Configuration**.
1. Sélectionner **Gestion des applications**.
1. Sélectionner **Utilisation des applications connectées OAuth**.
1. Assurez-vous que les actions d’aperçu des ventes affichent &quot;Bloc&quot; à côté. Si &quot;Débloquer&quot; s’affiche, cliquez sur le bouton pour débloquer l’accès des actions Sales Insight à Salesforce.
