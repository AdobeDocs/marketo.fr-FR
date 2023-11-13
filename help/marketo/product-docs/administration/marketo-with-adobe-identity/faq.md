---
description: FAQ sur Adobe Identity Management - Documentation Marketo - Documentation du produit
title: FAQ sur Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 094a11f9544e0dba75167de229d78e8ff50cf6e8
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 3%

---

# FAQ sur Adobe Identity Management {#adobe-identity-management-faq}

**Qu’est-ce que l’identité Adobe ?**

Adobe Identity Management System se compose de trois composants.

* [!DNL Adobe Identity Service]: gère l’authentification et la validation de l’utilisateur final, y compris la fédération et l’authentification unique au moment de l’exécution.

* Adobe Admin Console : le Admin Console fournit un emplacement central pour la gestion des droits d’Adobe dans l’ensemble de votre organisation. Il gère la gestion des utilisateurs, le service cloud, les droits de licence de bureau, la configuration de fédération et fournit des fonctionnalités de sécurité de prévention des pertes de données.

* API Adobe User Management (UMAPI) : permet aux entreprises de gérer les utilisateurs et les droits des entreprises dans Adobe Admin Console au niveau de l’API.

**Quand les abonnements de Marketo Engage existants seront-ils intégrés à IMS ?**

Les abonnements Marketo existants seront migrés vers le système Identity Management Adobe plus tard dans l’année. La prise en charge de Marketo ne pourra fournir aucune mise à jour concernant la migration d’Adobe IMS. L’équipe Compte d’Adobe atteindra le délai prévu au cours des prochains mois.

**Quelle est la différence entre un administrateur de produit Adobe et un administrateur de Marketo Engage ?**

* L’administrateur de produit Adobe est un nouveau rôle dans la plateforme Marketo.
* Le rôle Administrateur de produit Adobe est attribué aux utilisateurs ajoutés en tant qu’administrateur de produit dans Adobe Admin Console
* L’administrateur de produit Adobe est un rôle en lecture seule qui ne peut pas être modifié ni supprimé de Marketo Engage.
* L’administrateur de produit Adobe dispose des mêmes droits et privilèges qu’un administrateur Marketo standard.
* Le rôle d’administrateur du Marketo Engage est toujours un administrateur et est attribué à un utilisateur en Marketo Engage.

**La prise en charge des clients de l’API de gestion des utilisateurs a-t-elle changé ?**

Oui. Ceux qui ont été intégrés à Adobe IMS ne peuvent pas utiliser toutes les API de gestion des utilisateurs Marketo existantes. Pour les actions d’invitation, de mise à jour et de suppression de l’utilisateur, l’Adobe [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} doit être utilisé. Pour la gestion des rôles, les API de gestion des utilisateurs de Marketo s’appliquent toujours. En outre, aucune autre modification n’est apportée à la prise en charge des clients de l’API REST Marketo.

**Qui contacter pour obtenir de l’aide si nous sommes intégrés à IMS ?**

Vous devez suivre la procédure standard pour contacter [Prise en charge de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**Si j’utilise une identité d’Adobe pour accéder à d’autres applications d’Adobe, puis-je l’utiliser pour accéder à Marketo ?**

Même si vous disposez d’autres produits Adobe, vous ne pouvez pas accéder à Marketo avec l’Adobe Identity tant que l’abonnement n’est pas migré vers IMS.

**Les rôles utilisateur Marketo (dans les espaces de travail) sont-ils gérés dans Adobe Admin Console ?**

Non. La gestion des rôles utilisateur (dans les espaces de travail) est effectuée dans Marketo Engage.

**Je suis administrateur Marketo dans un abonnement intégré IMS et n’ai pas accès au Admin Console. Comment puis-je y accéder ?**

Tout administrateur système d’Adobe ou de produit ayant accès au Admin Console de votre entreprise peut vous donner accès. Si vous ne savez pas qui dans votre organisation dispose des privilèges d’administrateur dans la console, contactez [Adobe de l’assistance clientèle](https://helpx.adobe.com/contact.html){target="_blank"}.

**Comment un administrateur ajoute-t-il des utilisateurs à Marketo ? [!DNL Sales Connect]?**

Il y aura une carte de produit en Admin Console pour [!DNL Sales Connect], Admin Console ne doit pas être utilisé pour ajouter/gérer des utilisateurs. Le lien suivant permet aux administrateurs de gérer les utilisateurs via Marketo. [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Où puis-je en savoir plus sur Adobe Admin Console ?**

[https://helpx.adobe.com/fr/enterprise/admin-guide.html](https://helpx.adobe.com/fr/enterprise/admin-guide.html){target="_blank"}.

**Puis-je toujours accéder à la section Admin de Marketo pour apporter des modifications au compte utilisateur de mon compte ?**

Non, vous devez accéder à [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Comment cela fonctionne-t-il avec Marketo Universal ID ?**

Les personnes intégrées à l’identité Adobe peuvent accéder facilement à tous les abonnements activés pour IMS via le sélecteur d’abonnements du produit.

**Cela fonctionne-t-il avec SSO ?**

Oui. L’intégration de Marketo avec Adobe IMS prend en charge les utilisateurs d’ID universels et l’authentification unique. L’authentification unique est désormais pilotée par Adobe IMS et configurée au niveau de l’organisation dans Adobe Admin Console. [En savoir plus ici](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Comment fonctionne l’autorisation de périphérique ?**

Adobe IMS ne prend actuellement en charge rien de tel que la fonctionnalité d’autorisation des périphériques de Marketo.

**Est-il toujours possible d’utiliser la fonction &quot;Se connecter dans la boîte de dialogue d’invitation&quot; pour rendre la connexion d’un utilisateur unique à partir de son email ?**

Non. Le workflow d’invitation d’utilisateur n’est plus actif lorsqu’un abonnement est activé sur IMS. La fonctionnalité n’est donc plus valide. L’identité de l’Adobe nécessite que l’identité d’un utilisateur soit déterminée par son email.

**Pour Adobe IMS, avons-nous la possibilité d’utiliser Adobe ID, Enterprise ID ou Federated ID ?**

Oui, vous déterminez le type d’identité à prendre en charge par votre organisation. Plus d’informations sont disponibles ici : [Présentation des identités](https://helpx.adobe.com/enterprise/using/identity.html) et ici : [Configuration d’identité](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Quelles cartes de produits sont prises en charge dans Adobe Admin Console ?**

Les cartes de produits prises en charge sont les suivantes : Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect et Marketo Sales Insight Actions.
