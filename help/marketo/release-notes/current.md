---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: bf6525359d8bc206ed01220823b6c1de5734df55
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 6%

---

# Notes De Mise À Jour : Janvier 2025 {#release-notes-jan-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 25 janvier. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour dédiées au Adobe Dynamic Chat [sont disponibles ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, veuillez contacter votre représentant de Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **17 janvier 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication peuvent faire l’objet de modifications. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr> 
   <td><strong>Nouveau Designer d’e-mail</strong> : créez des e-mails modernes et efficaces à l’aide du nouveau Designer d’e-mail natif dans Marketo Engage. Accédez à l’un des modèles d’e-mail prêts à l’emploi préconçus ou créez facilement le vôtre. Utilisez du contenu dynamique et accédez aux images à partir des services cloud Adobe Experience Manager.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Annuler l’inscription des personnes inscrites à un événement dans les webinaires interactifs</strong> : désormais, si vous ne souhaitez pas qu’une personne inscrite à votre webinaire le soit pour une raison quelconque, vous pouvez l’annuler. Le workflow supprime l’inscrit du programme d’événement Marketo ainsi que d’Adobe Connect.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Désactiver les campagnes sur l’archive </strong> : désactivez les campagnes de déclenchement actives et annulez toutes les exécutions par lots planifiées des campagnes dans un dossier lorsqu’il est archivé. Dans la mesure où une vérification des autorisations supplémentaires est effectuée pour les dossiers d’archivage contenant des campagnes actives (Activer la campagne de déclenchement et Planifier la campagne par lots), cette fonctionnalité est désactivée par défaut avec cette version et peut être activée en accédant à <b>Admin</b> &gt; <b>Coffre au trésor</b> dans votre abonnement de Marketo Engage.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour de l’API Get Program Members** : nous avons amélioré l’API [ Get Program Members](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} pour permettre de récupérer l’identifiant des membres du programme. Pour ce faire, ajoutez l’ID à la liste des champs spécifiés dans le paramètre fields de la requête API.

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 30 juin 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête « Authorization », [comme décrit ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API SOAP de Marketo prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
