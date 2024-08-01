---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 1839ccb646e775b67efa8de7d2d2bf3dbbbefa72
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 6%

---

# Notes de mise à jour : juillet 2024 {#release-notes-july-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 juillet. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques au Adobe Dynamic Chat [ se trouvent ici ](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **26 juillet 2024**, avec un déploiement progressif des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
     <tr> 
   <td><strong>Tableau de bord de l’engagement pour les webinaires interactifs</strong> : obtenez une vue agrégée des performances des webinaires ainsi qu’une vue complète de l’engagement pour chaque participant au cours du webinaire afin que vous puissiez déterminer les pistes à cibler par le biais d’outils d’orchestration de Marketo Engage.</td> 
    <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">Tableau de bord des engagements</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Gestion de salle pour les webinaires interactifs</strong> : accédez aux salles individuelles créées (et apportez des modifications si nécessaire), accédez au contenu et à l’enregistrement (et effacez-les si nécessaire pour optimiser le stockage).</td> 
    <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">Gestion des salles</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Personnalisation de webinaires pour les webinaires interactifs</strong> : offrez une expérience de marque approuvée par l’organisation de manière uniforme grâce à l’utilisation d’une interface de salle commune, d’écrans intermédiaires (tels que les arrière-plans d’accès aux participants), ainsi que d’arrière-plans vidéo personnalisés, afin que la stratégie des webinaires s’aligne plus facilement sur la stratégie de la marque.</td> 
    <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">Personnalisation des webinaires interactifs</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Modification de l’API REST Marketo</strong> : nous introduisons une modification mineure de l’ <a href="https://developers.marketo.com/rest-api/user-management/">API User Management</a>. Les points de terminaison <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Parcourir les utilisateurs</a> et <a href="https://developers.marketo.com/rest-api/user-management/#delete_user"> Supprimer l’utilisateur</a> prennent désormais en charge les utilisateurs de la <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">gestion de compte Target</a>.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Nouveau site de documentation pour les développeurs** : dans le cadre de nos efforts continus pour améliorer l’expérience utilisateur des Marketo Engage, nous migrerons toute la documentation pour les développeurs vers Adobe Experience League et le site web Adobe Developer en juillet 2024. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Abandon des fonctions sociales** : le mercredi 31 juillet 2024, Marketo Engage commencera à abandonner les fonctions sociales suivantes dans le produit :

   * Sondages
   * Réseaux sociaux
   * Offre de parrainage
   * Partage de vidéos
   * Loteries

Les utilisateurs ne pourront plus créer, cloner ou incorporer l’une de ces fonctions Social dans Marketo Engage. Les ressources sociales existantes continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Jeton d’accès dans l’obsolescence des paramètres de requête** : la prise en charge de l’authentification à l’aide de jetons d’accès dans un paramètre de requête d’un appel de l’API REST Marketo Engage sera supprimée dans une version ultérieure (date spécifique à déterminer). Les intégrations existantes doivent migrer vers l’utilisation de l’en-tête d’autorisation [décrite ici](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Le nouveau développement ne doit utiliser que l’en-tête d’autorisation pour l’authentification avec Marketo Engage.

* **Réauthentification LinkedIn requise** : LinkedIn met à niveau ses API marketing utilisées par les intégrations LinkedIn Marketo Engage. Ces modifications nécessiteront une réauthentification de tous les services LinkedIn LaunchPoint de votre menu **Admin** > **LaunchPoint** entre le 26 juillet et le 15 décembre 2024, afin d’éviter toute interruption de service. Vous trouverez des instructions sur la façon d’y parvenir [ici pour Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} et [ici pour Matched Audiences](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Le service Lead Gen Form possède un type &quot;LinkedIn Lead Gen&quot; et le service de correspondance d’audience a un type &quot;LinkedIn Matched Audiences&quot;. Pour plus d’informations, consultez la [FAQ sur la migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
