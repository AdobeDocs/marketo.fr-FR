---
description: Notes De Mise À Jour - Octobre 2022 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Octobre 2022
exl-id: 1494b8b9-049c-4969-ab95-a4be41d886b0
feature: Release Information
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 21%

---

# Notes de mise à jour : octobre 2022 {#release-notes-oct-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 octobre. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 14 octobre 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Veuillez vérifier ci-dessous chaque fonctionnalité pour connaître son statut.

### Environnement de données marketing {#marketing-data-environment}

</br>

* **Synchronisation des champs personnalisés des membres de programme** : possibilité de synchroniser de manière bidirectionnelle les champs extensibles capturés pour un membre de programme (par exemple, les préférences du participant lors de l’enregistrement à un événement, telles que la nourriture, les sessions, les suivis, etc.) avec les champs des membres de campagne dans Salesforce.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Synchronisation des champs personnalisés des personnes membres du programme</a></td>
  </tr>
  </tbody>
</table>

* **Intégration d’Adobe Privacy Service** : harmonisez-le avec Privacy Service afin d’automatiser la conformité aux réglementations de confidentialité des données sur l’ensemble des produits Experience Cloud. Actuellement, ce service n’est disponible que pour les clients Marketo Engage qui ont intégré le système Adobe Identity Management.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Expérience nouvelle génération {#modern-ux}

</br>

* **Mise à jour de Screens dans l’expérience de nouvelle génération** : nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour et accessibles via le bouton bascule :

   * Détails du modèle de page de destination
   * Liste de modèles d’e-mail

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Bouton (bascule)</a></td>
  </tr>
  </tbody>
</table>

* **Amélioration de l’onglet Utilisé par dans les Détails du modèle d’e-mail** : dans la nouvelle expérience, vous verrez des informations supplémentaires relatives aux ressources utilisant le modèle d’e-mail, y compris le statut de la ressource, Dernière modification et Dernière modification par. Vous pouvez également rechercher, trier et filtrer la liste des utilisés par les ressources.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

* **Modales de filtre des ressources de rapport** : nouvelle conception pour les modèles de configuration de rapport affichant une nouvelle arborescence de ressource dans le menu de configuration et un filtre pour les dates de création et de modification.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

### Améliorations de l’API {#api-enhancements}

</br>

* **Importation de leads en bloc : association des vendeurs** : parité avec l’API REST de lead pour pouvoir associer des leads aux vendeurs pendant le processus d’importation de leads en bloc, ce qui réduit la complexité et le nombre d’appels d’API requis.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Importation de leads en bloc</a></td>
  </tr>
  </tbody>
</table>

### Sales Insight {#sales-insight}

</br>

![(étoile)](assets/yellow-star.png)

* **Intégration de Sales Insight à Dynamic Chat** : le tableau de bord Insights comprend désormais les activités Dynamic Chat dans la grille dynamique, ainsi qu’un résumé hebdomadaire et des cartes détaillées.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Intégration de Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Fonctionnalités de mise à jour d’Agile

Les fonctionnalités suivantes suivent un format Agile et sont publiées à différentes dates avant ou après la date de publication standard. Veuillez vérifier ci-dessous chaque fonctionnalité pour connaître son statut.

* **Réorganiser automatiquement les flux de dialogue pour Dynamic Chat** : améliorez votre zone de travail de boîte de dialogue encombrée en organisant tous les éléments de la zone de travail dans un format propre et facile à lire en appuyant sur un bouton via Réorganiser automatiquement.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Icônes de diffusion Designer</a></td>
  </tr>
  </tbody>
</table>

* **Liens de réunion pour Dynamic Chat** : option permettant d’inclure automatiquement un lien Équipes ou Réunion pour Google et Outlook dans chaque invitation de calendrier envoyée aux visiteurs.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Calendrier</a></td>
  </tr>
  </tbody>
</table>

* **Prise en charge de types de données supplémentaires pour Dynamic Chat** : trois nouveaux types de données (booléen, entier, flottant) vous permettent d’exploiter davantage de champs Marketo Engage existants dans Dynamic Chat pour des choses telles que le ciblage basé sur les scores ou le fait de poser des questions oui/non aux visiteurs.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

## Annonces {#announcements}

* **Forms 1.0** : l’obsolescence de Forms 1.0 sera terminée avec la version d’octobre. Les ressources de Forms 1.0 ne pourront plus envoyer de données à Marketo Engage et renverront des erreurs si elles sont tentées.

* **No-Script Forms** : Forms ne fonctionnera plus lorsque JavaScript sera désactivé dans le navigateur. L’envoi du formulaire nécessite l’activation de JavaScript.
