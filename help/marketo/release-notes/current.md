---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 6da797bc91de018e789f1e5980523a02e38eba30
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 5%

---

# Notes De Mise À Jour : Mai 2025 {#release-notes-may-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 25 mai. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [sont disponibles ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **23 mai 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication peuvent faire l’objet de modifications. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto"> 
 <tbody>
 <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr> 
   <td><strong>Personalization de contenu d’e-mail</strong> : Marketo Engage suit désormais la même syntaxe de casse mixte que les autres jetons d’application AEP, ce qui permet de fournir une expérience cohérente entre les produits Adobe DX. Tous les jetons standard, ainsi que les jetons spécifiques à Marketo Engage tels que Membre, Programme et Mes jetons, sont disponibles dans la nouvelle Designer d’e-mail.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/personalization-tokens.md">Jetons Personalization</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Contrôle d’accès en fonction du rôle pour Email Designer Assets</strong> : une nouvelle amélioration du système de contrôle d’accès en fonction du rôle (RBAC) offre des autorisations plus granulaires et une meilleure gestion des utilisateurs pour les ressources optimisées par le nouveau Designer d’e-mail.</td> 
   <td>Expédié</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">Autorisations granulaires pour New Email Designer (article de blog)</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Clonage des e-mails créés dans le Designer d’e-mail</strong> : vous pouvez désormais cloner un e-mail existant créé à l’aide du nouveau Designer d’e-mail.</td> 
   <td>Expédié</td>
   <td>S.O.</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Intégration de GenStudio dans Email Designer </strong> : intégrez GenStudio pour le marketing de performance à partir des e-mails afin d’améliorer l’efficacité du marketing et de maintenir la cohérence de la marque.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Jetons de déclenchement pour n’importe quel attribut</strong> : liste développée de jetons de déclenchement à prendre en charge pour l’utilisation de données provenant de n’importe quel attribut d’activité dans les champs de campagne intelligente.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour de l’intégration de la conversion hors ligne Facebook** : le 29 mai 2025, l’intégration [Facebook Offline Conversion](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"} pour Marketo Engage sera migrée vers la nouvelle API Meta [Conversions](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"}, en raison de l’obsolescence de l’API [Offline Conversions](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} par Meta, conformément au contrôle de version de l’API Graph. Pour plus d’informations, consultez le guide de Meta relatif à l’[envoi d’événements hors ligne via l’API de conversion](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI pour hors ligne).

* **Nouvelle fonctionnalité Analytics - Beta publique** : [Analytique BI avancée](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anciennement connue sous le nom de Revenue Explorer et de Advanced Report Builder) a commencé à être déployée auprès de tous les utilisateurs actuels de Revenue Cycle Explorer à la mi-avril. Ce nouvel outil offre une interface flexible de création de rapports et de visualisation sur les données Marketo Engage, fournissant des détails granulaires sur la progression, les performances, etc. Il offre une interactivité et une visualisation plus riches, des performances plus rapides et une expérience utilisateur plus fluide et intuitive.

Pour accéder à cette fonctionnalité, vous devez avoir acheté le module complémentaire BI Analytics avancé. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 31 octobre 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête « Authorization », [comme décrit ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
