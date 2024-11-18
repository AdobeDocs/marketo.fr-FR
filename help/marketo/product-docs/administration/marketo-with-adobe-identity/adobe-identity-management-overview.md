---
description: Présentation d’Adobe Identity Management - Documentation Marketo - Documentation du produit
title: Présentation d’Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 8d4a542687119e7e4044b26eeafcc71315609f19
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Présentation d’Adobe Identity Management {#adobe-identity-management-overview}

Tous les nouveaux abonnements Adobe Marketo Engage (du 31 juillet 2023 ou version ultérieure) sont intégrés au système Identity Management Adobe. Les abonnements de Marketo Engage existants sont actuellement migrés vers le système Identity Management Adobe lors de tout événement de vente, qui inclut les renouvellements, les événements de recontraction et/ou les ajouts. Les migrations en dehors d’un événement de vente sont prises en charge à compter d’octobre 2024. Les administrateurs de Marketo recevront une notification 2 à 4 semaines à l’avance si leur abonnement est prévu en dehors d’un événement de vente.

>[!NOTE]
>
>La prise en charge de Marketo ne peut fournir aucune mise à jour concernant la migration d’Adobe IMS. L’équipe Compte d’Adobe atteindra le délai prévu au cours des prochains mois. Pour plus d&#39;informations, consultez [cet article](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"} et la [foire aux questions](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

Pour les abonnements intégrés à une identité Adobe, Adobe Admin Console est utilisé pour la gestion des utilisateurs. Les concepts liés aux identités, tels que l’authentification unique, sont également gérés dans l’Admin Console.

* En savoir plus sur [Adobe Admin Console](https://helpx.adobe.com/fr/enterprise/using/admin-console.html){target="_blank"}.
* Pour plus d&#39;informations sur la [configuration de votre organisation d&#39;Adobe associée à votre abonnement Marketo](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Si vous souhaitez mettre en oeuvre l’authentification unique et que votre abonnement a été intégré à Adobe Identity sans que l’authentification unique soit mise en oeuvre dans l’organisation d’Adobe, envoyez un ticket à l’[Assistance Marketo](https://nation.marketo.com/){target="_blank"} et spécifiez la rubrique &quot;Marketo on Admin Console, implémentation de l’authentification unique&quot;.

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
  <td>Responsable de l’administration des utilisateurs au sein d’un profil de produit. Ils ne peuvent pas gérer les utilisateurs en dehors de ce profil spécifique. Un administrateur de profil de produit n’a pas accès à l’application Marketo, sauf s’il a été ajouté au profil de produit en tant qu’utilisateur. Leur rôle reste un utilisateur standard (espace de travail par défaut s’il dispose de plusieurs espaces de travail).
</td>
 </tr>
 <tr>
  <td><strong>Administrateur Marketo Engage</strong></td>
  <td>Personne ayant accès à un Marketo Engage avec des privilèges d’administrateur. Rôle attribué dans Marketo Engage et non dans Adobe Admin Console (apparaît simplement comme "Admin" dans le modal <b>Modifier l’utilisateur</b>).</td>
 </tr>
 <tr>
  <td><strong>Utilisateur Marketo Engage</strong></td>
  <td>Personne à qui l’accès au Marketo Engage a été accordé. Aucun privilège d’administrateur.</td>
 </tr>
</table>

## Questions fréquentes {#faq}

Les questions fréquentes [ se trouvent ici ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Configuration de l’administrateur](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Ajout ou suppression d’un administrateur de produit](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Ajouter ou supprimer un utilisateur](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
