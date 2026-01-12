---
description: Notes De Mise À Jour - Janvier 2025 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Janvier 2025
feature: Release Information
exl-id: fd816b9c-9e06-4292-87d6-9fa991c4681f
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 35%

---

# Notes de mise à jour : janvier 2025 {#release-notes-jan-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 25 janvier. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 17 janvier 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr>
   <td><strong>Nouveau Designer d’e-mail</strong> : créez des e-mails modernes et efficaces à l’aide du nouveau Designer d’e-mail natif de Marketo Engage. Accédez à l’un des modèles d’e-mail prêts à l’emploi préconçus ou créez facilement le vôtre. Utilisez du contenu dynamique et accédez aux images à partir des services cloud Adobe Experience Manager. Utilisez la fonctionnalité IA générative de l’accélérateur de contenu pour créer des e-mails innovants et performants à grande échelle.
   <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : pour accéder au nouveau concepteur d’e-mail, votre abonnement Marketo Engage doit être migré vers le <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">système Adobe Identity Management (IMS)</a>. Si le vôtre n’a pas encore été envoyé et que vous souhaitez qu’il soit traité rapidement, veuillez contacter l’équipe du compte Adobe (votre gestionnaire de compte) ou l’assistance de <a href="https://nation.marketo.com/t5/support/ct-p/Support">Marketo</a>. Pour accéder à la fonctionnalité IA généralisée de l’accélérateur de contenu, contactez l’équipe du compte Adobe.</td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">Vue d’ensemble du concepteur d’e-mail</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Annuler l’inscription des personnes inscrites à un événement dans les webinaires interactifs</strong> : désormais, si vous ne souhaitez pas qu’une personne inscrite à votre webinaire le soit pour une raison quelconque, vous pouvez l’annuler. Le workflow supprime l’inscrit du programme d’événement Marketo ainsi que d’Adobe Connect.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Désactiver les campagnes sur l’archive </strong> : désactivez les campagnes de déclenchement actives et annulez toutes les exécutions par lots planifiées des campagnes dans un dossier lorsqu’il est archivé. Dans la mesure où une vérification des autorisations supplémentaires est effectuée pour les dossiers d’archivage contenant des campagnes actives (Activer la campagne de déclenchement et Planifier la campagne par lots), cette fonctionnalité est désactivée par défaut avec cette version et peut être activée en accédant à <b>Admin</b> &gt; <b>Coffre au trésor</b> dans votre abonnement Marketo Engage.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
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

À ce jour, les utilisateurs n’ont pas pu créer, cloner ni incorporer ces fonctionnalités de réseaux sociaux dans Marketo Engage. Les actifs sociaux existants continuent de fonctionner jusqu’au 31 janvier 2025. Le 1er février 2025, les actifs sociaux cesseront de fonctionner. Les fonctionnalités sociales intégrées aux pages de destination devront être supprimées. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Mise à jour de l’API Get Program Members** : nous avons amélioré l’API [&#x200B; Get Program Members](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} pour permettre de récupérer l’identifiant des membres du programme. Pour ce faire, ajoutez l’ID à la liste des champs spécifiés dans le paramètre fields de la requête API.

* **Obsolescence du paramètre « access_token » de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours de suppression et ne sera plus disponible après le mercredi 31 mars 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API SOAP Marketo prendra fin le mercredi 31 mars 2026. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
