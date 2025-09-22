---
description: Mesures de la liste d’attente de synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Mesures de la liste d’attente de synchronisation Salesforce
feature: Reporting
exl-id: 6b58eb50-ff0d-4774-a232-3ae929948e2a
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Mesures de la liste d’attente de synchronisation Salesforce  {#salesforce-sync-backlog-metrics}

La liste d’attente de synchronisation est le nom utilisé pour les enregistrements en attente de synchronisation. Il prend en compte les enregistrements en attente de synchronisation de Salesforce vers Marketo Engage, et vice versa. Veiller à ce que la liste d’attente reste contrôlée permettra des synchronisations fluides et temporelles. La liste d’attente couvre les nombres de mises à jour de post-synchronisation en attente d’un côté ou de l’autre, et non ceux entrepris par des étapes de flux de synchronisation telles que les étapes de flux Synchroniser le lead avec SFDC .

## Accès {#how-to-access}

1. Dans Marketo Engage, accédez à la zone **Admin**.

   ![](assets/salesforce-sync-backlog-metrics-1.png)

1. Sélectionnez **Salesforce**.

   ![](assets/salesforce-sync-backlog-metrics-2.png)

## Tendance de la liste d&#39;attente de synchronisation {#sync-backlog-trend}

La tendance de la liste d’attente reflète les modifications de la liste d’attente enregistrée au cours des 5 derniers jours. La liste d’attente s’affiche par intervalles de 4 heures répartis sur 5 jours. Par conséquent, le graphique affichera 6 intervalles par jour fois 5 jours, ce qui équivaut à 30 intervalles.

La liste d’attente est observée à un intervalle de temps particulier de 4 heures sur l’axe des abscisses. Cette valeur concerne tous les objets synchronisés. Il s’agit du total de la liste d’attente dans Salesforce et Marketo Engage en attente de synchronisation.

![](assets/salesforce-sync-backlog-metrics-3.png)

## Débit de synchronisation et liste d’attente {#sync-throughput-and-backlog}

Les statistiques reflètent le débit et le statut de la liste d’attente pour chaque type d’objet synchronisé au cours des dernières 24 heures. Les types d’objets incluent tous les objets synchronisés, notamment : lead, contact, compte, opportunité, campagne, utilisateur et objets personnalisés. Les statistiques de débit sont actualisées automatiquement toutes les 15 minutes, mais vous pouvez les actualiser manuellement à l’aide de l’icône d’actualisation. La liste d’attente est récupérée toutes les heures.

>[!NOTE]
>
>Les statistiques sont mises à jour de manière progressive, et non par jour calendaire.

![](assets/salesforce-sync-backlog-metrics-4.png)

<table><thead>
  <tr>
    <th>Champ</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Nbre max. d'enregistrements synchronisés/h</td>
    <td>Le nombre maximal d’enregistrements synchronisés par heure (débit maximal) observé au cours des dernières 24 heures pour le type d’objet. La période de 24 heures suit le temps, et non le jour du calendrier.</td>
  </tr>
  <tr>
    <td>Nb min d'enregistrements synchronisés/h</td>
    <td>Le nombre minimum d’enregistrements synchronisés par heure (débit minimum) observé au cours des dernières 24 heures pour le type d’objet. La période de 24 heures suit le temps, et non le jour du calendrier.</td>
  </tr>
  <tr>
    <td>Nombre moyen d'enregistrements synchronisés par heure</td>
    <td>Le nombre moyen d’enregistrements synchronisés par heure (débit minimal) observé au cours des dernières 24 heures pour le type d’objet. La période de 24 heures suit le temps, et non le jour du calendrier. Il s’agit du nombre total d’enregistrements synchronisés au cours des dernières 24 heures.</td>
  </tr>
  <tr>
    <td>Liste d'attente de synchronisation</td>
    <td>La liste d'attente des enregistrements en attente de synchronisation pour le type d'objet. Il s’agit du total de la liste d’attente de synchronisation dans les deux directions (de Salesforce vers Marketo Engage, et vice versa). La liste d’attente de Salesforce est obtenue à l’aide d’un appel API à Salesforce et la liste d’attente de Marketo Engage est calculée à l’aide des statistiques obtenues à partir du journal des données de modification. Il est calculé toutes les heures. Les deux champs suivants de ce tableau indiquent respectivement la date du dernier calcul de la liste d’attente et le prochain planning de calcul.</td>
  </tr>
  <tr>
    <td>Retard estimé (temps)</td>
    <td>Estimation du temps nécessaire pour synchroniser la liste d’attente par type d’objet. Calculé comme suit : « Nombre moyen d’enregistrements synchronisés par heure ».</td>
  </tr>
  <tr>
    <td>Dernière récupération de la liste d’attente</td>
    <td>Heure du dernier calcul de la liste d’attente.</td>
  </tr>
  <tr>
    <td>Prochaine récupération de la liste d’attente</td>
    <td>Heure du prochain calcul de la liste d’attente.</td>
  </tr>
  <tr>
    <td>Statut de la liste d’attente</td>
    <td>Indique si la liste d’attente a augmenté au cours des 6 dernières heures. Il est considéré comme « croissant » si l’arriéré actuel est supérieur à l’arriéré enregistré il y a 6 heures. Dans le cas contraire, il s’affiche comme « Normal ». L’objectif est d’indiquer si le débit de synchronisation rattrape la liste d’attente.</td>
  </tr>
</tbody></table>

## Causes des retards de synchronisation {#what-causes-sync-backlogs}

Que la mise à jour soit effectuée du côté Marketo Engage ou du côté CRM, elle déclenchera la resynchronisation de l’enregistrement pour mettre à jour les informations de l’autre côté via le cycle de synchronisation Marketo Engage vers CRM standard. Chaque fois qu’une mise à jour est apportée à un enregistrement sur Salesforce, elle génère un horodatage de modification du système, appelé « SysModStamp ». Cette opération met en file d’attente une modification à synchroniser.

Lorsqu’un grand nombre de mises à jour sont effectuées (par exemple à partir de la modification d’une valeur de champ), de nombreux enregistrements sont modifiés, ce qui entraîne de nouveaux SysModStamps. Un grand nombre de mises à jour d’enregistrements de personnes doit ensuite être resynchronisé entre Marketo Engage et votre CRM, ce qui crée parfois une liste d’attente momentanée.

## Bonnes pratiques de gestion des retards de synchronisation {#best-practices}

**Champs visibles pour l’utilisateur de la synchronisation** : assurez-vous que les champs visibles à synchroniser sont uniquement ceux qui doivent être synchronisés et ont une valeur pour les efforts marketing. Toute mise à jour d’un enregistrement dans Salesforce qui met à jour la date et l’heure de la dernière modification met un enregistrement en file d’attente dans la liste d’attente de synchronisation. De plus, la synchronisation des champs inutiles peut ralentir les champs plus importants sous synchronisation. Si les champs inutiles sont masqués à l’utilisateur de la synchronisation, les mises à jour de ces champs entraîneront une omission beaucoup plus rapide qu’une mise à jour. Contactez votre administrateur Salesforce pour passer en revue les bonnes pratiques [ici](https://nation.marketo.com/t5/marketo-whisperer-blogs/best-practices-for-determining-which-fields-to-sync-with-marketo/ba-p/247449){target="_blank"} et mettre à jour les champs visibles par l’utilisateur de synchronisation Marketo.

**Masquer ou filtrer les enregistrements inutiles** : si un enregistrement n’est pas commercialisable, cela peut entraîner une perte de ressources de synchronisation. Si l’utilisateur ou l’utilisatrice de la synchronisation ne peut pas le voir, il ne gaspillera pas de ressources à essayer de le synchroniser. La prise en charge de [Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"} peut vous aider à configurer un filtre de synchronisation pour empêcher la synchronisation des enregistrements en fonction de critères supplémentaires. Vous trouverez plus d’informations sur la configuration d’un filtre de synchronisation personnalisé [ici](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}. Il est vivement recommandé d’utiliser les champs d’index dans Salesforce (contactez Salesforce pour plus d’informations).

**Planifier des mises à jour en bloc pendant les heures non critiques** : passez en revue vos modèles de synchronisation des données pour identifier les périodes non critiques. Vérifiez si des mises à jour en bloc peuvent être planifiées au cours de ces périodes non critiques, si possible.

**Champs fréquemment mis à jour** : certains champs sont sujets à de fréquentes mises à jour. Par exemple, les champs de devise qui font l’objet de modifications de devise. Vérifiez si ces champs doivent être synchronisés ou s’ils doivent être conçus différemment. Si d’autres champs sont mis à jour fréquemment et ne sont pas nécessaires, masquez-les à l’utilisateur ou à l’utilisatrice de synchronisation. Veillez à discuter avec vos administrateurs SFDC des intégrations susceptibles de mettre à jour les champs.

**Objets personnalisés** : vérifiez régulièrement [objets personnalisés](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync){target="_blank"} activés pour synchroniser et désactiver ceux qui n’ont plus besoin d’être synchronisés.

**Activités** : [vérifiez si la synchronisation activée pour les activités](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync){target="_blank"} peut être supprimée de la synchronisation.  Ces activités ne se synchronisent qu’une seule fois par jour par prospect.

**Vérifier les erreurs de synchronisation** : la gestion des exceptions peut ralentir la synchronisation. La révision des notifications utilisateur et la résolution des erreurs peuvent améliorer l’intégrité de la synchronisation.

**Contactez l’assistance** : si vous suivez toutes les bonnes pratiques ci-dessus et que vous rencontrez toujours des retards importants, contactez l’assistance de [Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"}.
