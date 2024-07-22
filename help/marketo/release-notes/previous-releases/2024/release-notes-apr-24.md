---
description: Notes de mise à jour - Avril 2024 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Avril 2024
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 8%

---

# Notes de mise à jour : avril 2024 {#release-notes-apr-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 avril. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques au Adobe Dynamic Chat [ se trouvent ici ](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **26 avril 2024**, avec un déploiement progressif des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
     <tr> 
   <td><strong>Améliorations apportées aux webinaires interactifs</strong> : vous pouvez désormais fournir aux hôtes et aux présentateurs la possibilité d’ajouter un titre de webinaire, de renommer une salle et de synchroniser manuellement les données d’engagement après la diffusion de l’événement.</td> 
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
   <td><strong>Améliorations du journal d’audit</strong> : 
   De nouveaux types d’actions peuvent désormais être capturés dans le journal d’audit pour les modifications apportées à la gestion des champs, les modifications apportées aux utilisateurs et aux rôles, ainsi que le nombre de personnes exportées à partir de listes et de listes dynamiques.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Autorisations des nouveaux utilisateurs et rôles</strong> : de nouvelles autorisations sont disponibles, ce qui permet aux utilisateurs d’accéder plus précisément au Marketo Engage. Les parties de contrôle de l’administrateur qui n’étaient pas jusque-là sécurisées, telles que Nouvelle expérience et Audiences prédictives, partagent les autorisations pour accorder l’accès au journal d’audit des ressources et au journal d’audit de l’administrateur séparément, et utilisent de nouvelles autorisations de création et de déplacement pour les ressources et les dossiers afin d’empêcher les utilisateurs en lecture seule d’apporter des modifications. 
   <p>Bien que les nouvelles autorisations s’affichent dans votre instance de Marketo Engage à compter du 26 avril, elles sont passives pour l’instant et deviennent accessibles plus tard ce trimestre.
   <li>Accès à Adobe Experience Manager</li>
   <li>Mappage de l’organisation d’accès</li>
   <li>Accéder au journal d’audit de l’administrateur</li>
   <li>Accéder au journal d’audit des ressources</li>
   <li>Accès à une nouvelle expérience</li>
   <li>Accès aux audiences prédictives</li>
   <li>Créer un rapport</li>
   <li>Créer une liste</li>
   <li>Exporter l’activité de campagne</li>
   </td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Descriptions des autorisations de rôle</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour de l’API d’activités** : le 26 avril, nous ajoutons plusieurs nouveaux attributs aux activités web et par e-mail qui sont renvoyés lorsque vous récupérez des activités à l’aide de l’ [’&#39;API REST Marketo](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"}. Les activités répertoriées ci-dessous comprennent désormais les attributs Navigateur, Plateforme, Appareil et Agent utilisateur. Appelez le point de terminaison [Get Activity Types](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"} pour passer en revue les détails d’attribut pour chaque activité.

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

**Activités basées sur un e-mail**

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
