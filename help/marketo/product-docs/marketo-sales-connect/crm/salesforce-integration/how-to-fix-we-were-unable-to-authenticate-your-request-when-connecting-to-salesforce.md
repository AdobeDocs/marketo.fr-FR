---
unique-page-id: 14352484
description: Comment corriger "Nous n'avons pas pu authentifier votre demande" lors de la connexion à Salesforce - Marketo Docs - Documentation du produit
title: Comment corriger "Impossible d'authentifier votre requête" lors de la connexion à Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Comment corriger &quot;Nous n&#39;avons pas pu authentifier votre requête&quot; lors de la connexion à Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si vous recevez le message d&#39;erreur &quot;Nous n&#39;avons pas pu authentifier votre demande&quot; lors de la tentative de connexion de Sales Connect à Salesforce, il se peut qu&#39;une restriction s&#39;applique à votre accès à l&#39;API de Salesforce. Vérifiez auprès de votre administrateur Salesforce que les éléments suivants sont bien en place.

## Activer l’API dans les autorisations d’utilisateur {#enable-api-in-user-permissions}

1. Demandez à un administrateur Salesforce de se connecter à SFDC.
1. Sélectionnez **Configuration**.
1. Sélectionnez **Gérer les utilisateurs**.
1. Sélectionnez **Profils**.
1. Recherchez le Profil sous lequel se trouvent les utilisateurs de ToutApp et cliquez sur **Modifier**.
1. Faites défiler l&#39;écran jusqu&#39;à **Autorisations administratives** et vérifiez que **API activée** est cochée.

## Vérifier si Salesforce bloque la connexion des ventes de {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Demandez à un administrateur Salesforce de se connecter à SFDC.
1. Sélectionnez **Configuration**.
1. Sélectionnez **Gérer les applications**.
1. Sélectionnez **Utilisation OAuth des applications connectées**.
1. Assurez-vous que Sales Connect affiche &quot;Bloc&quot; en regard de celui-ci. Si &quot;Débloquer&quot; s&#39;affiche, cliquez sur le bouton pour débloquer l&#39;accès de Sales Connect à Salesforce.

