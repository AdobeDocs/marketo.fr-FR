---
description: Notes de mise à jour - Octobre 2022 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Octobre 2022
exl-id: 1494b8b9-049c-4969-ab95-a4be41d886b0
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 5%

---

# Notes de mise à jour : Octobre 2022 {#release-notes-oct-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 octobre. Vérifiez la disponibilité de votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **14 octobre 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonctionnalité ci-dessous.

### Environnement de données marketing {#marketing-data-environment}

</br>

* **Synchronisation des champs personnalisés des membres du programme**: Possibilité de synchroniser de manière bidirectionnelle les champs extensibles capturés pour un membre du programme (par exemple, les préférences du participant lors de l’enregistrement de l’événement, tels que la nourriture, les sessions, les suivis, etc.) avec des champs de membre Campaign dans Salesforce.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Synchronisation des champs personnalisés des membres du programme</a></td>
  </tr>
  </tbody>
</table>

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

### Expérience de nouvelle génération {#modern-ux}

</br>

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
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Basculer entre les deux</a></td>
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

### Améliorations des API {#api-enhancements}

</br>

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

### Sales Insight {#sales-insight}

</br>

![(étoile)](assets/yellow-star.png)

* **Intégration de Sales Insight à Dynamic Chat**: Le tableau de bord des statistiques comprend désormais des activités de Dynamic Chat dans la grille dynamique, ainsi qu’un résumé hebdomadaire et des cartes détaillées.

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

## Fonctionnalités de version agile

Les fonctionnalités suivantes suivent un format Agile et sont publiées à diverses dates avant ou après la date de publication standard. Vérifiez l’état de chaque fonctionnalité ci-dessous.

* **Réorganiser automatiquement les flux de dialogue pour les Dynamic Chat**: Améliorez votre canevas de dialogue bondé en organisant tout sur la zone de travail dans un format propre et facile à lire en appuyant sur un bouton via l’option Réorganiser automatiquement.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md#stream-designer-icons">Icônes du concepteur de diffusion en continu</a></td>
  </tr>
  </tbody>
</table>

* **Liens de réunion pour le Dynamic Chat**: Option permettant d’inclure automatiquement un lien Equipes ou Rencontrer pour Google et Outlook dans chaque invitation calendaire envoyée aux visiteurs.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md">Calendrier</a></td>
  </tr>
  </tbody>
</table>

* **Prise en charge des types de données supplémentaires pour Dynamic Chat**: Trois nouveaux types de données (booléen, entier, flottant) vous permettent d’exploiter davantage de champs de Marketo Engage existants dans Dynamic Chat pour des tâches comme le ciblage en fonction des scores ou la demande de oui/non aux visiteurs.

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

## Annonces {#announcements}

* **Forms 1.0**: L’obsolescence de Forms 1.0 sera terminée avec la version d’octobre. Les ressources Forms 1.0 ne pourront plus envoyer de données à Marketo Engage et renverront des erreurs si elles sont tentées.

* **Forms sans script**: Forms ne fonctionnera plus lorsque JavaScript est désactivé dans le navigateur. L’envoi du formulaire nécessite l’activation de JavaScript.
