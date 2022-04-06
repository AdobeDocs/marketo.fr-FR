---
description: Ajout d’un jeu d’autorisations Sales Insight - Documents Marketo - Documentation du produit
title: Ajouter un jeu d’autorisations Sales Insight
hide: true
hidefromtoc: true
source-git-commit: 2ac0ef0b715eb2acd03fe2c5ad4cfee8daeef4f6
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 3%

---

# Ajouter un jeu d’autorisations Sales Insight {#add-sales-insight-permission-set}

Procédez comme suit pour ajouter l’accès aux fonctionnalités Sales Insight dans Salesforce. Applicable à Salesforce Classic et à l’éclairage

>[!PREREQUISITES]
>
>[Mettre à jour votre package Salesforce Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;} vers la version 1.8000 ou ultérieure pour utiliser cette fonctionnalité.

>[!IMPORTANT]
>
>Si vous avez auparavant donné l’accès à Sales Insight à tous les profils et/ou mis en oeuvre Sales Insight pour tous vos utilisateurs, vous devez [suppression de l’accès au niveau de profil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;} pour utiliser ce jeu d’autorisations.

## APERÇU {#overview}

L’autorisation &quot;Application Marketo&quot; fait partie du package Salesforce d’aperçu des ventes. Il inclut l’accès aux objets, classes d’apex et pages de force visuelle mentionnés ci-dessous. Elles sont requises pour accéder à toutes les fonctionnalités d’aperçu des ventes.

**Paramètres d’objet**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>Détails de la vue des meilleurs paris</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>Meilleures vues de paris</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>IntégrerMomentsCache</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>Configuration de Marketo Sales Insight</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>Valeurs</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
  <tr> 
   <td>CacheActivitéWeb</td> 
   <td>Lecture, Créer, Modifier, Supprimer, Tout afficher, Tout modifier</td> 
  </tr> 
 </tbody> 
</table>

* Accès à la classe Apex : 159 classes Apex avec &quot;mkto_si&quot;
* Visualforce Page Access : 64 Pages Visualforce avec &quot;mkto_si&quot;
* Définitions des paramètres personnalisés : Paramètres mkto_si.Marketo et préférences de l’utilisateur mkto_si.User

## Ajout d’un jeu d’autorisations d’application Marketo aux utilisateurs {#adding-marketo-app-permission-set-to-users}

1. Connectez-vous à votre compte Salesforce.

PICC

1. Cliquez sur **Configuration**.

PICC

1. Sous Administrateur, cliquez sur pour effectuer le déploiement. **Gestion des utilisateurs**, puis **Utilisateurs**.

PICC

1. Sous Tous les utilisateurs, sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès, puis cliquez sur **Affectations de jeux d’autorisations**.

PICC

1. Cliquez sur **Modifier les affectations**.

PICC

1. Sélectionner **Accès aux applications Marketo** à partir des jeux d’autorisations disponibles, puis **Ajouter**. Cliquez sur **Enregistrer**.

PICC

1. Désormais, lorsque vous faites défiler la page Détails de l’utilisateur, &quot;Accès à l’application Marketo&quot; s’affiche sous Affectations de jeu d’autorisations.

PICC

>[!NOTE]
>
>Les utilisateurs qui n’ont pas accès à Sales Insight verront ce message : &quot;Vous ne disposez pas des privilèges suffisants pour accéder à cet onglet.&quot;

C&#39;est tout! Vous avez correctement ajouté l’accès Sales Insight . Répétez les mêmes étapes pour tout autre profil auquel vous souhaitez ajouter un accès.
