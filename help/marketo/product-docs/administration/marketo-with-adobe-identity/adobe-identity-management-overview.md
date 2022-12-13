---
description: Présentation d’Adobe Identity Management - Documentation Marketo - Documentation du produit
title: Présentation d’Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 034e3a9a1e2e7feec749afe981aaaf804a4bcddc
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 0%

---

# Présentation d’Adobe Identity Management {#adobe-identity-management-overview}

Si vous disposez d’un nouveau compte avec Adobe Marketo Engage (un nouveau compte, et pas seulement une nouvelle instance pour un compte existant) à compter du 15 février 2022, il peut être intégré au système Identity Management d’Adobe, en fonction du package de produits acheté. Pour savoir si vous l’avez, contactez votre administrateur Marketo ou le responsable du succès client de votre compte.

Les abonnements Marketo existants commenceront à être migrés vers le système Identity Management Adobe au cours du second semestre 2023.

>[!NOTE]
>
>La prise en charge de Marketo ne pourra fournir aucune mise à jour concernant la migration d’Adobe IMS. Votre responsable du succès client atteindra le délai prévu au cours des prochains mois.

## Niveaux de profil {#profile-levels}

Les abonnements Adobe Marketo Engage intégrés à Adobe Identity Management System prennent en charge divers profils. Voici les types de profils utilisateur pertinents dans cette intégration.

<table>
 <tr>
  <td><strong>Administrateur système Adobe Admin Console</strong></td>
  <td>Responsable de la configuration des concepts d’identité pour l’organisation Adobe et le produit Marketo Engage dans Adobe Admin Console. Rôle attribué lors de la configuration de l’organisation d’Adobe.</td>
 </tr>
 <tr>
  <td><strong>Administrateur de produit Adobe Admin Console</strong></td>
  <td>Responsable du droit des utilisateurs au produit Marketo Engage dans Adobe Admin Console. Rôle attribué dans Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrateur de profil de produit Adobe Admin Console</strong></td>
  <td>Responsable de l’administration des utilisateurs dans un profil de produits. Ils ne peuvent pas gérer les utilisateurs en dehors de ce profil spécifique. Un administrateur de profil de produit n’a pas accès à l’application Marketo, sauf s’il a été ajouté au profil de produit en tant qu’utilisateur. Leur rôle reste un utilisateur standard (espace de travail par défaut s’il dispose de plusieurs espaces de travail).
</td>
 </tr>
 <tr>
  <td><strong>Administrateur de produit Marketo Engage</strong></td>
  <td>Personne ayant accès à un Marketo Engage avec des privilèges d’administrateur. Rôle attribué en Marketo Engage, pas en Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Utilisateur Marketo Engage</strong></td>
  <td>Personne à qui l’accès au Marketo Engage a été accordé. Aucun privilège d’administrateur.</td>
 </tr>
</table>

## FAQ {#faq}

**Qu’est-ce que l’identité Adobe ?**

Adobe Identity Management System se compose de trois composants.

* Adobe Identity Service : Gère l’authentification et la validation de l’utilisateur final, y compris la fédération et l’authentification unique au moment de l’exécution.

* Adobe Admin Console : Le Admin Console fournit un emplacement central pour la gestion des droits d’Adobe dans l’ensemble de votre organisation. Il gère la gestion des utilisateurs, le service cloud, les droits de licence de bureau, la configuration de fédération et fournit des fonctionnalités de sécurité de prévention des pertes de données.

* API de gestion des utilisateurs Adobe (UMAPI) : Permet aux entreprises de gérer les utilisateurs et les droits des entreprises dans Adobe Admin Console au niveau de l’API.

**Quand les abonnements de Marketo Engage existants seront-ils intégrés à IMS ?**

Les abonnements Marketo existants seront migrés vers le système Identity Management Adobe plus tard dans l’année. La prise en charge de Marketo ne pourra fournir aucune mise à jour concernant la migration d’Adobe IMS. Votre responsable du succès client atteindra le délai prévu au cours des prochains mois.

**Quelle est la différence entre un administrateur de produit Adobe et un administrateur de Marketo Engage ?**

