---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 38ec4726dece1695a15104fdb7fa7592b298d4a9
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 7%

---

# Notes De Mise À Jour : Avril 2025 {#release-notes-apr-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version d&#39;avril 2025. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [sont disponibles ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **25 avril 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication peuvent faire l’objet de modifications. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr> 
   <td><strong>Compatibilité des modèles pour Email Designer</strong> : les modèles d'email de l'éditeur d'email classique sont désormais compatibles avec le nouveau <a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">Email Designer</a>.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Secure Socket Layer (SSL) Self Service</strong> : le chiffrement SSL vous permet de rendre les pages de destination d’une instance Marketo Engage sécurisées. Avant d’activer cette fonctionnalité, l’équipe d’assistance d’Adobe devait vous aider. Les utilisateurs de Marketo peuvent désormais l’activer eux-mêmes, ce qui leur permet de gagner un temps précieux.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Nouvelle fonctionnalité Analytics - Beta publique** : [Analytique BI avancée](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anciennement connue sous le nom de Revenue Explorer et de Advanced Report Builder) commence à être déployée pour tous les utilisateurs actuels de Revenue Cycle Explorer à la mi-avril. Ce nouvel outil offre une interface flexible de création de rapports et de visualisation sur les données Marketo Engage, fournissant des détails granulaires sur la progression, les performances, etc. Il offre une interactivité et une visualisation plus riches, des performances plus rapides et une expérience utilisateur plus fluide et intuitive.

Pour accéder à cette fonctionnalité, vous devez avoir acheté le module complémentaire BI Analytics avancé. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 30 juin 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête « Authorization », [comme décrit ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Fonctionnalités sociales obsolètes** : le mercredi 31 juillet 2024, Marketo Engage a commencé à abandonner les fonctionnalités sociales suivantes du produit :

   * Sondages
   * Réseaux sociaux
   * Offre de parrainage
   * Partage de vidéos
   * Loteries

À ce jour, les utilisateurs n’ont pas pu créer, cloner ni incorporer ces fonctionnalités de réseaux sociaux dans Marketo Engage. Les actifs sociaux existants continuent de fonctionner jusqu’au 31 janvier 2025. Le 1er février 2025, les actifs sociaux ont cessé de fonctionner. Toutes les fonctionnalités de réseaux sociaux intégrées aux pages de destination doivent être supprimées. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}
