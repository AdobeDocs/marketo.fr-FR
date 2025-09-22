---
description: Notes De Mise À Jour - Mars 2025 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Mars 2025
feature: Release Information
exl-id: a0e45d8e-6b74-4ab0-a1ba-4dae3754bc8f
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 39%

---

# Notes de mise à jour : mars 2025 {#release-notes-mar-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version de mars 2025. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 28 mars 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr>
   <td><strong>Designer d’e-mail disponible dans tous les programmes</strong> : les nouveaux e-mails de Designer d’e-mail sont désormais accessibles dans les programmes d’engagement, par défaut et d’événement (à la seule exception des programmes de webinaire interactif). Auparavant, ils n’étaient disponibles que dans les programmes de messagerie.</td>
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Fonctionnalités de GenAI dans les webinaires interactifs</strong> : vous pouvez désormais générer des chapitres ainsi qu’un résumé pour les webinaires à la demande. Modifiez et exportez un fichier HTML de vos données.</td>
   <td>Expédié</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai">Fonctionnalités de GenAI</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Mes jetons globaux et Workspace</strong> : configurez mes jetons à la fois au niveau de l’espace de travail et au niveau global pour permettre une productivité et un contrôle améliorés de la marque et des dérivés marketing sur les espaces de travail Marketo Engage et même les instances entières.</td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md#create-a-my-token">Créer un jeton Mon global</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Fonctionnalités sociales obsolètes** : le mercredi 31 juillet 2024, Marketo Engage a commencé à abandonner les fonctionnalités sociales suivantes du produit :

   * Sondages
   * Bouton social
   * Offre de parrainage
   * Partage de vidéos
   * Loteries

À ce jour, les utilisateurs n’ont pas pu créer, cloner ni incorporer ces fonctionnalités de réseaux sociaux dans Marketo Engage. Les actifs sociaux existants continuent de fonctionner jusqu’au 31 janvier 2025. Le 1er février 2025, les actifs sociaux ont cessé de fonctionner. Toutes les fonctionnalités de réseaux sociaux intégrées aux pages de destination doivent être supprimées. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Obsolescence du paramètre « access_token » de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours de suppression et ne sera plus disponible après le 31 octobre 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API SOAP Marketo prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Nouvelle fonctionnalité Analytics - Beta publique** : [Analytique BI avancée](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anciennement connue sous le nom de Revenue Explorer et de Advanced Report Builder) commence à être déployée pour tous les utilisateurs actuels de Revenue Cycle Explorer à la mi-avril. Ce nouvel outil offre une interface flexible de création de rapports et de visualisation sur les données Marketo Engage, fournissant des détails granulaires sur la progression, les performances, etc. Il offre une interactivité et une visualisation plus riches, des performances plus rapides et une expérience utilisateur plus fluide et intuitive.

Pour accéder à cette fonctionnalité, vous devez avoir acheté le module complémentaire BI Analytics avancé. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