* L’administrateur de produit Adobe est un nouveau rôle dans la plateforme Marketo.
* Le rôle Administrateur de produit Adobe est attribué aux utilisateurs ajoutés en tant qu’administrateur de produit dans Adobe Admin Console
* L’administrateur de produit Adobe est un rôle en lecture seule qui ne peut pas être modifié ni supprimé de Marketo Engage.
* L’administrateur de produit Adobe dispose des mêmes droits et privilèges qu’un administrateur Marketo standard.
* Le rôle d’administrateur du Marketo Engage est toujours un administrateur et est attribué à un utilisateur en Marketo Engage.

**La prise en charge des clients de l’API de gestion des utilisateurs a-t-elle changé ?**

Oui. Ceux qui ont été intégrés à Adobe IMS ne peuvent pas utiliser toutes les API de gestion des utilisateurs Marketo existantes. Pour les actions d’invitation, de mise à jour et de suppression de l’utilisateur, l’Adobe [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html) doit être utilisé. Pour la gestion des rôles, les API de gestion des utilisateurs de Marketo s’appliquent toujours. En outre, aucune autre modification n’est apportée à la prise en charge des clients de l’API REST Marketo.

**Qui contacter pour obtenir de l’aide si nous sommes intégrés à IMS ?**

Vous devez suivre la procédure standard pour contacter [Prise en charge de Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

**Si j’utilise une identité d’Adobe pour accéder à d’autres applications d’Adobe, puis-je l’utiliser pour accéder à Marketo ?**

Même si vous disposez d’autres produits Adobe, vous ne pouvez pas accéder à Marketo avec l’Adobe Identity tant que l’abonnement n’est pas migré vers IMS.

**Les rôles utilisateur Marketo (dans les espaces de travail) sont-ils gérés dans Adobe Admin Console ?**

Nombre La gestion des rôles utilisateur (dans les espaces de travail) est effectuée dans Marketo Engage.

**Je suis administrateur Marketo dans un abonnement intégré IMS et n’ai pas accès au Admin Console. Comment puis-je y accéder ?**

Tout administrateur système d’Adobe ou de produit ayant accès au Admin Console de votre entreprise peut vous donner accès. Si vous ne savez pas qui dans votre organisation dispose des privilèges d’administrateur dans la console, contactez [Assistance clientèle Adobe](https://helpx.adobe.com/contact.html).

**Comment un administrateur ajouterait-il des utilisateurs à Marketo Sales Connect ?**

Bien qu’il y ait une carte de produit dans Admin Console pour Sales Connect, Admin Console ne doit pas être utilisé pour ajouter/gérer des utilisateurs. Le lien suivant permet aux administrateurs de gérer les utilisateurs via Marketo Sales Connect : [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Où puis-je en savoir plus sur Adobe Admin Console ?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**Puis-je toujours accéder à la section Admin de Marketo pour apporter des modifications au compte utilisateur de mon compte ?**

Non, vous devez accéder à [account.adobe.com](https://account.adobe.com).

**Comment cela fonctionne-t-il avec Marketo Universal ID ?**

Les personnes intégrées à l’identité Adobe peuvent accéder facilement à tous les abonnements activés pour IMS via le sélecteur d’abonnements du produit.

**Cela fonctionne-t-il avec SSO ?**

Oui. L’intégration de Marketo avec Adobe IMS prend en charge les utilisateurs d’ID universels et l’authentification unique. L’authentification unique est désormais pilotée par Adobe IMS et configurée au niveau de l’organisation dans Adobe Admin Console. [En savoir plus ici](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Comment fonctionne l’autorisation de périphérique ?**

Adobe IMS ne prend actuellement en charge rien de tel que la fonctionnalité d’autorisation des périphériques de Marketo.

**Est-il toujours possible d’utiliser la fonction &quot;Se connecter dans la boîte de dialogue d’invitation&quot; pour rendre la connexion d’un utilisateur unique à partir de son email ?**

Nombre Le workflow d’ invitation d’utilisateur n’est plus principal lorsqu’un abonnement est activé pour IMS. La fonctionnalité n’est donc plus valide. L’identité de l’Adobe nécessite que l’identité d’un utilisateur soit déterminée par son email.

**Pour Adobe IMS, avons-nous la possibilité d’utiliser Adobe ID, Enterprise ID ou Federated ID ?**

Oui, vous déterminez le type d’identité à prendre en charge par votre organisation. Plus d’informations sont disponibles ici : [Présentation des identités](https://helpx.adobe.com/enterprise/using/identity.html) et ici : [Configuration d’identité](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [Configuration de l’administrateur](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Ajout ou suppression d’un administrateur de produit](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Ajout ou suppression d’un utilisateur](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

