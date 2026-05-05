---
description: Présentation d’Adobe Identity Management for Marketo Engage, y compris le calendrier de la migration, la gestion des utilisateurs Admin Console et les niveaux de profil tels que Administrateur système et Administrateur de produit.
title: Vue d’ensemble d’Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: c06481152e88b8760a4539842a91aea90ab07fa1
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 6%

---

# Vue d’ensemble d’Adobe Identity Management {#adobe-identity-management-overview}

Tous les nouveaux abonnements Adobe Marketo Engage (31 juillet 2023 ou version ultérieure) sont intégrés au système Adobe Identity Management.

Pour les abonnements intégrés à Adobe identity, Adobe Admin Console est utilisé pour la gestion des utilisateurs. Les concepts liés à l’identité, tels que l’authentification SSO, sont également gérés dans Admin Console.

* En savoir plus sur le [](https://helpx.adobe.com/fr/enterprise/using/admin-console.html){target="_blank"}.
* Obtenez des informations supplémentaires sur [la configuration de votre organisation Adobe liée à votre abonnement Marketo](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Si vous souhaitez implémenter l’authentification unique et que votre abonnement a été intégré à Adobe Identity sans que la connexion unique ne soit implémentée dans l’organisation Adobe, envoyez un ticket à l’assistance de [Marketo](https://nation.marketo.com/){target="_blank"} et indiquez la rubrique « Marketo sur Admin Console, implémentation de l’authentification unique ».

## Niveaux de profil {#profile-levels}

Les abonnements Adobe Marketo Engage intégrés au système Adobe Identity Management prennent en charge divers profils. Voici les types de profils utilisateur pertinents dans cette intégration.

<table>
 <tr>
  <td><strong>Administrateur système Adobe Admin Console</strong></td>
  <td>Responsable de la configuration des concepts d’identité pour l’organisation Adobe et le produit Marketo Engage dans Adobe Admin Console. Rôle accordé lors de la configuration de l’organisation Adobe.</td>
 </tr>
 <tr>
  <td><strong>Administrateur de produit Adobe Admin Console</strong></td>
  <td>Responsable de l’octroi des droits aux utilisateurs pour le produit Marketo Engage dans Adobe Admin Console. Rôle accordé dans Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrateur de profil de produit Adobe Admin Console</strong></td>
  <td>Responsable de l’administration des utilisateurs dans un profil de produit. Ils ne peuvent pas gérer les utilisateurs en dehors de ce profil spécifique. Un administrateur de profil de produit n’a pas accès à l’application Marketo, sauf s’il est ajouté au profil de produit en tant qu’utilisateur. Leur rôle serait toujours celui d’un utilisateur standard (espace de travail par défaut s’il existe plusieurs espaces de travail).
</td>
 </tr>
 <tr>
  <td><strong>Administrateur Marketo Engage</strong></td>
  <td>Personne ayant reçu l’accès à Marketo Engage avec les privilèges d’administration. Rôle attribué dans Marketo Engage, et non dans Adobe Admin Console (s’affiche uniquement en tant qu’« administrateur » dans la boîte de dialogue modale <b>Modifier l’utilisateur</b>).</td>
 </tr>
 <tr>
  <td><strong>Utilisateur Marketo Engage</strong></td>
  <td>Personne à qui l’accès à Marketo Engage a été accordé. Aucun privilège d’administration.</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>* [Configuration de l’administration](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Ajout ou suppression d’un administrateur de produit](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-product-admin.md){target="_blank"}
>* [Ajouter ou supprimer un utilisateur](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md){target="_blank"}
