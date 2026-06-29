---
description: Découvrez comment ajouter le jeu d’autorisations Sales Insight dans Salesforce. Attribuez la visionneuse aux utilisateurs qui ont besoin d’un accès à Marketo Sales Insight.
title: Ajouter un jeu d’autorisations d’Informations sur les ventes
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/uFyP8aZCuXSPJn5ktZUxmCoVekyw9LN88U3KaY06-do
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 427d3327b9d5641dbc6744ee32ee8803ae76d6fe
workflow-type: tm+mt
source-wordcount: 393
ht-degree: 4%

---

# Ajouter un jeu d’autorisations [!DNL Sales Insight] {#add-sales-insight-permission-set}

Procédez comme suit pour ajouter l’accès aux fonctionnalités [!DNL Sales Insight] dans [!DNL Salesforce]. Applicable à [!DNL Salesforce] Classic et Lighting

>[!PREREQUISITES]
>
>[Mettez à jour votre [!DNL Sales Insight] [!DNL Salesforce] package](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} vers la version 1.8000 ou ultérieure pour utiliser cette fonctionnalité.

>[!IMPORTANT]
>
>* Si vous avez précédemment donné un accès [!DNL Sales Insight] à tous les profils et/ou implémenté des [!DNL Sales Insight] pour tous vos utilisateurs, vous devez [supprimer l’accès au niveau du profil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} pour utiliser ce jeu d’autorisations.
>
>* La licence Salesforce standard est requise pour une fonctionnalité complète de MSI. Les utilisateurs disposant de la licence Salesforce Platform (une classe de licence limitée) peuvent voir des erreurs lors de l’exécution de certaines actions ou de l’accès à certains onglets.

## Vue d’ensemble {#overview}

L’autorisation « Application Marketo » fait partie du package [!DNL Sales Insight] [!DNL Salesforce]. Il permet d’accéder aux objets, classes apex et pages visualforce mentionnés ci-dessous. Ils sont nécessaires pour accéder à toutes les fonctionnalités [!DNL Sales Insight].

**Paramètres de l’objet**

<table>
 <tbody>
 <tr>
   <td>BestBetsCache</td>
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td>
  </tr>
  <tr>
   <td>Détails de la vue des meilleurs paris</td>
   <td>Lecture, Création, Modification, Suppression, Afficher tout, Modifier tout</td>
  </tr>
  <tr>
   <td>Meilleures vues</td>
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
   <td>Configuration du [!DNL Sales Insight] Marketo</td>
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

## Ajout d’un jeu d’autorisations d’application Marketo aux utilisateurs {#adding-marketo-app-permission-set-to-users}

1. Connectez-vous à votre compte [!DNL Salesforce].

1. Cliquez sur **[!UICONTROL Configurer]**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. Sous Administrateur, cliquez pour déployer **[!UICONTROL Gérer les utilisateurs]**, puis **[!UICONTROL Utilisateurs]**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. Sous Tous les utilisateurs, sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès, puis cliquez sur **[!UICONTROL Affectations de jeux d’autorisations]**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Cliquez sur **[!UICONTROL Modifier les affectations]**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Sélectionnez **[!UICONTROL Accès à l&#39;application]** parmi les jeux d&#39;autorisations disponibles, puis **[!UICONTROL Ajouter]**. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/add-sales-insight-permission-set-5.png)

1. Désormais, lorsque vous faites défiler la page Détails de l’utilisateur vers le bas, vous voyez « Accès à l’application Marketo » sous Affectations de jeux d’autorisations.

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Les utilisateurs qui n’ont pas accès à [!DNL Sales Insight] verront le message suivant : « Vous ne disposez pas des privilèges suffisants pour accéder à cet onglet ».

Vous avez terminé. Vous avez correctement ajouté l’accès à [!DNL Sales Insight]. Répétez les mêmes étapes pour tout autre profil auquel vous souhaitez ajouter un accès.
