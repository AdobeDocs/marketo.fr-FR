---
description: Ajout d’un jeu d’autorisations Sales Insight - Documents Marketo - Documentation du produit
title: Ajouter un jeu d’autorisations Sales Insight
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 3%

---

# Ajouter un jeu d’autorisations Sales Insight {#add-sales-insight-permission-set}

Procédez comme suit pour ajouter l’accès aux fonctionnalités Sales Insight dans Salesforce. Applicable à Salesforce Classic et à l’éclairage

>[!PREREQUISITES]
>
>[Mettez à jour votre package Sales Insight Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} vers la version 1.8000 ou ultérieure pour utiliser cette fonctionnalité.

>[!IMPORTANT]
>
>Si vous avez auparavant donné l’accès à Sales Insight à tous les profils et/ou mis en oeuvre Sales Insight pour tous vos utilisateurs, vous devez [ supprimer l’accès au niveau de profil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} pour utiliser ce jeu d’autorisations.

## Vue d’ensemble {#overview}

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

* Accès aux classes Apex : 159 classes Apex commençant par &quot;mkto_si&quot;
* Visualforce Page Access : 64 pages Visualforce commençant par &quot;mkto_si&quot;
* Définitions des paramètres personnalisés : paramètres de mkto_si.Marketo et préférences de mkto_si.User

## Ajout d’un jeu d’autorisations d’application Marketo aux utilisateurs {#adding-marketo-app-permission-set-to-users}

1. Connectez-vous à votre compte Salesforce.

1. Cliquez sur **Configuration**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. Sous Administrateur, cliquez pour déployer **Gérer les utilisateurs**, puis **Utilisateurs**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. Sous Tous les utilisateurs, sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès, puis cliquez sur **Attributs du jeu d’autorisations**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Cliquez sur **Modifier les affectations**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Sélectionnez **Marketo App Access** parmi les jeux d’autorisations disponibles, puis **Ajouter**. Cliquez sur **Enregistrer**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Désormais, lorsque vous faites défiler la page Détails de l’utilisateur, &quot;Accès à l’application Marketo&quot; s’affiche sous Affectations de jeu d’autorisations.

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Les utilisateurs qui n’ont pas accès à Sales Insight verront ce message : &quot;Vous ne disposez pas des privilèges suffisants pour accéder à cet onglet.&quot;

C&#39;est tout ! Vous avez correctement ajouté l’accès Sales Insight . Répétez les mêmes étapes pour tout autre profil auquel vous souhaitez ajouter un accès.
