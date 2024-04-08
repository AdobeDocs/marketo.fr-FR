---
description: Notes De Mise À Jour - Mars 2024 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Mars 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: fd92f5307880019f54bb2f1778093c110a53ed2c
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 3%

---

# Notes De Mise À Jour : Mars 2024 {#release-notes-mar-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version de mars 2024. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant ou représentante de Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **8 mars 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication peuvent faire l’objet de modifications. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr> 
   <td><strong>Logique de flux de conversation avancée</strong>: ajoutez des champs supplémentaires pour l’évaluation dans un seul choix pour le suivi du flux de conversation.</td> 
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
   <td><strong>Réorganiser la logique du flux de conversation</strong>: dans Marketo Engage Forms, vous pouvez désormais réorganiser les choix de flux de conversation, au lieu d’avoir à les supprimer et à les rajouter.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Paramètres de flux de conversation pour Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Métadonnées d’activité de l’API</strong>: les métadonnées telles que l’agent utilisateur, la plateforme et l’appareil sont désormais incluses dans les activités web et de messagerie électronique, ce qui permet de fournir des informations cohérentes sur ces activités via l’API REST Marketo.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Obtenir le correctif de l’API du membre de programme**: une modification a été apportée récemment pour corriger le comportement du [Obtenir les membres du programme](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} point d’entrée. Auparavant, lors de l’utilisation de `updatedAt` type de filtre pour spécifier une période, il est possible que les enregistrements d’appartenance au programme mis à jour dans cette période n’aient pas été inclus dans la réponse. En outre, il était possible que des enregistrements d’appartenance au programme mis à jour en dehors de la période spécifiée soient incorrectement inclus dans la réponse. Les deux problèmes ont été résolus.

* **Obsolescence du plug-in du navigateur Account Insight**: l’Adobe supprime la gestion de compte Target. [Plug-in du navigateur Account Insight](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on April 8, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
