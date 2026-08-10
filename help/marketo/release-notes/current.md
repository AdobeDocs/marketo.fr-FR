---
description: Notes de mise à jour actuelles - Documentation Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 618fe38fae7621ecf72aab8ec09fc345aba23358
workflow-type: tm+mt
source-wordcount: 434
ht-degree: 21%

---

# Notes De Mise À Jour : Août 2026 {#release-notes-aug-26}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 26 août. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **14 août 2026**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Nouvelle interface utilisateur de Marketo Engage </strong> : l’interface de Marketo Engage a été actualisée, avec des menus, des icônes et une disposition mis à jour pour une expérience plus épurée et plus moderne. Il s’agit d’une mise à jour visuelle uniquement, aucune fonctionnalité ou workflow existant n’est affecté.
</td>
   <td>Déploiement échelonné tout au long du mois d’août</td>
   <td><i>s/o</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Créateur de scripts</strong> : le créateur de scripts est un assistant optimisé par l’IA qui vous permet de créer des scripts de personnalisation plus rapidement.
</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Désactiver les campagnes sur l’archive </strong> : l’archivage d’un dossier désactive et déplanifie désormais toutes les campagnes de cette arborescence de dossiers, empêchant l’exécution inattendue de campagnes intelligentes archivées.
</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 31 août 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Identifiant d’exécution de campagne de l’API REST** : dans certains cas, la valeur de l’identifiant d’exécution de campagne d’une activité était parfois renvoyée avec un formatage incorrect, entre deux paires de guillemets (par exemple, `"campaignRunId": ""102938""`). <br/>À partir de la version d’août, cette valeur sera toujours renvoyée avec le bon format numérique (`"campaignRunId": 102938`)

* **Limites de taille de liste statique pour les activités Get Lead et Get Lead Changes** : à compter du 30 septembre 2026, les appels aux points d’entrée Get Lead Activities ou Get Lead Changes qui incluent le paramètre `listId` échoueront si les listes cibles contiennent 10 000 leads ou plus avec un code d’erreur 1003 indiquant que la liste statique cible contient trop d’enregistrements. Consultez le [ Guide de migration ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} pour plus d’informations.

* **Limite de leads de fusion de l’API REST** : depuis le 31 juillet 2026, les appels qui incluent plus de 25 identifiants dans le paramètre leadIds d’un appel de l’API Merge Leads génèrent un code d’erreur 1080 et l’appel est ignoré. Les tâches nécessitant la fusion de plus de 25 enregistrements en un seul doivent être divisées en plusieurs tâches pour assurer le succès de ces appels.
