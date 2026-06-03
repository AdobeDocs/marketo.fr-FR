---
description: Migration AWS - Documents Marketo Engage - Documentation du produit
title: Migration d’AWS
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 4a123d365c78c6c03858656c6ef954b55df4338f
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 1%

---

# Migration d’AWS {#aws-migration}

Au cours des prochains mois, tous les abonnements Marketo Engage seront migrés d’un centre de données privé vers le cloud public d’AWS afin d’améliorer la fiabilité, l’évolutivité et la vitesse.

Vous recevrez un e-mail ainsi qu’une notification in-app environ 30 jours avant la migration. Utilisez ce guide pour vous préparer.

## Actions recommandées

Pendant la période de migration, tous les services Marketo Engage ne seront pas disponibles. Nous vous recommandons de prendre les mesures suivantes pour atténuer tout impact sur votre entreprise.

* **Évitez de créer ou de mettre à jour des prospects/personnes** ou d’exécuter des processus qui modifient les enregistrements de personne.

* **Ne déclenchez pas de processus de suivi** car les campagnes planifiées seront suspendues.

* **Désactivez temporairement toutes les intégrations** qui envoient ou reçoivent des données vers ou depuis Marketo Engage.

* **Évitez d’exécuter** d’importer ou d’exporter des données ou toute campagne majeure de génération de leads/personnes.

* **Examinez et mettez à jour les places sur la liste autorisée IP** pour la connexion, l’accès aux API, l’envoi d’e-mails, le tracking web et les intégrations.

* **Ajoutez les adresses IP suivantes** et conservez vos adresses IP actuelles en l’état :

   * 54.160.246.246
   * 54.237.141.197
   * 52.20.211.99

## Impacts attendus sur le service

Les impacts ci-dessous ne nécessitent aucune action de votre part.

* **Les intégrations CRM et les services LaunchPoint** seront désactivés, mais devraient reprendre automatiquement par la suite.
* **Les pages de destination, les formulaires et la collecte de données** ne seront pas disponibles et un message de maintenance s’affichera à la place.

## Planning {#schedule}

De nouvelles dates et informations sur les datacenters/pods sont régulièrement ajoutées. N’oubliez pas de revenir ici pour plus de détails.

Avant de consulter le tableau ci-dessous, [découvrez comment identifier](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) le centre de données et le pod/serveur dans lesquels se trouve votre abonnement.

<table>
 <tbody>
  <tr>
   <th style="width:50%">Date</th>
   <th style="width:20%">Pod</th>
   <th style="width:30%">Heure</th>
  </tr>
  <tr>
   <td>19 Juin 2026</td>
   <td>AB46</td>
   <td>17 h (heure du Pacifique)</td>
  </tr>
  <tr>
   <td>8 juillet 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17 h (heure du Pacifique)<br>
   18 h (heure du Pacifique)</td>
  </tr>
  <tr>
   <td>9 juillet 2026</td>
   <td>AB70<br>
   AB43</td>
   <td>17 h (heure du Pacifique)<br>
   18 h (heure du Pacifique)</td>
  </tr>
  </body>
  </table>

## Mises à jour et assistance

Pour connaître les dernières mises à jour, mettez un signet sur cette page. Pour toute question, contactez l’assistance Adobe via le portail d’assistance d’Admin Console ou [Experience League](https://experienceleague.adobe.com/en/support).
