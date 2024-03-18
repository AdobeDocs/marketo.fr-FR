---
description: Notes de mise à jour actuelles - Documentation de Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: cfbf9206bcb0e54abdbd962e52844bba11b07197
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 6%

---

# Notes de mise à jour : mars 2024 {#release-notes-mar-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 mars. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **8 mars 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr> 
   <td><strong>Logique avancée du flux de conversation</strong>: ajoutez des champs supplémentaires à évaluer dans un seul choix pour le suivi du flux de conversation.</td> 
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
   <td><strong>Réorganiser la logique de flux de conversation</strong>: dans Marketo Engage Forms, vous pouvez désormais réorganiser les choix de flux de conversation, au lieu d’avoir à les supprimer et à les ajouter à nouveau.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Paramètres de flux de conversation pour Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Métadonnées d’activité de l’API</strong>: des métadonnées telles que l’agent utilisateur, la plateforme et l’appareil sont désormais incluses dans les activités web et de courrier électronique, ce qui permet d’obtenir des informations homogènes sur ces activités via l’API REST Marketo.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Obtenir le correctif de l’API des membres du programme**: une modification a été apportée récemment pour corriger le comportement de la variable [Obtention des membres du programme](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} point de terminaison . Auparavant, lors de l’utilisation de la variable `updatedAt` type de filtre pour spécifier une période, il était possible que les enregistrements d’appartenance au programme mis à jour au cours de cette période n’aient pas été inclus dans la réponse. En outre, il était possible que les enregistrements d’adhésion au programme mis à jour en dehors de la période spécifiée soient incorrectement inclus dans la réponse. Les deux problèmes ont été résolus.

* **Abandon du module du navigateur Insight de compte**: Adobe supprime la gestion de compte Target [Module externe de navigateur Insight de compte](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on March 18, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
