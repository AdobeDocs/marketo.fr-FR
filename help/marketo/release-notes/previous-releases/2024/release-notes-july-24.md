---
description: Notes De Mise À Jour - Juillet 2024 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Juillet 2024
feature: Release Information
exl-id: ff63af41-2d33-40f8-abca-3fd9493e7916
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 22%

---

# Notes de mise à jour : juillet 2024 {#release-notes-july-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 juillet. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 26 juillet 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
     <tr>
   <td><strong>Tableau de bord d’engagement pour les webinaires interactifs</strong> : obtenez une vue globale des performances du webinaire ainsi qu’une vue complète de l’engagement de chaque participant pendant le webinaire afin de pouvoir décider quels prospects cibler via les outils d’orchestration de Marketo Engage.</td>
    <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">Tableau de bord des engagements</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Gestion des salles pour les webinaires interactifs</strong> : accédez aux salles individuelles créées (et apportez des modifications si nécessaire) ainsi qu’au contenu et à l’enregistrement (et effacez-les si nécessaire pour optimiser le stockage).</td>
    <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">Gestion des salles</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Personnalisation des webinaires pour les webinaires interactifs</strong> : offrez une expérience de marque uniforme approuvée par l’organisation grâce à l’utilisation d’une interface de salle commune, d’écrans intermédiaires (tels que les arrière-plans de l’écran d’entrée du participant), ainsi que d’arrière-plans vidéo personnalisés, afin que la stratégie du webinaire puisse s’aligner plus facilement sur la stratégie de la marque.</td>
    <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">Personnalisation des webinaires interactifs</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Modification de l’API REST Marketo </strong>: Nous apportons une modification mineure à l’API <a href="https://developers.marketo.com/rest-api/user-management/"> User Management</a>. Les points d’entrée <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Parcourir les utilisateurs</a> et <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Supprimer un utilisateur</a> prennent désormais en charge les utilisateurs <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Gestion de compte Target</a>.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
 </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Nouveau site de documentation pour les développeurs** : dans le cadre de nos efforts continus pour améliorer l’expérience utilisateur de Marketo Engage, nous allons migrer toute la documentation destinée aux développeurs vers Adobe Experience League et le site web Adobe Developer en juillet 2024. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Obsolescence des fonctionnalités sociales** : le mercredi 31 juillet 2024, Marketo Engage commencera l’obsolescence des fonctionnalités sociales suivantes du produit :

   * Sondages
   * Bouton social
   * Offre de parrainage
   * Partage de vidéos
   * Loteries

Les utilisateurs ne pourront plus créer, cloner ni incorporer ces fonctionnalités de réseaux sociaux dans Marketo Engage. Les actifs sociaux existants continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Jeton d’accès obsolète dans les paramètres de requête** : la prise en charge de l’authentification à l’aide de jetons d’accès dans un paramètre de requête d’un appel API REST Marketo Engage sera supprimée dans une version ultérieure (date spécifique à déterminer). Les intégrations existantes doivent migrer vers l’utilisation de l’en-tête d’autorisation [décrit ici](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Le nouveau développement ne doit utiliser que l’en-tête Autorisation pour l’authentification avec Marketo Engage.

* **Réauthentification requise pour LinkedIn** : LinkedIn met à niveau ses API marketing utilisées par les intégrations Marketo Engage LinkedIn. Ces modifications nécessiteront une réauthentification de tous les services LinkedIn LaunchPoint dans votre menu **Admin** > **LaunchPoint** entre le 26 juillet et le 15 décembre 2024, afin d’éviter l’interruption du service. Vous trouverez des instructions sur la manière d’accomplir cette opération [ici pour la génération de leads Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} et [ici pour les audiences appariées](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Le service de formulaire de génération de leads est de type « LinkedIn Lead Gen » et le service d’audiences appariées est de type « LinkedIn Matched Audiences ». Pour plus d’informations, consultez le [FAQ sur la migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
