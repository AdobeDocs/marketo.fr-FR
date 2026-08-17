---
description: Migration AWS - Documents Marketo Engage - Documentation du produit
title: Migration d’AWS
feature: Getting Started
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: d5768261c9bb659ef96b73c46a9e078f953d8ed6
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 4%

---

# Migration d’AWS {#aws-migration}

Au cours des prochains mois, tous les abonnements Marketo Engage seront migrés d’un centre de données privé vers le cloud public d’AWS afin d’améliorer la fiabilité, l’évolutivité et la vitesse.

Vous recevrez un e-mail ainsi qu’une notification in-app environ 30 jours avant la migration. Utilisez ce guide pour vous préparer.

## Actions recommandées {#actions}

Pendant la période de migration, tous les services Marketo Engage ne seront pas disponibles. Nous vous recommandons de prendre les mesures suivantes pour atténuer tout impact sur votre entreprise.

* **Évitez de créer ou de mettre à jour des prospects/personnes** ou d’exécuter des processus qui modifient les enregistrements de personne.

* **Ne déclenchez pas de processus de suivi** car les campagnes planifiées seront suspendues.

* **Désactivez temporairement toutes les intégrations** qui envoient ou reçoivent des données vers ou depuis Marketo Engage.

* **Évitez d’exécuter** d’importer ou d’exporter des données ou toute campagne majeure de génération de leads/personnes.

* **Examinez et mettez à jour les places sur la liste autorisée IP** pour la connexion, l’accès aux API, l’envoi d’e-mails, le tracking web et les intégrations.

