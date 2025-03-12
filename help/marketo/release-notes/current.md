---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 7a583a482af64290d08644945e569612f4be8ab9
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 9%

---

# Notes De Mise À Jour : Mars 2025 {#release-notes-mar-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version de mars 2025. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [sont disponibles ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **28 mars 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication peuvent faire l’objet de modifications. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr> 
   <td><strong>Designer d’e-mail disponible dans tous les programmes</strong> : les nouveaux e-mails de Designer d’e-mail sont désormais accessibles dans les programmes d’engagement, par défaut et d’événement (à la seule exception des programmes de webinaire interactif). Auparavant, ils n’étaient disponibles que dans les programmes de messagerie.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Fonctionnalités de GenAI dans les webinaires interactifs</strong> : vous pouvez désormais générer des chapitres ainsi qu’un résumé pour les webinaires à la demande. Modifiez et exportez un fichier HTML de vos données.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Mes jetons globaux et Workspace</strong> : configurez mes jetons à la fois au niveau de l’espace de travail et au niveau global pour permettre une productivité et un contrôle améliorés de la marque et des dérivés marketing sur les espaces de travail Marketo Engage et même les instances entières.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Jetons pour n’importe quel attribut de déclencheur</strong> : développe la liste des jetons de déclencheur disponibles uniquement à partir de la liste de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments" target="_blank">ce document</a> pour prendre en charge l’utilisation de données provenant de n’importe quel attribut d’activité de déclenchement dans les champs de flux de campagne. Imprimer les données d’un attribut d’activité dans un moment intéressant ou définir le dernier ID de transaction d’un prospect à partir d’une activité personnalisée dans un champ de prospect.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Fonctionnalités sociales obsolètes** : le mercredi 31 juillet 2024, Marketo Engage a commencé à abandonner les fonctionnalités sociales suivantes du produit :

   * Sondages
   * Réseaux sociaux
   * Offre de parrainage
   * Partage de vidéos
   * Loteries

À ce jour, les utilisateurs n’ont pas pu créer, cloner ni incorporer ces fonctionnalités de réseaux sociaux dans Marketo Engage. Les actifs sociaux existants continuent de fonctionner jusqu’au 31 janvier 2025. Le 1er février 2025, les actifs sociaux ont cessé de fonctionner. Toutes les fonctionnalités de réseaux sociaux intégrées aux pages de destination doivent être supprimées. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 30 juin 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête « Authorization », [comme décrit ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

