---
description: Notes De Mise À Jour - Octobre 2024 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Octobre 2024
feature: Release Information
exl-id: 2e28ae7f-51de-4510-b3e8-79a989f0daf5
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 21%

---

# Notes de mise à jour : octobre 2024 {#release-notes-oct-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 octobre. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 4 octobre 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr>
   <td><strong>Tokenisation pour les webinaires interactifs</strong> : vous pouvez désormais utiliser des jetons pour promouvoir les webinaires interactifs dans les e-mails et les pages de destination sans avoir à ajouter manuellement les détails du webinaire.</td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/promoting-an-interactive-webinar.md#interactive-webinars-tokens" target="_blank">Promotion d’un webinaire interactif</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Nombre de personnes définies pour affecter la liste dynamique</strong> : déterminez le nombre de personnes affectées lors de la modification des règles de qualification d’une campagne dynamique.</td>
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Bouton Mon compte dans le rail de navigation</strong> : pour les personnes qui ont migré vers le système Adobe Identity Management, un nouveau bouton « Mon compte » dans le rail de navigation de gauche permet de configurer votre fuseau horaire et d’accéder aux détails de l’abonnement.</td>
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Améliorations apportées aux rapports sur les performances des e-mails</strong> : de nombreuses améliorations ont été apportées aux mesures des rapports sur les e-mails et au suivi des activités, offrant ainsi des informations supplémentaires et améliorant la précision.
   <ul>
   <li>Filtrer les personnes supprimées et fusionnées des mesures de performances des e-mails</li>
   <li>Les e-mails sont désormais classés comme <i>abandonnés</i> après avoir attendu trois jours une activité de réponse</li>
   <li>Les ouvertures d’e-mails sont comptabilisées comme des ouvertures uniques séparément pour chaque campagne dynamique</li>
   </td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">Rapport des performances des e-mails</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Mesures de la liste d’attente de synchronisation de Salesforce </strong> : surveillez le débit de synchronisation et les tendances de la liste d’attente afin de planifier et de planifier les mises à jour de CRM pour une expérience de synchronisation optimale.
   </td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Mesures de la liste d’attente de synchronisation Salesforce</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour de l’API d’extraction en bloc** : nous avons corrigé un problème dans l’API d’extraction en bloc impliquant l’option columnHeaderNames , qui vous permet de spécifier des noms d’en-tête de colonne personnalisés dans le fichier exporté. Auparavant, les noms d’en-tête de colonne contenant des caractères non-ASCII pouvaient être corrompus.

* **Obsolescence du paramètre access_token de l’API Rest** : le paramètre de requête « access_token » utilisé pour authentifier les appels API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 31 janvier 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête « Authorization » [comme décrit ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication#using-an-access-token).

* **Obsolescence du code QR** : le 4 octobre 2024, la fonctionnalité de code QR utilisée dans les notifications push et les ressources de messagerie in-app sera abandonnée. Cela inclut l’utilisation de codes QR pour un nouvel appareil de test et la création de nouvelles ressources avec des codes QR. L’obsolescence des fonctionnalités les moins utilisées nous permet de réaffecter leurs ressources à la maintenance globale de Marketo Engage.

* **Modifications Munchkin**

   * **Nouvelle version** : le 17 septembre 2024, [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 commencera à être déployé sur les instances Marketo Engage dont le paramètre « Munchkin Beta » est activé dans **Admin** > **Coffre au trésor**. Son déploiement sur toutes les autres instances est prévu pour le 29 octobre. Cette version met à jour la création du cookie Munchkin. Aucune modification n’a été apportée aux fonctionnalités.

   * **Caractères de l’URL supprimés** : les activités « Page web de visites » et « Lien de clics » créées par Munchkin JS suppriment désormais les caractères de contrôle non codés par une URL de tous les champs d’URL. Cette modification a pour but d’empêcher les erreurs liées à la propagation de ces types de caractères dans des systèmes qui ne les prennent pas en charge et qui n’ont pas une utilisation valide dans Marketo Engage.
