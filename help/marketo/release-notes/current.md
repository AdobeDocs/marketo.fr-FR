---
description: Notes de mise à jour actuelles - Documentation de Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 11%

---

# Notes de mise à jour : avril 2024 {#release-notes-apr-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 avril. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

Notes de mise à jour spécifiques à Adobe Dynamic Chat [peut être consulté ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **26 avril 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
     <tr> 
   <td><strong>Améliorations des webinaires interactifs</strong>: vous pouvez désormais fournir aux hôtes et aux présentateurs la possibilité d’ajouter un titre de webinaire, de renommer une salle et de synchroniser manuellement les données d’engagement après la diffusion de l’événement.</td> 
   <td>Expédié</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Création d’un webinaire interactif</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Synchronisation manuelle</a></li></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Améliorations du journal d’audit</strong>: de nouveaux types d’actions peuvent désormais être capturés dans le journal d’audit pour les modifications apportées à la gestion des champs, les modifications apportées aux utilisateurs et aux rôles, ainsi que le nombre de personnes exportées à partir de listes et de listes dynamiques.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Nouvelles autorisations d’utilisateurs et de rôles</strong>: de nouvelles autorisations sont disponibles, ce qui donne aux utilisateurs un accès plus granulaire à Marketo Engage. Les parties de contrôle de l’administrateur qui n’étaient pas jusque-là sécurisées, telles que Nouvelle expérience et Audiences prédictives, partagent les autorisations pour accorder l’accès au journal d’audit des ressources et au journal d’audit de l’administrateur séparément, et utilisent de nouvelles autorisations de création et de déplacement pour les ressources et les dossiers afin d’empêcher les utilisateurs en lecture seule d’apporter des modifications. Bien que les nouvelles autorisations s’affichent dans votre instance de Marketo Engage à compter du 26 avril, elles sont passives pour l’instant et deviennent accessibles plus tard ce trimestre.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Descriptions des autorisations de rôle</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour de l’API d’activités**: le 26 avril, nous ajoutons plusieurs nouveaux attributs aux activités web et par e-mail qui sont renvoyées lorsque vous récupérez des activités à l’aide de la variable [API REST MARKETO](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} point de terminaison pour consulter les détails des attributs de chaque activité.

**Activités Web**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">Activité</th> 
   <th style="width:70%">Attributs nouvellement ajoutés</th>
   </tr>
  <tr> 
   <td>Visit Webpage</td> 
   <td>Navigateur, plateforme, périphérique</td>
  </tr>
   <tr> 
   <td>Remplir formulaire</td> 
   <td>Navigateur, plateforme, périphérique</td>
  </tr>
  <tr> 
   <td>Cliquer sur lien</td> 
   <td>Navigateur, plateforme, périphérique</td>
  </tr>
 </tbody> 
</table>

**Activités basées sur le courrier électronique**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">Activité</th> 
   <th style="width:70%">Attributs nouvellement ajoutés</th>
  </tr>
   <tr> 
   <td>Envoyer un e-mail</td> 
   <td>Browser, Platform, Device, User Agent</td>
  </tr>
   </tr>
  <tr> 
   <td>E-mail remis au destinataire</td> 
   <td>Browser, Platform, Device, User Agent</td>
  </tr>
   <tr> 
   <td>E-mail renvoyé</td> 
   <td>Browser, Platform, Device, User Agent</td>
  </tr>
  <tr> 
   <td>Se désabonner des e-mails</td> 
   <td>Navigateur, plateforme, périphérique</td>
  </tr>
  <tr> 
   <td>Ouvrir e-mail</td> 
   <td>Navigateur</td>
  </tr>
   <tr> 
   <td>Cliquer sur e-mail</td> 
   <td>Navigateur</td>
  </tr>
  <tr> 
   <td>E-mail renvoyé provisoirement</td> 
   <td>Browser, Platform, Device, User Agent</td>
  </tr>
 </tbody> 
</table>
