---
description: Suppression de l’accès à Sales Insight - Documents Marketo - Documentation du produit
title: Supprimer l’accès à Sales Insight
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 4%

---

# Supprimer l’accès [!DNL Sales Insight] {#remove-sales-insight-access}

Procédez comme suit pour supprimer l’accès aux fonctionnalités [!DNL Sales Insight] dans [!DNL Salesforce]. Applicable à [!DNL Salesforce] Classic et Lightning.

## Vue d’ensemble {#overview}

L’autorisation des objets mentionnés ci-dessous, des classes apex et des pages visualforce est requise pour accéder à toutes les fonctionnalités de [!DNL Sales Insight]. Si vous les supprimez, vous supprimez l’accès à [!DNL Sales Insight].

**Paramètres de l’objet**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] Consulter les détails</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>[!DNL Best Bets] Vues</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>CacheMomentsIntéressants</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>[!DNL Marketo Sales Insight] Config</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>Valeurs</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
  <tr> 
   <td>CacheActivitéWeb</td> 
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td> 
  </tr> 
 </tbody> 
</table>

* Accès aux classes Apex : 159 classes Apex commençant par « mkto_si »
* Accès à la page Visualforce : 64 pages Visualforce commençant par « mkto_si »
* Définitions des paramètres personnalisés : mkto_si.Marketo Settings &amp; mkto_si.User Preferences

## Suppression de l’accès à [!DNL Sales Insight] {#removing-access-to-sales-insight}

1. Connectez-vous à votre compte [!DNL Salesforce].

1. Cliquez sur **[!UICONTROL Configurer]**.

   ![](assets/remove-sales-insight-access-1.png)

1. Sous [!UICONTROL Administrateur], cliquez sur **[!UICONTROL Gérer les utilisateurs]**, puis **[!UICONTROL Profils]**.

1. Cliquez sur le profil que vous souhaitez mettre à jour, puis **[!UICONTROL Modifier]**.

1. Faites défiler jusqu’à « [!UICONTROL Paramètres d’onglet personnalisés] » sous [!UICONTROL Paramètres d’onglet].

1. Sélectionnez l’option « [!UICONTROL Onglet masqué] » dans la liste déroulante de la boîte d’envoi de configuration [!DNL Marketo Sales Insight] et de [!DNL Marketo Sales] MSI.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Faites défiler jusqu’à « [!UICONTROL &#x200B; Autorisations d’objet personnalisé &#x200B;] ».

1. Supprimez l’accès « Lire, Créer, Modifier et Supprimer » des objets suivants :

   * BestBetsCache
   * [!DNL Best Bets] Afficher les détails
   * [!DNL Best Bets] vues
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * CacheMomentsIntéressants
   * Configuration [!DNL Marketo Sales Insight]
   * ScoringCache
   * Valeurs
   * CacheActivitéWeb

1. Faites défiler l’écran jusqu’à la section « [!UICONTROL Accès de classe apex activé] ». Cliquez sur **[!UICONTROL Modifier]**.

1. Dans la section « [!UICONTROL Classes Apex activées] », sélectionnez toutes les classes commençant par « mkto_si ». Cela devrait ajouter jusqu’à 159 classes.

1. Cliquez sur **[!UICONTROL Supprimer]**, puis sur **[!UICONTROL Enregistrer]**.

   ![](assets/remove-sales-insight-access-4.png)

1. Faites défiler l’écran jusqu’à la section « [!UICONTROL Accès à la page Visualforce activé] ». Cliquez sur **[!UICONTROL Modifier]**.

1. Dans la section « [!UICONTROL Activer les pages Visualforce] », sélectionnez toutes les pages qui commencent par « mkto_si ». Cela devrait faire jusqu’à 64 pages.

1. Cliquez sur **[!UICONTROL Supprimer]**, puis sur **[!UICONTROL Enregistrer]**.

   ![](assets/remove-sales-insight-access-5.png)

1. Faites défiler l’écran jusqu’à la section « [!UICONTROL Accès aux définitions de paramètres personnalisés activés] ». Cliquez sur **[!UICONTROL Modifier]**.

1. Sélectionnez « Paramètres Marketo Sales Insight.mkto_si.Marketo » et « Préférences utilisateur Marketo Sales Insight.mkto_si. »

1. Cliquez sur **[!UICONTROL Supprimer]**, puis sur **[!UICONTROL Enregistrer]**.

   ![](assets/remove-sales-insight-access-6.png)

Vous avez terminé. Vous avez correctement supprimé l’accès à [!DNL Sales Insight]. Répétez les mêmes étapes pour tout autre profil dont vous souhaitez supprimer l’accès.
