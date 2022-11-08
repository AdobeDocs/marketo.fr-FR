---
description: Notes de mise à jour de la pratique - Documents Marketo - Documentation du produit
title: Notes de mise à jour de la pratique
hide: true
hidefromtoc: true
exl-id: e1004c31-8b8c-4bc7-845f-4e06644a3273
source-git-commit: d6d8674ef3357cef1b388a43baade1c57ed98e3e
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 3%

---

# Notes de mise à jour : Octobre 2022 {#release-notes-oct-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 octobre. Vérifiez la disponibilité de votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

Les fonctionnalités suivantes commenceront à être publiées sur **14 octobre 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire). Les fonctionnalités de publication et les dates exactes peuvent être modifiées.

## Orchestration cross-canal {#cross-channel-orchestration}

_**Chat dynamique**_

* **Organiser automatiquement les flux de dialogue pour la conversation dynamique**: Améliorez votre canevas de dialogue bondé en organisant tout sur la zone de travail dans un format propre et facile à lire en appuyant sur un bouton via l’option Réorganiser automatiquement.

* **Prise en charge des types de données supplémentaires pour Dynamic Chat**: Trois nouveaux types de données (booléen, entier, flottant) vous permettent d’exploiter d’autres champs de Marketo Engage existants dans Dynamic Chat pour des tâches comme le ciblage en fonction des scores ou la demande de questions oui/non aux visiteurs.

* **Liens de réunion pour la conversation dynamique**: Option permettant d’inclure automatiquement un lien Equipes ou Rencontrer pour Google et Outlook dans chaque invitation calendaire envoyée aux visiteurs.

* **Notifications de réunion planifiées pour la messagerie instantanée**: Les représentants commerciaux reçoivent des notifications par e-mail automatisées concernant les réunions planifiées ainsi que toute information pertinente sur l’interaction de chatbot du visiteur.

* **Rôles et autorisations pour Dynamic Chat**: Les administrateurs peuvent utiliser des autorisations granulaires pour contrôler la visibilité et l’utilisation de l’application et créer des rôles utilisateur personnalisés.

   * Accès complet : les utilisateurs peuvent profiter pleinement de cette fonctionnalité (par exemple, publier des boîtes de dialogue, changer de modèle de couleur, etc.)
   * Accès en lecture seule : les utilisateurs peuvent consulter les informations mais ne peuvent pas apporter de modifications (par exemple, voir Critères d’audience ou Concepteur de diffusion en continu, mais pas modifier).
   * Accès restreint : les utilisateurs ne peuvent pas afficher ni accéder aux sections Configuration ou Intégrations .

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

## Expérience de nouvelle génération {#next-generation-experience}

* **Mise à jour d’Screens dans l’expérience de nouvelle génération**: Nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour, accessibles par le biais d’un bouton d’activation/désactivation :

   * Détails du modèle de page d’entrée
   * Liste des modèles de courrier électronique

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-next-generation-experience/toggle-switch.md">Basculer entre les deux</a></td>
  </tr>
  </tbody>
</table>

* **Amélioration de l’option Utilisé par l’onglet Détails du modèle de courrier électronique**: Dans la nouvelle expérience, vous verrez des informations supplémentaires relatives aux ressources à l’aide du modèle de courrier électronique, notamment Asset Status (État de la ressource), Last Modified (Dernière modification) et Last Modified By (Dernière modification). Vous pouvez également rechercher, trier et filtrer la liste des ressources utilisées.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

* **Modèles de filtre de ressources de rapport**: Nouvelle conception des modèles de configuration de rapport affichant une nouvelle arborescence de ressources dans le menu de configuration et un filtre pour Date de création et de modification.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

## Environnement de données marketing {#marketing-data-environment}

* **Intégration d’Adobe Privacy Service**: Harmonisez-vous avec Privacy Service afin d’automatiser la conformité aux réglementations de confidentialité des données dans les produits Experience Cloud. Actuellement, ce service n’est disponible que pour les clients Marketo Engage intégrés au système Identity Management Adobe.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

## Améliorations des API {#api-enhancements}

* **Importation de pistes en bloc : Association des vendeurs**: Parité avec l’API REST Lead pour pouvoir associer des prospects aux vendeurs au cours du processus d’importation de prospects en masse, ce qui réduit la complexité et le nombre d’appels API requis.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="https://developers.marketo.com/rest-api/bulk-import/bulk-lead-import/">Importation de pistes en bloc</a></td>
  </tr>
  </tbody>
</table>

## Sales Insight {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **Intégration de Sales Insight à Dynamic Chat**: Le tableau de bord des statistiques comprend désormais des activités de conversation dynamique dans la grille dynamique, ainsi qu’un résumé hebdomadaire et des cartes détaillées.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Intégration de tchat dynamique</a></td>
  </tr>
  </tbody>
</table>

## Annonces {#announcements}

* **Forms 1.0**: L’obsolescence de Forms 1.0 sera terminée avec la version d’octobre. Les ressources Forms 1.0 ne pourront plus envoyer de données à Marketo Engage et renverront des erreurs si elles sont tentées.

* **Forms sans script**: Forms ne fonctionnera plus lorsque JavaScript est désactivé dans le navigateur. L’envoi du formulaire nécessite l’activation de JavaScript.
