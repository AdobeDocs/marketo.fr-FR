---
description: Tableau de bord des mesures d’observabilité de la synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Tableau de bord des mesures d’observabilité de la synchronisation Salesforce
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 2457f0f51c6365c29a040e908678e81517327de5
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Mesures de journal de synchronisation Salesforce  {#salesforce-sync-backlog-metrics}

Passez en revue les débits de performances de synchronisation et synchronisez les retards avec ce tableau de bord.

## Débit de synchronisation et journal des transactions {#sync-throughput-and-backlog}

1. Dans Marketo Engage, accédez à la zone Admin .

   CAPTURE D’ÉCRAN

1. Sélectionnez Salesforce.

   CAPTURE D’ÉCRAN

Les statistiques reflètent l’état du débit et du journal des travaux pour chaque type d’objet sous synchronisation pendant les dernières 24 heures. Les types d’objet incluent tous les objets sous-synchronisés, notamment : Lead, Contact, Account, Opportunity, Campaign, User et Custom Objects. Les statistiques de débit sont automatiquement actualisées toutes les 15 minutes, mais vous pouvez les actualiser manuellement à l’aide de l’icône d’actualisation. Le journal des logs est récupéré toutes les heures.

>[!NOTE]
>
>Les statistiques sont mises à jour sur une base variable et non par jour calendaire.

CAPTURE D’ÉCRAN

<table><thead>
  <tr>
    <th>Champ</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Nombre max. d’enregistrements synchronisés / hr</td>
    <td>Nombre maximum d’enregistrements synchronisés par heure (débit maximum) observés au cours des dernières 24 heures pour le type d’objet. La période de 24 heures s’étend avec le temps, et non avec le jour calendaire.</td>
  </tr>
  <tr>
    <td>Enregistrements mineurs synchronisés / hr</td>
    <td>Nombre minimum d’enregistrements synchronisés par heure (débit minimal) observé au cours des dernières 24 heures pour le type d’objet. La période de 24 heures s’étend avec le temps, et non avec le jour calendaire.</td>
  </tr>
  <tr>
    <td>Nombre moyen d’enregistrements synchronisés / heure</td>
    <td>Nombre moyen d’enregistrements synchronisés par heure (débit minimal) observés au cours des dernières 24 heures pour le type d’objet. La période de 24 heures s’étend avec le temps, et non avec le jour calendaire. Il s’agit du nombre total d’enregistrements synchronisés au cours des dernières 24 heures.</td>
  </tr>
  <tr>
    <td>Journal de synchronisation</td>
    <td>Le journal des enregistrements en attente de synchronisation pour le type d’objet. Il s’agit de la somme totale des retards de synchronisation dans les deux directions (de Salesforce à Marketo Engage, et vice versa). Le journal de Salesforce est obtenu à l’aide d’un appel API à Salesforce et le journal de Marketo Engage est calculé à l’aide des statistiques obtenues à partir du journal de données des modifications. Ceci est calculé toutes les heures. Les deux champs suivants de ce tableau indiquent la date du dernier calcul du retard et le prochain planning de calcul, respectivement.</td>
  </tr>
  <tr>
    <td>Arborescence estimée (temps)</td>
    <td>Estimation du temps nécessaire à la synchronisation du journal des travaux par type d’objet. Calculé en tant qu’enregistrements de journal de synchronisation/moyenne synchronisés par heure.</td>
  </tr>
  <tr>
    <td>Dernière récupération du journal</td>
    <td>Heure du dernier calcul du journal des travaux en souffrance.</td>
  </tr>
  <tr>
    <td>Récupération suivante du backlog</td>
    <td>Heure du prochain calcul du journal des travaux en souffrance.</td>
  </tr>
  <tr>
    <td>État du journal</td>
    <td>Cela indique si le retard a augmenté au cours des 6 dernières heures. On parle alors de "croissance" si le retard actuel est supérieur au retard enregistré il y a 6 heures. Dans le cas contraire, il s’affiche sous la forme "Normal". Cela a pour but d’indiquer si le débit de synchronisation rattrape le retard.</td>
  </tr>
</tbody></table>

## Tendance du journal {#backlog-trend}

La tendance des retards reflète les changements dans les retards enregistrés au cours des 5 derniers jours. Le journal des logs s’affiche dans un intervalle de 4 heures réparti sur 5 jours. Par conséquent, le graphique affichera 6 intervalles par jour et 5 jours, ce qui équivaut à 30 intervalles.

Le journal est observé à un intervalle de temps de 4 heures spécifique sur l’axe X. Cette valeur est destinée à tous les objets synchronisés. Il s’agit du total du journal dans Salesforce et Marketo Engage en attente de synchronisation.

CAPTURE D’ÉCRAN
