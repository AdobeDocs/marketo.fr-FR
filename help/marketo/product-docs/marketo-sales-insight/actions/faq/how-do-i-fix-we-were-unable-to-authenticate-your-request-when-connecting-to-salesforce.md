---
description: Comment résoudre le problème "Nous n’avons pas pu authentifier votre requête" lors de la connexion à Salesforce - Documents Marketo - Documentation du produit
title: Comment résoudre le problème "Nous n’avons pas pu authentifier votre requête" lors de la connexion à Salesforce
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 0899b8cf9c97953d7212e79164d26d2f42dfeb23
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Comment résoudre le problème &quot;Nous n’avons pas pu authentifier votre requête&quot; lors de la connexion à Salesforce {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Si vous tentez de connecter votre instance Marketo Sales à Salesforce et que l’erreur &quot;Nous ne parvenons pas à authentifier votre demande&quot; s’affiche, cela est probablement lié à la manière dont votre instance Salesforce est configurée.

Deux types d’erreurs peuvent générer cette page d’authentification en échec.

* Erreur de connexion Domaine restreint
* Application Oauth bloquée

Vous pouvez identifier le type obtenu en vérifiant l’URL.

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## Résoudre l’erreur de connexion Domaine restreint {#resolve-login-error-restricted-domain}

Cette erreur indique généralement que vous disposez d’un domaine personnalisé vers lequel nous ne sommes pas en mesure de router. Pour résoudre cette erreur, essayez de vous connecter en premier à l’instance Salesforce à laquelle vous souhaitez vous connecter. Ensuite, suivez les étapes pour vous connecter à Salesforce.

Si l’instance à laquelle vous essayez de vous connecter est un domaine Salesforce Sandbox et que vous obtenez une erreur, vous devrez passer par d’autres étapes pour mettre à jour votre instance afin d’être compatible avec Salesforce Sandbox. [En savoir plus](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}.

## Résoudre l’application Oauth bloquée {#resolve-oauth-app-blocked}

Si vous avez reçu le message d’erreur &quot;Nous n’avons pas pu authentifier votre demande&quot; avec le type d’erreur Oauth App Blocked (ou un autre type) dans l’URL, il se peut qu’une restriction s’applique à votre accès à l’API de Salesforce. Vérifiez auprès de votre administrateur Salesforce que les éléments ci-dessous sont bien en place.

### Activation de l’API dans les autorisations d’utilisateur {#enable-api-in-user-permissions}

1. Demandez à un administrateur Salesforce de se connecter à Salesforce.
1. Sélectionner **Configuration**.
1. Sélectionner **Gestion des utilisateurs**.
1. Sélectionner **Profils**.
1. Recherchez le profil sous lequel se trouvent les utilisateurs ToutApp et cliquez sur **Modifier**.
1. Faites défiler jusqu’à **Autorisations administratives** et assurez-vous de **API activée** est cochée.

### Vérifiez si Salesforce bloque les actions Sales Insight de la connexion {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Demandez à un administrateur Salesforce de se connecter à Salesforce.
1. Sélectionner **Configuration**.
1. Sélectionner **Gestion des applications**.
1. Sélectionner **Utilisation des applications connectées OAuth**.
1. Assurez-vous que les actions d’aperçu des ventes affichent &quot;Bloc&quot; à côté de celui-ci. Si &quot;Débloquer&quot; s’affiche, cliquez sur le bouton pour débloquer l’accès des actions Sales Insight à Salesforce.
