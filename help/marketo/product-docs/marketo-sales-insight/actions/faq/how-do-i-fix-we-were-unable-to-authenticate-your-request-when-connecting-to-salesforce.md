---
description: Comment résoudre le problème « Nous n’avons pas pu authentifier votre demande » lors de la connexion à Salesforce - Documents Marketo - Documentation du produit
title: Comment résoudre le problème « Nous n’avons pas pu authentifier votre demande » lors de la connexion à Salesforce
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Comment résoudre le problème « Nous n’avons pas pu authentifier votre demande » lors de la connexion à [!DNL Salesforce] {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si vous tentez de connecter votre instance de vente Marketo à Salesforce et que l’erreur « Nous ne parvenons pas à authentifier votre demande » s’affiche, cela est probablement lié à la configuration de votre instance Salesforce.

Deux types d’erreurs peuvent générer cette page d’authentification ayant échoué.

* Domaine restreint d&#39;erreur de connexion
* Application Oauth Bloquée

Vous pouvez identifier le type obtenu en vérifiant l’URL.

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## Résoudre l&#39;erreur de connexion Domaine restreint {#resolve-login-error-restricted-domain}

Cette erreur indique généralement que vous disposez d’un domaine personnalisé vers lequel nous ne pouvons pas effectuer le routage. Pour résoudre cette erreur, essayez d’abord de vous connecter à l’instance Salesforce à laquelle vous souhaitez vous connecter. Ensuite, suivez les étapes pour vous connecter à Salesforce.

Si l’instance à laquelle vous tentez de vous connecter est un domaine Sandbox Salesforce et que vous obtenez une erreur, vous devrez passer par des étapes supplémentaires pour mettre à jour votre instance afin qu’elle soit compatible avec Sandbox Salesforce. [En savoir plus](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}.

## Application Oauth De Résolution Bloquée {#resolve-oauth-app-blocked}

Si vous avez reçu le message d’erreur « Nous n’avons pas pu authentifier votre demande » avec le type d’erreur Application Oauth bloquée (ou un autre type) dans l’URL, il se peut qu’il y ait une restriction sur votre accès à l’API Salesforce. Vérifiez auprès de votre administrateur Salesforce que les éléments ci-dessous sont en place.

### Activer l’API dans les autorisations utilisateur {#enable-api-in-user-permissions}

1. Demandez à un administrateur Salesforce de se connecter à Salesforce.
1. Sélectionnez **Configuration**.
1. Sélectionnez **Gérer les utilisateurs**.
1. Sélectionnez **Profils**.
1. Recherchez le profil sous lequel se trouvent les utilisateurs de ToutApp et cliquez sur **Modifier**.
1. Faites défiler jusqu’à **Autorisations d’administration** et assurez-vous que **API activée** est coché.

### Vérifier si Salesforce empêche les actions Sales Insight de se connecter {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Demandez à un administrateur Salesforce de se connecter à Salesforce.
1. Sélectionnez **Configuration**.
1. Sélectionnez **Gérer Les Applications**.
1. Sélectionnez **Utilisation d’OAuth pour les applications connectées**.
1. Assurez-vous que le composant Actions de Sales Insight indique « Block » en regard de celui-ci. Si « Débloquer » s’affiche, cliquez sur le bouton pour débloquer l’accès de Sales Insight Actions à Salesforce.
