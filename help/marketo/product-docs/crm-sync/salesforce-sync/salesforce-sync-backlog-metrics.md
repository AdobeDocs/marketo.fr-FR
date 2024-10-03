---
description: Mesures de journal de synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Mesures de journal de synchronisation Salesforce
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 1cc876285f8d7ac7a21a763dd65da34341341a0e
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Mesures de journal de synchronisation Salesforce  {#salesforce-sync-backlog-metrics}

Le journal de synchronisation représente les enregistrements en attente de synchronisation de Salesforce vers Marketo Engage, et vice versa. S’assurer que les retards restent sous contrôle permettra des synchronisations régulières et opportunes.

>[!NOTE]
>
>Le journal des travaux en souffrance couvre les nombres en attente de post-mises à jour de synchronisation de part et d’autre, et non ceux qui sont effectués par des étapes de flux de synchronisation telles que les étapes de flux [Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} ou [Synchroniser la personne avec Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} .

## Accès {#how-to-access}

1. En Marketo Engage, accédez à la zone **Admin**.

   CAPTURE D’ÉCRAN

1. Sélectionnez **Salesforce**.

   CAPTURE D’ÉCRAN

## Tendance du journal de synchronisation {#sync-backlog-trend}

La tendance des retards reflète les changements dans les retards enregistrés au cours des 5 derniers jours. Le journal des logs s’affiche dans un intervalle de 4 heures réparti sur 5 jours. Par conséquent, le graphique affichera 6 intervalles par jour et 5 jours, ce qui équivaut à 30 intervalles.

Le journal est observé à un intervalle de temps de 4 heures spécifique sur l’axe X. Cette valeur est destinée à tous les objets synchronisés. Il s’agit du total du journal dans Salesforce et Marketo Engage en attente de synchronisation.

CAPTURE D’ÉCRAN

## Débit de synchronisation et journal des transactions {#sync-throughput-and-backlog}

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
    <td>Estimation du temps nécessaire à la synchronisation du journal des travaux par type d’objet. Calculé comme suit : "Journal de synchronisation/enregistrements moyens synchronisés par heure".</td>
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

## Causes des retards de synchronisation {#what-causes-sync-backlogs}

Que la mise à jour soit effectuée côté Marketo Engage ou côté CRM, l’enregistrement sera resynchronisé afin de mettre à jour les informations de l’autre côté par le biais du cycle de synchronisation du Marketo Engage ordinaire vers le CRM. Chaque fois qu’une mise à jour est apportée à un enregistrement sur Salesforce, elle génère un horodatage de modification du système, appelé &quot;SysModStamp&quot;. Cette opération place la synchronisation en file d’attente.

Lorsqu’un grand nombre de mises à jour sont effectuées (par exemple à partir d’un changement de valeur de champ), de nombreux enregistrements sont modifiés, provoquant de nouveaux SysModStamps. Un grand nombre de mises à jour des enregistrements de personne doivent ensuite être resynchronisées entre Marketo Engage et votre CRM, ce qui crée parfois un retard momentané.

## Bonnes pratiques pour la gestion des retards de synchronisation {#best-practices}

**Champs sous synchronisation** : assurez-vous que les champs sous-synchronisés ne sont que ceux qui doivent être synchronisés. Les modifications apportées aux champs augmentent le journal de synchronisation et les champs de priorité inférieure peuvent arrêter ou ralentir les champs plus importants sous synchronisation. Pour supprimer les champs synchronisés, contactez le [support Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**Champs sensibles** : certains champs sont sujets à de fréquentes mises à jour (par exemple, les champs de devise sujets à des modifications de devise). Vérifiez si ces champs doivent être synchronisés ou s’ils doivent être conçus différemment.

**Objets personnalisés** : passez régulièrement en revue les objets personnalisés en cours de synchronisation et supprimez ceux qui n’ont plus besoin d’être synchronisés.

**Activités** : vérifiez s’il existe des activités en cours de synchronisation qui peuvent être supprimées de la synchronisation.

**Planifiez les mises à jour en masse pendant les heures non critiques** : vérifiez vos modèles de synchronisation des données pour identifier les périodes non critiques. Vérifiez si des mises à jour en masse peuvent être planifiées pendant ces périodes non critiques.

Si vous suivez toutes les bonnes pratiques ci-dessus et que vous rencontrez toujours des retards importants, contactez le [support Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
