---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 7853491f53bd2f7d5ec6e63189c1e8b77b4b5349
workflow-type: tm+mt
source-wordcount: 543
ht-degree: 23%

---

# Notes De Mise À Jour : Mai 2026 {#release-notes-may-26}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 26 mai. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **22 mai 2026**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Marketo AI</strong> : utilisez une suite d’agents conçus pour automatiser les fonctions marketing longues mais importantes (deux agents disponibles maintenant, d’autres seront bientôt disponibles).
</td>
   <td>Disponibilité limitée (<a href="https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode">demander l'accès ici</a>)</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/overview">Présentation de Marketo AI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Serveur MCP Marketo Engage </strong> : le serveur MCP Marketo Engage fait office de pont entre votre assistant AI et Marketo Engage. Il expose plus de 100 opérations sur des formulaires, des programmes, des campagnes intelligentes, des personnes/prospects, des e-mails, des fragments de code, des listes et des dossiers.</td>
   <td>Disponibilité limitée (<a href="https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode">demander l'accès ici</a>)</td>
   <td><a href="https://experienceleague.corp.adobe.com/docs/marketo-developer/marketo/mcp-server.html">Serveur MCP Marketo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td>Designer d’e-mail - Contenu conditionnel pour les fragments d’e-mail</strong> : <i>Parité avec l’ancien éditeur d’e-mail</i>. <strong>Le contenu conditionnel est désormais pris en charge pour les fragments.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Gestion des listes de sélection</strong> : vous pouvez désormais spécifier les valeurs qui peuvent être utilisées dans les champs de Marketo Engage.
   </td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Champs d’obsolescence des fonctionnalités sociales** : en 2025, Marketo Engage a abandonné les fonctionnalités sociales suivantes :

   * Sondages
   * Bouton social
   * Offre de parrainage
   * Partage de vidéos
   * Loteries

Plus tôt cette année, les champs connexes qui avaient été laissés en arrière-plan ont été supprimés de Marketo. Peu après, les requêtes d’API référençant certains champs de prospect liés aux réseaux sociaux ont renvoyé une erreur « champ introuvable », provoquant des interruptions. Le service a été restauré après la remise à disposition des champs concernés. Afin d’éviter toute perturbation supplémentaire, Marketo a donc découplé définitivement les champs des réseaux sociaux de l’obsolescence des fonctionnalités des réseaux sociaux (qui seront donc disponibles dans votre compte Marketo). Nous recommandons aux utilisateurs de passer en revue les requêtes d’API et les intégrations qui font référence à des champs liés à Marketo Social et de déterminer si ces champs sont toujours requis pour les processus métier en cours.

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 31 juillet 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 juillet 2026. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Limites de taille de liste statique pour les activités Get Lead et Get Lead Changes** : à compter du 30 septembre 2026, les appels aux points d’entrée Get Lead Activities et Get Lead Changes qui incluent le paramètre `listId` renverront un code d’erreur 1003 si la liste statique cible contient 10 000 leads ou plus. Consultez le [&#x200B; Guide de migration &#x200B;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} pour plus d’informations.
