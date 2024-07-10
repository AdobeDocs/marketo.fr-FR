---
description: Notes de mise à jour actuelles - Documentation de Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: cb69844d8e9e25cae19bc2d4a91c28376f58eadb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 6%

---

# Notes de mise à jour : juillet 2024 {#release-notes-july-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 juillet. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

Notes de mise à jour spécifiques à Adobe Dynamic Chat [peut être consulté ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **26 juillet 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
     <tr> 
   <td><strong>Tableau de bord des engagements pour les webinaires interactifs</strong>: obtenez une vue globale des performances des webinaires ainsi qu’une vue complète de l’engagement pour chaque participant au cours du webinaire afin que vous puissiez décider quel conduit à cibler par le biais des outils d’orchestration de Marketo Engage.</td> 
    <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Gestion des salles pour les webinaires interactifs</strong>: accédez aux pièces individuelles créées (et apportez des modifications si nécessaire) ainsi qu’au contenu et à l’enregistrement (et effacez-les si nécessaire pour optimiser le stockage).</td> 
    <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Personnalisation de webinaires pour les webinaires interactifs</strong>: proposez une expérience de marque unique approuvée par l’organisation grâce à l’utilisation d’une interface de salle commune, d’écrans intermédiaires (tels que les arrière-plans d’écran d’entrée des participants) et d’arrière-plans vidéo personnalisés, de sorte que la stratégie du webinaire puisse s’aligner plus facilement sur la stratégie de la marque.</td> 
    <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Modification de l’API REST Marketo</strong>: nous introduisons une modification mineure au <a href="https://developers.marketo.com/rest-api/user-management/">API User Management</a>. Les deux <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Parcourir les utilisateurs</a> et <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Supprimer un utilisateur</a> Prise en charge des points de fin <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Gestion de compte Target</a> utilisateurs.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Nouveau site de documentation destiné aux développeurs**: dans le cadre de nos efforts continus pour améliorer l’expérience utilisateur des Marketo Engage, nous migrerons en juillet 2024 toute la documentation destinée aux développeurs vers Adobe Experience League et le site web Adobe Developer. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Jeton d’accès dans l’obsolescence des paramètres de requête**: la prise en charge de l’authentification à l’aide des jetons d’accès dans un paramètre de requête d’un appel de l’API REST Marketo Engage sera supprimée dans une version ultérieure (date spécifique à déterminer). Les intégrations existantes doivent migrer vers l’utilisation de l’en-tête d’autorisation. [décrit ici](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Le nouveau développement ne doit utiliser que l’en-tête d’autorisation pour l’authentification avec Marketo Engage.

* **Réauthentification linkedIn requise**: LinkedIn met à niveau ses API marketing utilisées par les intégrations LinkedIn Marketo Engage. Ces modifications nécessiteront une réauthentification de tous les services LinkedIn LaunchPoint de votre **Administration** > **LaunchPoint** du 26 juillet au 15 décembre 2024, pour éviter l’interruption de service. Vous trouverez des instructions sur la manière d’y parvenir. [ici pour Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} et [ici pour les audiences mises en correspondance](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Le service Lead Gen Form possède un type &quot;LinkedIn Lead Gen&quot; et le service de correspondance d’audience a un type &quot;LinkedIn Matched Audiences&quot;. Pour plus d’informations, voir la section [FAQ sur la migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
