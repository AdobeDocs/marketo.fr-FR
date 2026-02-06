---
description: Notes De Mise À Jour - Avril 2024 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Avril 2024
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 31%

---

# Notes de mise à jour : avril 2024 {#release-notes-apr-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version d&#39;avril 2024. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 26 avril 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
     <tr>
   <td><strong>Améliorations apportées aux webinaires interactifs</strong> : vous pouvez désormais permettre aux hôtes et aux présentateurs d’ajouter un titre au webinaire, de renommer une salle et de synchroniser manuellement les données d’engagement après la diffusion de l’événement.</td>
   <td>Libéré</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Créer un webinaire interactif</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Synchronisation manuelle</a></li></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Améliorations du journal d'audit</strong> :
   De nouveaux types d’actions peuvent désormais être capturés dans le journal d’audit pour les modifications apportées à la gestion des champs, aux modifications apportées aux utilisateurs et aux rôles, ainsi qu’au nombre de personnes exportées à partir de listes et de listes dynamiques.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Nouvelles autorisations des utilisateurs et des rôles</strong> : de nouvelles autorisations sont disponibles pour fournir aux utilisateurs un accès plus granulaire à Marketo Engage. Contrôlez les parties d’Admin qui n’étaient pas auparavant bloquées, telles que les nouvelles audiences d’expérience et les audiences prédictives, divisez les autorisations pour accorder l’accès à la piste d’audit de ressource et à la piste d’audit d’administrateur séparément, et utilisez les nouvelles autorisations de création et de déplacement pour les ressources et les dossiers afin d’empêcher les utilisateurs en lecture seule d’apporter des modifications.
   <p>Bien que les nouvelles autorisations apparaîtront dans votre instance Marketo Engage à partir du 26 avril, elles sont passives pour l’instant et deviendront accessibles plus tard ce trimestre.
   <li>Accéder à Adobe Experience Manager</li>
   <li>Accéder au mappage d’organisation Adobe</li>
   <li>Accéder au journal d'audit d'administration</li>
   <li>Accéder au journal d’audit des ressources</li>
   <li>Accéder à une nouvelle expérience</li>
   <li>Accès aux audiences prédictives</li>
   <li>Créer un rapport</li>
   <li>Créer une liste</li>
   <li>Exporter l'activité de campagne</li>
   </td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Descriptions des autorisations de rôles</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour de l’API Activities** : le 26 avril, nous ajouterons plusieurs nouveaux attributs aux activités basées sur le web et sur les e-mails qui sont renvoyées lorsque vous récupérez des activités à l’aide de l’API REST [Marketo](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"}. Les activités répertoriées ci-dessous incluent désormais les attributs Navigateur, Plateforme, Appareil et Agent utilisateur. Appelez le point d’entrée [Get Activity Types](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"} pour consulter les détails d’attribut pour chaque activité.

**Activités basées sur le Web**

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:30%">Activité</th>
   <th style="width:70%">Attributs nouvellement ajoutés</th>
   </tr>
  <tr>
   <td>Visit Webpage</td>
   <td>Navigateur, Plateforme, Appareil</td>
  </tr>
   <tr>
   <td>Remplir formulaire</td>
   <td>Navigateur, Plateforme, Appareil</td>
  </tr>
  <tr>
   <td>Cliquer sur lien</td>
   <td>Navigateur, Plateforme, Appareil</td>
  </tr>
 </tbody>
</table>

**Activités par e-mail**

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:30%">Activité</th>
   <th style="width:70%">Attributs nouvellement ajoutés</th>
  </tr>
   <tr>
   <td>Envoyer un e-mail</td>
   <td>Navigateur, Plateforme, Appareil, Agent Utilisateur</td>
  </tr>
   </tr>
  <tr>
   <td>E-mail remis au destinataire</td>
   <td>Navigateur, Plateforme, Appareil, Agent Utilisateur</td>
  </tr>
   <tr>
   <td>E-mail renvoyé</td>
   <td>Navigateur, Plateforme, Appareil, Agent Utilisateur</td>
  </tr>
  <tr>
   <td>Se désabonner des e-mails</td>
   <td>Navigateur, Plateforme, Appareil</td>
  </tr>
  <tr>
   <td>Ouvrir e-mail</td>
   <td>Navigateur</td>
  </tr>
   <tr>
   <td>Cliquer sur l’e-mail</td>
   <td>Navigateur</td>
  </tr>
  <tr>
   <td>E-mail renvoyé provisoirement</td>
   <td>Navigateur, Plateforme, Appareil, Agent Utilisateur</td>
  </tr>
 </tbody>
</table>
