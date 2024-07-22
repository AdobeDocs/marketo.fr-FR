---
description: Suppression de l’accès Sales Insight - Documents Marketo - Documentation du produit
title: Suppression de l’accès à Sales Insight
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 5%

---

# Suppression de l’accès à Sales Insight {#remove-sales-insight-access}

Suivez les étapes ci-après pour supprimer l’accès aux fonctionnalités Sales Insight dans Salesforce. Applicable à Salesforce Classic et à Lightning.

## Vue d’ensemble {#overview}

Pour accéder à toutes les fonctionnalités d’aperçu des ventes, vous devez disposer des autorisations nécessaires pour accéder aux objets mentionnés ci-dessous, aux classes d’apex et aux pages de force visuelle. La suppression de ces informations supprimera l’accès à Sales Insight.

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

## Suppression de l’accès à Sales Insight {#removing-access-to-sales-insight}

1. Connectez-vous à votre compte Salesforce.

1. Cliquez sur **Configuration**.

   ![](assets/remove-sales-insight-access-1.png)

1. Sous Administrateur, cliquez sur **Gérer les utilisateurs**, puis sur **Profils**.

1. Cliquez sur le profil que vous souhaitez mettre à jour, puis **Modifier**.

1. Faites défiler l’écran jusqu’à &quot;Paramètres d’onglet personnalisés&quot; sous Paramètres d’onglet.

1. Sélectionnez l’option &quot;Onglet masqué&quot; dans la liste déroulante pour Marketo Sales Insight Config et MSI Marketo Sales Outbox (Boîte d’envoi des ventes).

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Faites défiler l’écran jusqu’à &quot;Autorisations d’objet personnalisé&quot;.

1. Supprimez l’accès &quot;Lecture, Créer, Modifier, Supprimer&quot; des objets suivants :

   * BestBetsCache
   * Détails de la vue des meilleurs paris
   * Meilleures vues de paris
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * IntégrerMomentsCache
   * Configuration de Marketo Sales Insight
   * ScoringCache
   * Valeurs
   * CacheActivitéWeb

1. Faites défiler l’écran jusqu’à la section &quot;Accès activé à la classe Apex&quot;. Cliquez sur **Modifier**.

1. Dans la section &quot;Classes Apex activées&quot;, sélectionnez toutes les classes commençant par &quot;mkto_si&quot;. Cela devrait ajouter jusqu’à 159 classes.

1. Cliquez sur **Supprimer**, puis sur **Enregistrer**.

   ![](assets/remove-sales-insight-access-4.png)

1. Faites défiler l’écran jusqu’à la section &quot;Accès à la page Visualforce activé&quot;. Cliquez sur **Modifier**.

1. Dans la section &quot;Pages Visualforce activées&quot;, sélectionnez toutes les pages commençant par &quot;mkto_si&quot;. Cela devrait ajouter jusqu’à 64 pages.

1. Cliquez sur **Supprimer**, puis sur **Enregistrer**.

   ![](assets/remove-sales-insight-access-5.png)

1. Faites défiler l’écran jusqu’à la section &quot;Activé de l’accès aux définitions de paramètres personnalisés&quot;. Cliquez sur **Modifier**.

1. Sélectionnez &quot;Marketo Sales Insight.mkto_si.Marketo Settings&quot; et &quot;Marketo Sales Insight.mkto_si.User Preferences&quot;.

1. Cliquez sur **Supprimer**, puis sur **Enregistrer**.

   ![](assets/remove-sales-insight-access-6.png)

C&#39;est tout ! Vous avez supprimé l’accès à Sales Insight. Répétez les mêmes étapes pour tout autre profil dont vous souhaitez supprimer l’accès.
