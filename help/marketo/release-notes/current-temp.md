---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
hide: true
hidefromtoc: true
feature: Release Information
source-git-commit: 7ec3687c0c16738805394377b2080295c2f18032
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 4%

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
   <td><strong>Jetons de déclenchement pour n’importe quel attribut</strong> : liste développée de jetons de déclenchement à prendre en charge pour l’utilisation de données provenant de n’importe quel attribut d’activité dans les champs de campagne intelligente.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Nouvelle fonctionnalité Analytics - Beta publique** : [Analytique BI avancée](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anciennement connue sous le nom de Revenue Explorer et de Advanced Report Builder) a commencé à être déployée auprès de tous les utilisateurs actuels de Revenue Cycle Explorer à la mi-avril. Ce nouvel outil offre une interface flexible de création de rapports et de visualisation sur les données Marketo Engage, fournissant des détails granulaires sur la progression, les performances, etc. Il offre une interactivité et une visualisation plus riches, des performances plus rapides et une expérience utilisateur plus fluide et intuitive.

Pour accéder à cette fonctionnalité, vous devez avoir acheté le module complémentaire BI Analytics avancé. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 30 juin 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête « Authorization », [comme décrit ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
