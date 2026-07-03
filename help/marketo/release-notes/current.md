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
source-git-commit: 7ed34709d2a8b8ab3922a62d043bcdfa8e2d33ce
workflow-type: tm+mt
source-wordcount: 483
ht-degree: 22%

---

# Notes de mise à jour : #1 de juillet 2026 sur 2 {#release-notes-july-26-one}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la première version du 26 juillet. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **10 juillet 2026**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Compétences en IA dédiée à Marketo - Connaissance des produits </strong> : la connaissance des produits vous donne un accès à la demande à l’expertise de Marketo sans quitter la plateforme. Posez une question en langage clair et l’IA dédiée à Marketo s’appuie sur la documentation officielle d’Adobe pour y répondre.</td>
   <td>Ouvrir la version bêta</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">Présentation de Marketo AI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Compétences en IA dédiée à Marketo - Rechercher des prospects </strong> : découvrez pourquoi une personne/un prospect spécifique n’a pas atteint un jalon (comme MQL, qualification d’un programme ou une campagne) et obtenez une explication en langage clair de ce qui s’est passé.
</td>
   <td>Ouvrir la version bêta</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Présentation de Marketo AI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Menu contextuel de l'assistant AI</strong> : les fonctionnalités de l'assistant AI du Designer Email sont désormais accessibles à partir du menu contextuel (la barre noire). Par exemple, lorsque vous sélectionnez du contenu texte, l’icône de l’assistant d’IA s’affiche dans le menu contextuel, ce qui vous permet d’effectuer des actions rapides à partir de cet emplacement.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 31 juillet 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Limite de leads de fusion de l’API REST** : à compter du 31 juillet 2026, les appels qui incluent plus de 25 identifiants dans le paramètre leadIds d’un appel de l’API Merge Leads entraîneront un code d’erreur 1080 et l’appel sera ignoré. Les tâches nécessitant la fusion de plus de 25 enregistrements en un seul doivent être divisées en plusieurs tâches pour assurer le succès de ces appels.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 juillet 2026. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Limites de taille de liste statique pour les activités Get Lead et Get Lead Changes** : à compter du 30 septembre 2026, les appels aux points d’entrée Get Lead Activities et Get Lead Changes qui incluent le paramètre `listId` renverront un code d’erreur 1003 si la liste statique cible contient 10 000 leads ou plus. Consultez le [&#x200B; Guide de migration &#x200B;](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} pour plus d’informations.
