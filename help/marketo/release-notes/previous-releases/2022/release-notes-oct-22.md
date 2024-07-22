---
description: Notes de mise à jour - Octobre 2022 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Octobre 2022
exl-id: 1494b8b9-049c-4969-ab95-a4be41d886b0
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 6%

---

# Notes de mise à jour : octobre 2022 {#release-notes-oct-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 octobre. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **14 octobre 2022**, avec un déploiement progressif des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonctionnalité ci-dessous.

### Environnement de données marketing {#marketing-data-environment}

</br>

* **Synchronisation des champs personnalisés des membres du programme** : possibilité de synchroniser de manière bidirectionnelle les champs extensibles capturés pour un membre du programme (par exemple, les préférences du participant lors de l’enregistrement de l’événement, comme la nourriture, les sessions, les suivis, etc.) avec des champs de membre Campaign dans Salesforce.

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

* **Intégration de Privacy Service Adobe** : harmonisation avec Privacy Service pour automatiser la conformité aux réglementations de confidentialité des données dans les produits Experience Cloud. Actuellement, ce service n’est disponible que pour les clients Marketo Engage intégrés au système Identity Management Adobe.

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

* **Mise à jour de Screens dans l’expérience de nouvelle génération** : nous proposons des écrans supplémentaires actualisés dans l’expérience de nouvelle génération qui offrent une mise à jour de la conception et de la convivialité, accessibles par basculement :

   * Détails du modèle de page d’entrée
   * Liste des modèles de courrier électronique

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Basculer/Basculer</a></td>
  </tr>
  </tbody>
</table>

* **Onglet Utilisation améliorée par dans les détails du modèle de courrier électronique** : dans la nouvelle expérience, vous verrez des informations supplémentaires relatives aux ressources à l’aide du modèle de courrier électronique, notamment l’état des ressources, la dernière modification et la dernière modification par. Vous pouvez également rechercher, trier et filtrer la liste des ressources utilisées.

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

* **Modèles de filtre de ressources de rapport** : nouvelle conception des modèles de configuration de rapport affichant une nouvelle arborescence de ressources dans le menu de configuration et un filtre pour la date de création et de modification.

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

* **Importation de pistes en bloc : association de vendeurs** : parité avec l’API REST de piste pour pouvoir associer des pistes aux vendeurs au cours du processus d’importation de pistes en bloc, ce qui réduit la complexité et le nombre d’appels d’API requis.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Importation de pistes en bloc</a></td>
  </tr>
  </tbody>
</table>

### Sales Insight {#sales-insight}

</br>

![(star)](assets/yellow-star.png)

* **Intégration de Sales Insight avec Dynamic Chat** : le tableau de bord Insights inclut désormais les activités de Dynamic Chat dans la grille dynamique, ainsi qu’un résumé hebdomadaire et des cartes détaillées.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Intégration du Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Fonctionnalités de version agile

Les fonctionnalités suivantes suivent un format Agile et sont publiées à diverses dates avant ou après la date de publication standard. Vérifiez l’état de chaque fonctionnalité ci-dessous.

* **Réorganiser automatiquement les flux de dialogue pour les Dynamic Chat** : améliorez votre canevas de dialogue surpeuplé en organisant tout sur la zone de travail dans un format propre et facile à lire en appuyant sur un bouton via Réorganiser automatiquement.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Icônes de diffusion Designer</a></td>
  </tr>
  </tbody>
</table>

* **Liens de réunion pour Dynamic Chat** : option permettant d’inclure automatiquement un lien de réunion ou de réunion pour Google et Outlook dans chaque invitation à calendrier envoyée aux visiteurs.

<table> 
  <tr> 
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Calendrier</a></td>
  </tr>
  </tbody>
</table>

* **Prise en charge de types de données supplémentaires pour Dynamic Chat** : trois nouveaux types de données (booléen, entier, flottant) vous permettent d’exploiter davantage de champs de Marketo Engage existants dans Dynamic Chat pour des tâches telles que le ciblage en fonction des scores ou la question &quot;oui/non&quot; aux visiteurs.

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

* **Forms 1.0** : l’obsolescence de Forms 1.0 sera terminée avec la version d’octobre. Les ressources Forms 1.0 ne pourront plus envoyer de données à Marketo Engage et renverront des erreurs si elles sont tentées.

* **Forms sans script** : Forms ne fonctionnera plus lorsque JavaScript est désactivé dans le navigateur. L’envoi du formulaire nécessite l’activation de JavaScript.
