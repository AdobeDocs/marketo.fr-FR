---
description: Mesures de journal de synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Mesures de journal de synchronisation Salesforce
feature: Reporting
source-git-commit: cfd7e3f70246a0a36793f747f0f2f40bcb9619c5
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Mesures de journal de synchronisation Salesforce  {#salesforce-sync-backlog-metrics}

Le journal de synchronisation est le nom utilisé pour les enregistrements en attente de synchronisation. Il tient compte des enregistrements en attente de synchronisation de Salesforce vers Marketo Engage, et vice versa. S’assurer que le retard reste sous contrôle entraînera des synchronisations régulières et temporelles. Le journal des logs couvre les nombres en attente de mises à jour de publication de synchronisation de part et d’autre, et non ceux qui sont effectués par les étapes de flux de synchronisation, telles que les étapes de flux Piste de synchronisation vers SFDC .

## Accès {#how-to-access}

1. En Marketo Engage, accédez à la zone **Admin**.

   ![](assets/salesforce-sync-backlog-metrics-1.png)

1. Sélectionnez **Salesforce**.

   ![](assets/salesforce-sync-backlog-metrics-2.png)

## Tendance du journal de synchronisation {#sync-backlog-trend}

La tendance des retards reflète les changements dans les retards enregistrés au cours des 5 derniers jours. Le journal des logs s’affiche dans un intervalle de 4 heures réparti sur 5 jours. Par conséquent, le graphique affichera 6 intervalles par jour et 5 jours, ce qui équivaut à 30 intervalles.

Le journal est observé à un intervalle de temps de 4 heures spécifique sur l’axe X. Cette valeur est destinée à tous les objets synchronisés. Il s’agit du total du journal dans Salesforce et Marketo Engage en attente de synchronisation.

![](assets/salesforce-sync-backlog-metrics-3.png)

## Débit de synchronisation et journal des transactions {#sync-throughput-and-backlog}

Les statistiques reflètent l’état du débit et du journal des travaux pour chaque type d’objet sous synchronisation pendant les dernières 24 heures. Les types d’objet incluent tous les objets sous-synchronisés, notamment : Lead, Contact, Account, Opportunity, Campaign, User et Custom Objects. Les statistiques de débit sont automatiquement actualisées toutes les 15 minutes, mais vous pouvez les actualiser manuellement à l’aide de l’icône d’actualisation. Le journal des logs est récupéré toutes les heures.

>[!NOTE]
>
>Les statistiques sont mises à jour sur une base variable et non par jour calendaire.

![](assets/salesforce-sync-backlog-metrics-4.png)

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

**Champs visibles à l’utilisateur de synchronisation** : assurez-vous que les champs visibles à synchroniser sont uniquement ceux qui doivent être synchronisés et qui ont une valeur pour les efforts de marketing. Toute mise à jour d’un enregistrement dans Salesforce qui met à jour l’horodatage de la dernière modification met en file d’attente un enregistrement dans le journal de synchronisation, et la synchronisation des champs inutiles peut ralentir les champs plus importants en cours de synchronisation. Si les champs superflus sont masqués à l’utilisateur de synchronisation, les mises à jour de ces champs entraînent un saut beaucoup plus rapide qu’une mise à jour. Contactez votre administrateur Salesforce pour passer en revue les bonnes pratiques [ici](https://nation.marketo.com/t5/marketo-whisperer-blogs/best-practices-for-determining-which-fields-to-sync-with-marketo/ba-p/247449){target="_blank"} et mettre à jour les champs visibles par l’utilisateur de synchronisation Marketo.

**Masquer ou filtrer les enregistrements inutiles** : si un enregistrement n’est pas commercialisable, il se peut qu’il gaspille des ressources de synchronisation. Si l’utilisateur de synchronisation ne peut pas le voir, il ne gaspillera pas de ressources en essayant de le synchroniser. [ La prise en charge des Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"} peut vous aider à configurer un filtre de synchronisation afin d’empêcher les enregistrements de se synchroniser en fonction de critères supplémentaires. Vous trouverez plus d’informations sur la configuration d’un filtre de synchronisation personnalisé [ ici](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}. Il est vivement recommandé d’utiliser les champs d’index dans Salesforce (contactez Salesforce pour plus d’informations).

**Planifiez les mises à jour en masse pendant les heures non critiques** : vérifiez vos modèles de synchronisation des données pour identifier les périodes non critiques. Vérifiez si des mises à jour en masse peuvent être planifiées au cours de ces périodes non critiques si possible.

**Champs fréquemment mis à jour** : certains champs sont sujets à de fréquentes mises à jour. Par exemple, les champs de devise qui font l’objet de modifications de devise. Vérifiez si ces champs doivent être synchronisés ou s’ils doivent être conçus différemment. Si d’autres champs sont fréquemment mis à jour et ne sont pas nécessaires, masquez-les à l’utilisateur de synchronisation. Veillez à discuter avec vos intégrations d’administration SFDC qui peuvent mettre à jour des champs.

**Objets personnalisés** : consultez régulièrement les [objets personnalisés](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync){target="_blank"} activés pour la synchronisation et la désactivation de ceux qui n’ont plus besoin d’être synchronisés.

**Activités** : [Vérifiez si une synchronisation activée pour les activités](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync){target="_blank"} peut être supprimée de la synchronisation.  Ces activités ne se synchronisent qu’une fois par jour et par piste.

**Réviser les erreurs de synchronisation** : la gestion des exceptions peut ralentir la synchronisation. La révision des notifications utilisateur et la résolution des erreurs peuvent améliorer l’intégrité de la synchronisation.

**Contactez l’assistance** : si vous suivez toutes les bonnes pratiques ci-dessus et que vous rencontrez toujours des retards importants, contactez l’[assistance Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"}.
