---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: d26428137e9b99d04fef67a3b21b74d150f693e7
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Notes de mise à jour : Octobre 2022 {#release-notes-oct-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 octobre. Vérifiez la disponibilité de votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

Les fonctionnalités suivantes commenceront à être publiées sur **14 octobre 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire). Les fonctionnalités de publication et les dates exactes peuvent être modifiées.

## Orchestration cross-canal {#cross-channel-orchestration}

* **Organiser automatiquement les flux de dialogue pour la conversation dynamique**: Améliorez votre canevas de dialogue bondé en organisant tout sur la zone de travail dans un format propre et facile à lire en appuyant sur un bouton via l’option Réorganiser automatiquement.

* **Prise en charge des types de données supplémentaires pour Dynamic Chat**: Trois nouveaux types de données (booléen, entier, flottant) vous permettent d’exploiter d’autres champs de Marketo Engage existants dans Dynamic Chat pour des tâches comme le ciblage en fonction des scores ou la demande de questions oui/non aux visiteurs.

* **Liens de réunion pour la conversation dynamique**: Option permettant d’inclure automatiquement un lien Equipes ou Rencontrer pour Google et Outlook dans chaque invitation calendaire envoyée aux visiteurs.

* **Notifications de réunion planifiées pour la messagerie instantanée**: Les représentants commerciaux reçoivent des notifications par e-mail automatisées concernant les réunions planifiées ainsi que toute information pertinente sur l’interaction de chatbot du visiteur.

* **Rôles et autorisations pour Dynamic Chat**: Les administrateurs peuvent utiliser des autorisations granulaires pour contrôler la visibilité et l’utilisation de l’application et créer des rôles utilisateur personnalisés.

   * Accès complet : les utilisateurs peuvent profiter pleinement de cette fonctionnalité (par exemple, publier des boîtes de dialogue, changer de modèle de couleur, etc.)
   * Accès en lecture seule : les utilisateurs peuvent consulter les informations mais ne peuvent pas apporter de modifications (par exemple, voir Critères d’audience ou Concepteur de diffusion en continu, mais pas modifier).
   * Accès restreint : les utilisateurs ne peuvent pas afficher ni accéder aux sections Configuration ou Intégrations .

## Expérience de nouvelle génération {#next-generation-experience}

* **Mise à jour d’Screens dans l’expérience de nouvelle génération**: Nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour, accessibles par le biais d’un bouton d’activation/désactivation :

   * Détails du modèle de page d’entrée
   * Liste des modèles de courrier électronique

* **Amélioration de l’option Utilisé par l’onglet Détails du modèle de courrier électronique**: Dans la nouvelle expérience, vous verrez des informations supplémentaires relatives aux ressources à l’aide du modèle de courrier électronique, notamment Asset Status (État de la ressource), Last Modified (Dernière modification) et Last Modified By (Dernière modification). Vous pouvez également rechercher, trier et filtrer la liste des ressources utilisées.

* **Modèles de filtre de ressources de rapport**: Nouvelle conception des modèles de configuration de rapport affichant une nouvelle arborescence de ressources dans le menu de configuration et un filtre pour Date de création et de modification.

## Environnement de données marketing {#marketing-data-environment}

* **Intégration d’Adobe Privacy Service**: Harmonisez-vous avec Privacy Service afin d’automatiser la conformité aux réglementations de confidentialité des données dans les produits Experience Cloud. Actuellement, ce service n’est disponible que pour les clients Marketo Engage qui ont intégré le [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md)Système {target=&quot;_blank&quot;}.

* **Synchronisation des champs personnalisés des membres du programme**: Possibilité de synchroniser de manière bidirectionnelle les champs extensibles capturés pour un membre du programme (par exemple, les préférences du participant lors de l’enregistrement de l’événement, tels que la nourriture, les sessions, les suivis, etc.)

## Améliorations des API {#api-enhancements}

* **Importation de pistes en bloc : Association des vendeurs**: Parité avec l’API REST Lead pour pouvoir associer des prospects aux vendeurs au cours du processus d’importation de prospects en masse, ce qui réduit la complexité et le nombre d’appels API requis.

## Annonces {#announcements}

* **Forms 1.0**: L’obsolescence de Forms 1.0 sera terminée avec la version d’octobre. Les ressources Forms 1.0 ne pourront plus envoyer de données à Marketo Engage et renverront des erreurs si elles sont tentées.

* **Forms sans script**: Forms ne fonctionnera plus lorsque JavaScript est désactivé dans le navigateur. L’envoi du formulaire nécessite l’activation de JavaScript.
