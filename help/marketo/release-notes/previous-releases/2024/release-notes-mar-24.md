---
description: Notes De Mise À Jour - Mars 2024 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Mars 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 30%

---

# Notes de mise à jour : mars 2024 {#release-notes-mar-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version de mars 2024. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 8 mars 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Logique de flux de conversation avancée</strong> : ajoutez des champs supplémentaires pour l’évaluation dans un seul choix pour le suivi du flux de conversation.</td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Paramètres de flux conversationnel pour Marketo Engage Forms</a></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr>
   <td><strong>Réorganiser la logique de flux de conversation</strong> : dans Marketo Engage Forms, vous pouvez désormais réorganiser les choix de flux de conversation, au lieu d’avoir à les supprimer et à les rajouter.</td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Paramètres de flux conversationnel pour Marketo Engage Forms</a></td>
   </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Métadonnées d’activité de l’API</strong> :
   Les métadonnées telles que l’agent utilisateur, la plateforme et l’appareil sont désormais incluses dans les activités web et de messagerie électronique, ce qui permet de fournir des informations cohérentes sur ces activités via l’API REST Marketo.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
 </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Correctif API Get Program Member** : une modification a été récemment apportée pour corriger le comportement du point d’entrée [Get Program Members](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}. Auparavant, lorsque vous utilisiez le type de filtre `updatedAt` pour spécifier une période, il était possible que les enregistrements d’appartenance au programme mis à jour dans cette période ne soient pas inclus dans la réponse. En outre, il était possible que les enregistrements d’appartenance au programme mis à jour en dehors de la période spécifiée soient incorrectement inclus dans la réponse. Les deux problèmes ont été résolus.

* **Obsolescence du plug-in de navigateur Insight de compte** : Adobe supprime le [plug-in de navigateur Insight de compte](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} de la gestion de compte Target de la boutique en ligne Chrome le 8 avril 2024. Utilisateurs existants : vous pouvez continuer à utiliser le plug-in jusqu’à ce que vous migriez votre instance Marketo Engage vers Adobe Identity et Admin Console. Cette modification **n’aura aucune incidence** sur les autres fonctionnalités/données TAM de Marketo Engage ou sur les plug-ins de messagerie Chrome et Outlook qui fonctionnent avec Sales Insight. [En savoir plus](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
