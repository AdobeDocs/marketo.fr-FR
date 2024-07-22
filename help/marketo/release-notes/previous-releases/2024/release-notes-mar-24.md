---
description: Notes de mise à jour - Mars 2024 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Mars 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 2%

---

# Notes de mise à jour : mars 2024 {#release-notes-mar-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 mars. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **8 mars 2024**, avec un déploiement progressif des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr> 
   <td><strong>Logique de flux de conversation avancé</strong> : ajoutez des champs supplémentaires pour l’évaluation dans un choix unique pour le suivi du flux de conversation.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Paramètres de flux de conversation pour Marketo Engage Forms</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Réorganiser la logique de flux de conversation</strong> : dans Marketo Engage Forms, vous pouvez désormais réorganiser les choix de flux de conversation, au lieu d’avoir à supprimer et à ajouter à nouveau.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Paramètres de flux de conversation pour Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Métadonnées d’activité de l’API</strong> : 
   Des métadonnées telles que Agent utilisateur, Plateforme et Appareil sont désormais incluses dans les activités web et de courrier électronique, ce qui permet d’obtenir des informations homogènes sur ces activités via l’API REST Marketo.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Get Program Member API Fix** : une modification a été apportée récemment pour corriger le comportement du point de terminaison [Get Program Members](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}. Auparavant, lors de l’utilisation du type de filtre `updatedAt` pour spécifier une plage de dates, il était possible que les enregistrements d’appartenance au programme mis à jour dans cette plage ne soient pas inclus dans la réponse. En outre, il était possible que les enregistrements d’adhésion au programme mis à jour en dehors de la période spécifiée soient incorrectement inclus dans la réponse. Les deux problèmes ont été résolus.

* **Abandon du module de navigateur Insight Account** : Adobe supprime le [ module de navigateur de gestion de compte Insight ](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} du magasin Web Chrome le 8 avril 2024. Utilisateurs existants : vous pouvez continuer à utiliser le plug-in jusqu’à ce que vous migriez votre instance de Marketo Engage vers Adobe Identity et Admin Console. Cette modification **n’aura aucune incidence** sur les autres fonctionnalités/données TAM dans Marketo Engage ou les modules externes de messagerie Chrome et Outlook qui fonctionnent avec Sales Insight. [En savoir plus](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
