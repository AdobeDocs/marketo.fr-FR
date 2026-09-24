---
description: Notes De Mise À Jour - Juillet 2026 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Juillet 2026
feature: Release Information
source-git-commit: a1b00f94acf0fe9cd354a48bf40f17c3ad9b8ae6
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 13%
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
   <td><strong>Nouvelle interface utilisateur de Marketo Engage </strong> : l’interface de Marketo Engage a été actualisée, avec des menus, des icônes et une disposition mis à jour pour une expérience plus épurée et plus moderne. Il s’agit d’une mise à jour visuelle uniquement ; aucune fonctionnalité ou workflow existant n’est affecté.
</td>
   <td>Déploiement échelonné en août et en septembre</td>
   <td><i>s/o</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Serveur MCP Marketo Engage </strong> : le serveur MCP Marketo Engage fait office de pont entre votre assistant AI et Marketo Engage. Il expose plus de 100 opérations sur des formulaires, des programmes, des campagnes intelligentes, des personnes/prospects, des e-mails, des fragments de code, des listes et des dossiers.</td>
   <td>Désormais disponible au public</td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/mcp-server.html" target="_blank">Serveur MCP Marketo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Désactiver les campagnes sur l’archive </strong> : l’archivage d’un dossier désactive et déplanifie désormais toutes les campagnes de cette arborescence de dossiers, empêchant l’exécution inattendue de campagnes intelligentes archivées.
</td>
   <td>Libéré</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders#disable-campaigns-archive" target="_blank">Désactiver les campagnes sur l’archive</a></td>
  </tr>
    <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Menu contextuel Générer le contenu</strong> : les fonctionnalités « Générer le contenu » du Designer Email sont désormais accessibles à partir du menu contextuel (la barre noire). Par exemple, lorsque vous sélectionnez du contenu texte, l’icône Générer du contenu s’affiche dans le menu contextuel, ce qui vous permet d’effectuer des actions rapides.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Marketo AI est désormais Coworker for Marketo Engage** : Coworker for Marketo Engage fournit des compétences d’agent conçues pour automatiser les fonctions marketing qui prennent du temps. Nouveau nom, mêmes fonctionnalités, disponible pour tous les utilisateurs. [En savoir plus](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/coworker-for-marketo/overview){target="_blank"}

* **Obsolescence du paramètre &#39;access_token&#39; de l’API REST** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est obsolète et ne sera plus disponible après le 31 août 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Identifiant d’exécution de campagne de l’API REST** : dans certains cas, la valeur de l’identifiant d’exécution de campagne d’une activité était parfois renvoyée avec un formatage incorrect, entre deux paires de guillemets (par exemple, `"campaignRunId": ""102938""`). <br/>À partir de la version d’août, cette valeur sera toujours renvoyée avec le bon format numérique (`"campaignRunId": 102938`)

* **Limites de taille de liste statique pour les activités Get Lead et Get Lead Changes** : à compter du 30 septembre 2026, les appels aux points d’entrée Get Lead Activities ou Get Lead Changes qui incluent le paramètre `listId` échoueront avec un code d’erreur 1003 (indiquant que la liste statique cible contient trop d’enregistrements) si les listes cibles contiennent 10 000 leads ou plus. Consultez le [ Guide de migration ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} pour plus d’informations.

* **Limite de leads de fusion de l’API REST** : depuis le 31 juillet 2026, les appels qui incluent plus de 25 identifiants dans le paramètre leadIds d’un appel de l’API Merge Leads génèrent un code d’erreur 1080 et l’appel est ignoré. Les tâches nécessitant la fusion de plus de 25 enregistrements en un seul doivent être divisées en plusieurs tâches pour assurer le succès de ces appels.
