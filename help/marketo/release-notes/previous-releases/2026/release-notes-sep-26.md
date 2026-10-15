---
description: Notes De Mise À Jour - Septembre 2026 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Septembre 2026
feature: Release Information
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
subfeature_v2:
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
source-git-commit: 9eb8c0e78a581bc9093f0f017a3ad3525d2b9667
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 14%
---
# Notes De Mise À Jour : Septembre 2026 {#release-notes-sep-26}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 26 septembre. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **25 septembre 2026**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Nouvelle interface utilisateur de Marketo Engage </strong> : l’interface de Marketo Engage a été actualisée, avec des menus, des icônes et une disposition mis à jour pour une expérience plus épurée et plus moderne. Il s’agit d’une mise à jour visuelle uniquement ; aucune fonctionnalité ou workflow existant n’est affecté. <i>La possibilité de sélectionner l’interface utilisateur classique sera disponible dans la version de janvier 2027</i>.
</td>
   <td>Disponibilité générale à la mi-octobre</td>
   <td><i>s/o</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Sélectionner la partition à l’importation </strong> : vous pouvez désormais effectuer une sélection dans la liste de partitions de l’espace de travail local lors de l’importation d’enregistrements de personne dans des environnements où les espaces de travail et les partitions sont activés.</td>
   <td>Libéré</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people#step-import-your-spreadsheet-into-marketo:~:text=If%20you%20have%20Person%20Partitions%20set%20up" target="_blank">Import de liste</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Étapes de flux en libre-service - Délai d’expiration de rappel augmenté </strong> : le délai d’expiration de rappel des étapes de flux en libre-service passe d’une heure à quatre heures. Aucune action n’est requise de votre part.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Tableaux</strong> : vous pouvez désormais glisser-déposer le type de contenu « tableau » dans votre e-mail, avec la possibilité de définir le nombre de colonnes et de lignes.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Restrictions de nom d’API pour les attributs d’activité personnalisés** : les noms d’API pour les attributs d’activité personnalisés créés via l’API ou l’interface utilisateur peuvent désormais uniquement contenir des caractères alphanumériques et des traits de soulignement et doivent commencer par un caractère alphanumérique.

* **Limites de taille de liste statique pour les activités Get Lead et Get Lead Changes** : à compter du 30 septembre 2026, les appels aux points d’entrée Get Lead Activities ou Get Lead Changes qui incluent le paramètre `listId` échoueront avec un code d’erreur 1003 (indiquant que la liste statique cible contient trop d’enregistrements) si les listes cibles contiennent 10 000 leads ou plus. Consultez le [&#x200B; Guide de migration &#x200B;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} pour plus d’informations.

* **Obsolescence du paramètre &#39;access_token&#39; de l’API REST** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est obsolète depuis le 31 août 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **ID d’exécution de campagne de l’API REST** : dans certains cas, la valeur de l’ID d’exécution de campagne d’une activité était parfois renvoyée avec un formatage incorrect, entre deux paires de guillemets (par exemple, `"campaignRunId": ""102938""`). <br/>À compter de la version d’août, cette valeur sera toujours renvoyée avec le bon format numérique (`"campaignRunId": 102938`).

* **Obsolescence des images capturées sur le web** : pour se conformer aux bonnes pratiques modernes en matière de sécurité et de confidentialité, la fonctionnalité [Capturer des images sur le web](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"} sera abandonnée à compter de la version d’octobre.
