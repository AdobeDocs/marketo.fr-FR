---
description: Présentation D’Adobe Identity Management - Documentation De Marketo - Documentation Du Produit
title: Présentation d’Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Présentation d’Adobe Identity Management {#adobe-identity-management-overview}

Tous les nouveaux abonnements Adobe Marketo Engage (31 juillet 2023 ou version ultérieure) sont intégrés au système Adobe Identity Management. Les abonnements Marketo Engage existants sont actuellement migrés vers le système Adobe Identity Management lors de n’importe quel événement de vente, qui inclut les renouvellements, les événements de réapprovisionnement et/ou les addenda. Les migrations en dehors d’un événement de vente sont prises en charge à compter d’octobre 2024. Les administrateurs Marketo recevront une notification 2 à 4 semaines à l’avance si leur abonnement doit être migré en dehors d’un événement de vente.

>[!NOTE]
>
>L’assistance Marketo n’est pas en mesure de fournir des mises à jour concernant la migration d’Adobe IMS. L’équipe chargée du compte Adobe communiquera avec la date prévue dans les prochains mois. Pour plus d’informations, consultez [cet article](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"} et le [Forum aux questions](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

Pour les abonnements intégrés à Adobe identity, Adobe Admin Console est utilisé pour la gestion des utilisateurs. Les concepts liés à l’identité, tels que l’authentification unique, sont également gérés dans Admin Console.

* En savoir plus sur le [Adobe Admin Console](https://helpx.adobe.com/fr/enterprise/using/admin-console.html){target="_blank"}.
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
  <td>Responsable de l’administration des utilisateurs dans un profil de produit. Ils ne peuvent pas gérer les utilisateurs en dehors de ce profil spécifique. Un administrateur de profil de produit n’a pas accès à l’application Marketo, sauf s’il est ajouté au profil de produit en tant qu’utilisateur. Leur rôle reste celui d’un utilisateur standard (espace de travail par défaut s’il existe plusieurs espaces de travail).
</td>
 </tr>
 <tr>
  <td><strong>Administrateur Marketo Engage</strong></td>
  <td>Personne ayant reçu l’accès à Marketo Engage avec les privilèges d’administration. Rôle attribué dans Marketo Engage, et non dans Adobe Admin Console (apparaît simplement comme « Admin » dans la boîte de dialogue modale <b>Modifier l’utilisateur</b>).</td>
 </tr>
 <tr>
  <td><strong>Utilisateur Marketo Engage</strong></td>
  <td>Personne à qui l’accès à Marketo Engage a été accordé. Aucun privilège d’administration.</td>
 </tr>
</table>

## Questions fréquentes {#faq}

Foire aux questions [ici](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Configuration de l’administration](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Ajout ou suppression d’un administrateur de produit](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Ajouter ou supprimer un utilisateur](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