* **Ajoutez de nouvelles adresses IP** et conservez vos adresses IP actuelles en l’état. Voir les adresses IP à ajouter via le [tableau ci-dessous](#ip-addresses).

## Impacts attendus sur le service {#impacts}

Les impacts ci-dessous ne nécessitent aucune action de votre part.

* **Les intégrations CRM et les services LaunchPoint** seront désactivés, mais devraient reprendre automatiquement par la suite.
* **Les pages de destination, les formulaires et la collecte de données** ne seront pas disponibles et un message de maintenance s’affichera à la place.

>[!NOTE]
>
>Si vous utilisez [formulaires externes](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} et souhaitez éviter de perdre les données d’envoi de formulaire collectées alors que Marketo Engage n’est pas disponible pendant votre période de migration, contactez [l’assistance Adobe](https://experienceleague.adobe.com/en/support){target="_blank"} **au moins deux jours ouvrables** à l’avance et fournissez l’ID de formulaire et l’ID de Munchkin de votre abonnement.

## Identifier votre datacenter/pod {#identify}

Avant de passer en revue les tableaux ci-dessous, [découvrez comment identifier](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) le centre de données et le pod/serveur dans lesquels se trouve votre abonnement.

## Planning {#schedule}

De nouvelles dates et informations sur le datacenter/pod sont régulièrement ajoutées ou modifiées. Surveillez donc ce planning pour les mises à jour.

+++Planning de juillet
<table>
 <tbody>
  <tr>
   <th style="width:25%">Date</th>
   <th style="width:25%">Centre de données/pod</th>
   <th style="width:25%">Heure</th>
   <th style="width:25%">Statut</th>
  </tr>
  <tr>
   <td>8 juillet 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17 h (HAP)<br>
   18 h (HAP)</td>
   <td>Terminé<br>
   Terminé</td>
  </tr>
  <tr>
   <td>9 juillet 2026</td>
   <td>AB70</td>
   <td>17 h (HAP)</td>
   <td>Terminé</td>
  </tr>
  <tr>
   <td>11 juillet 2026</td>
   <td>AB46</td>
   <td>10 h (heure du Pacifique)</td>
   <td>Terminé</td>
  </tr>
  <tr>
   <td>13 Juillet 2026</td>
   <td>NLD101</td>
   <td>10 h (heure du Pacifique)</td>
   <td>Terminé</td>
  </tr>
  <tr>
   <td>15 juillet 2026</td>
   <td>NLD102<br>
   NLD104</td>
   <td>10 h (heure du Pacifique)<br>
   11 h (heure du Pacifique)</td>
   <td>Terminé<br>
   Terminé</td>
  </tr>
  <tr>
   <td>17 juillet 2026</td>
   <td>NLD103<br>
   NLD105</td>
   <td>10 h (heure du Pacifique)<br>
   11 h (heure du Pacifique)</td>
   <td>Terminé<br>
   Terminé</td>
  </tr>
  <tr>
   <td>21 juillet 2026</td>
   <td>AB54</td>
   <td>17 h (HAP)</td>
   <td>Terminé</td>
  </tr>
  <tr>
   <td>23 juillet 2026</td>
   <td>AB48</td>
   <td>17 h (HAP)</td>
   <td>Terminé</td>
  </tr>
  <tr>
   <td>31 juillet 2026</td>
   <td>AB43</td>
   <td>15 h (HAP)</td>
   <td>Terminé</td>
  </tr>
  </body>
</table>

+++

<table>
 <tbody>
  <tr>
   <th style="width:25%">Date</th>
   <th style="width:25%">Centre de données/pod</th>
   <th style="width:25%">Heure</th>
   <th style="width:25%">Statut</th>
  </tr>
  <tr>
   <td>12 Août 2026</td>
   <td>AB61<br>
   AB17</td>
   <td>15 h (HAP)<br>
   16 h (HAP)</td>
   <td>Terminé<br>
   Terminé</td>
  </tr>
  <tr>
  <td>13 Août 2026</td>
   <td>AB68</td>
   <td>16 h (HAP)</td>
   <td>Terminé</td>
  </tr>
  <tr>
  <td>18 Août 2026</td>
   <td><i>AB39</i></td>
   <td><i>17 h (HAP)</i></td>
   <td><i>Reporté (date à déterminer)</i></td>
  </tr>
  <tr>
   <td>20 Août 2026</td>
   <td>AB42<br>
   AB44</td>
   <td>17 h (HAP)<br>
   18 h (HAP)</td>
   <td>Prévu<br>
   Selon le calendrier</td>
  </tr>
  <tr>
   <td>26 Août 2026</td>
   <td>AB40<br>
   AB50</td>
   <td>17 h (HAP)<br>
   18 h (HAP)</td>
   <td>Prévu<br>
   Selon le calendrier</td>
  </tr>
  <tr>
   <td>28 Août 2026</td>
   <td>AB53<br>
   AB56</td>
   <td>15 h (HAP)<br>
   16 h (HAP)</td>
   <td>Prévu<br>
   Selon le calendrier</td>
  </tr>
  <tr>
   <td>8 septembre 2026</td>
   <td>AB01<br>
   AB02</td>
   <td>17 h (HAP)<br>
   18 h (HAP)</td>
   <td>Prévu<br>
   Selon le calendrier</td>
  </tr>
  <tr>
   <td>10 septembre 2026</td>
   <td>AB03<br>
   <i>AB04</i></td>
   <td>17 h (HAP)<br>
   18 <i> PDT</i></td>
   <td>Prévu<br>
   <i>Reporté (date à déterminer)</i></td>
  </tr>
  <tr>
   <td>15 septembre 2026</td>
   <td>AB05<br>
   AB06</td>
   <td>17 h (HAP)<br>
   18 h (HAP)</td>
   <td>Prévu<br>
   Selon le calendrier</td>
  </tr>
  <tr>
   <td>17 septembre 2026</td>
   <td>AB07<br>
   AB08</td>
   <td>17 h (HAP)<br>
   18 h (HAP)</td>
   <td>Prévu<br>
   Selon le calendrier</td>
  </tr>
  </body>
</table>

## Adresses IP à ajouter {#ip-addresses}

En fonction de votre centre de données, collaborez avec votre service informatique pour ajouter les adresses IP respectives.

<table>
<tbody>
<tr>
  <th style="width:25%">Centre de données</th>
  <th style="width:75%">Adresses IP</th>
</tr>
<tr>
  <td>AB</td>
  <td>54.160.246.246<br>
  54.237.141.197<br>
  52.20.211.99</td>
</tr>
<tr>
  <td>NLD</td>
  <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
</tr>
</body>
</table>

## Mises à jour et assistance {#support}

Pour connaître les dernières mises à jour, mettez un signet sur cette page. Pour toute question, contactez l’assistance Adobe via le portail d’assistance d’Admin Console ou [Experience League](https://experienceleague.adobe.com/en/support){target="_blank"}.

## Questions fréquentes {#faq}

**Où les données sont-elles stockées ?**
Toutes les données utilisateur de Marketo sont stockées sur Amazon Web Services (AWS). Marketo a migré son infrastructure depuis ses datacenters physiques vers la plateforme cloud de niveau entreprise d’AWS.

**Où précisément les données personnelles sont-elles stockées ?**
Les données personnelles sont stockées dans Amazon Aurora, le service de base de données relationnelle entièrement géré d&#39;AWS. Aurora reproduit les données de six façons sur trois zones de disponibilité distinctes dans la région AWS afin de protéger les données personnelles contre les défaillances matérielles, la dégradation du stockage et les événements d&#39;infrastructure localisés.

**À qui appartient l’environnement de stockage ?**
L’infrastructure de stockage est détenue et exploitée par Amazon Web Services (AWS). Adobe (Marketo) fonctionne comme un client d’AWS selon un modèle de responsabilité partagée : AWS est responsable de la sécurité et de la disponibilité de l’infrastructure sous-jacente, tandis qu’Adobe est responsable de la sécurité des données et des applications qu’il contient.

**Quels sont les détails complets sur la production, les emplacements de sauvegarde/reprise après sinistre et la technologie de stockage ?**
Marketo utilise Amazon Aurora, un moteur de base de données relationnelle natif dans le cloud entièrement géré par AWS, comme principale technologie de base de données. Aurora découple le calcul et le stockage, répliquant automatiquement les données de six façons sur trois zones de disponibilité dans la région de production et exigeant un quorum de quatre copies pour confirmer toute opération d&#39;écriture.

Aurora effectue également des sauvegardes automatiques continues vers Amazon S3 en temps réel, permettant la récupération instantanée (PITR) à n’importe quelle seconde dans la fenêtre de conservation configurée.

Actuellement, le déploiement de Marketo Aurora fonctionne dans une seule région AWS, sans réplication inter-régions. Les données de production restent au sein de l&#39;infrastructure régionale désignée, et la reprise après sinistre est assurée par la redondance du stockage multi-AZ d&#39;Aurora et des sauvegardes continues plutôt que par le basculement géographique vers une région secondaire. Cela peut être évalué plus en détail à mesure que l’infrastructure AWS de Marketo se développe.
