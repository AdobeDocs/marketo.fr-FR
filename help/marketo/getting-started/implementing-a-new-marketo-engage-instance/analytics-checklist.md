---
description: Configurez la section Analytics pour votre nouvelle instance de Marketo Engage.
title: Bonnes pratiques relatives aux nouvelles instances - Liste de contrôle Analytics
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 7a847ece020ea0c0001241abf8e49b9eadf8edce
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 1%

---

# Bonnes pratiques relatives aux nouvelles instances : liste de contrôle Analytics {#new-instance-best-practices-analytics-checklist}

La section Analytics propose des rapports globaux qui analysent les performances de vos efforts marketing. Découvrez les étapes nécessaires pour les parcourir.

Pensez à [télécharger les listes de contrôle](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) et suivre votre progression.

## Arborescence {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Organisation : dénomination, dossiers et archivage</td>
    <td><li>Utilisez une convention d’affectation des noms de rapport pour différencier les rapports dans l’onglet Rapports globaux .
    <ul><li>Un exemple de bonne pratique de convention d’affectation des noms est [Type de rapport] [Balise globale ou spécifique à une unité d’exploitation] [Description du rapport], par exemple [Performance de messagerie]-[Global]-[Engagement de messagerie de 180 jours].</li></ul><br>
    <li>Identifiez les rapports qui doivent être partagés avec différents groupes d’utilisateurs au sein de votre organisation (par exemple, l’équipe commerciale, la direction marketing) et organisez les rapports par dossier dans le dossier Rapports de groupe d’Analytics pour les rapports globaux.</li> 
    <li>L’archivage doit être limité au dossier Rapports globaux, car il s’agit de rapports toujours actifs.   <ul><li>Limitez l’archivage aux modifications organisationnelles, telles que la réduction ou l’ajout d’unités opérationnelles pertinentes si vous créez des rapports en fonction d’une structure d’unités opérationnelles.</li></ul>
    </td>
  </tr>
  <tr>
    <td>Espaces de travail (le cas échéant)</td>
    <td><li>Répliquez les rapports globaux et la structure de dossiers dans les espaces de travail afin de conserver des rapports cohérents pour vos équipes. Ces rapports se trouveraient dans le dossier Rapports de groupe .</li></td>
  </tr>
  <tr>
    <td>Mes rapports</td>
    <td><li>Identifiez et créez les rapports à utiliser dans la section <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Mes rapports</a> . Utilisez cette section de rapport privé comme environnement de test pour les rapports globaux. Ils ne sont disponibles que pour l’utilisateur qui crée le rapport.</li>
    <li>Utilisez la convention d’affectation des noms de votre entreprise pour identifier le rapport et l’utilisation afin de pouvoir réconcilier les rapports dans Mes rapports avec les rapports dans Rapports de groupe.</li></td>
  </tr>
  <tr>
    <td>Rapports de groupe</td>
    <td><li>Les rapports de groupe sont les rapports globaux de votre organisation et doivent générer des rapports sur l’activité globale de votre organisation.</li>
    <li>Envisagez de créer des <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">rapports principaux clonables</a> afin que chaque unité opérationnelle utilise le plus souvent afin de réduire le temps nécessaire pour extraire le rapport et garantir l’exactitude des données. Voir les détails dans le <a href="#global-reports">tableau Rapports globaux ci-dessous</a>.
    <ul><li>Rapport Performance des personnes (tout temps et en fonction du temps) par source, mois</li>
    <li>Rapport Performance du programme (par mois de coût, en fonction du temps)</li>
    <li>Rapport Performance des emails (en fonction du temps)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Activez "Reporting global"</a> dans l’onglet Configuration du rapport afin d’inclure les données de tous vos espaces de travail dans les rapports Performances des emails et Performances des liens d’email. Si vous disposez de plusieurs espaces de travail, vous n’avez qu’à les activer dans l’espace de travail par défaut.</li>
    <p><img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : créez la <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">liste dynamique</a> avec les filtres que vous souhaitez inclure dans la plupart de vos rapports dans la section Base de données . Lorsque vous devez mettre à jour les critères de liste dynamique, vous pouvez les mettre à jour à un seul emplacement au lieu de les mettre à jour dans tous les rapports globaux.</td>
  </tr>
</tbody>
</table>

## Abonnements {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Abonnements</td>
    <td><li>Alignez votre responsable marketing sur les personnes qui doivent consulter les résultats des rapports et leur cadence pendant la mise en oeuvre.</li> <li>Utilisez les abonnements pour distribuer des données aux personnes qui en ont besoin dans votre entreprise sans utiliser de licence d’utilisateur nommée.</li>
    <p><img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : si vous souhaitez que les personnes accèdent aux données de rapport en temps réel, vous devez les ajouter en tant qu’utilisateurs afin qu’elles puissent afficher le rapport.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Configurez les abonnements</a> à la cadence souhaitée (quotidien/hebdomadaire/mensuel) pour la surveillance continue de chaque équipe. Vous pouvez également <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">afficher tous vos abonnements</a> à un seul emplacement sous l’onglet Abonnements dans Analytics.</li></td>
  </tr>
</tbody>
</table>

## Rapports globaux {#global-reports}

Identifiez les rapports qui doivent être partagés avec différents groupes d’utilisateurs au sein de votre organisation (équipe commerciale, direction marketing, par exemple). Créez une structure de dossiers appropriée pour chaque équipe, groupe d’utilisateurs ou unité opérationnelle afin d’organiser les rapports clonés dans les rapports de groupe. Envisagez de configurer des rapports globaux, tels que :

<table>
<thead>
  <tr>
    <th style="width:20%">Type de rapport</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rapport des performances des e-mails</td>
    <td><li>Créez des rapports globaux, Workspace/Business Unit avec les emails sélectionnés.</li>
    <li>Créez un rapport de performances des emails local dans tous vos modèles de programme clonables.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Utilisez une période appropriée</a> (par exemple, YTD, les 90 derniers jours, etc.) pour que le rapport fournisse une vue exacte des mesures standard d’engagement et de délivrabilité des emails.</li>
    <p><img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Activez le filtrage Activité de robot dans <strong>Admin &gt; Email</strong></a> afin d’éviter la journalisation ou d’identifier si la journalisation est activée pour les activités de robots. Insérez le filtre pour n’autoriser que les activités <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Ayant ouvert/cliqué avec l’"activité de robot" limitées à "False"</a> dans la liste dynamique de vos rapports globaux pouvant être clonés.</td>
  </tr>
  <tr>
    <td>Rapport Performances des personnes</td>
    <td><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : Il est recommandé d’avoir une <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">stratégie de canal et de balise</a> appropriée pour chaque mise en oeuvre de Marketo Engage avant de pouvoir effectuer le suivi des personnes acquises et du retour sur investissement de vos investissements marketing par canal.
    <p>
    <li>Déterminez les critères que vous utiliserez pour mesurer les performances de vos programmes d’acquisition de prospects et créez vos rapports standard en fonction du temps (année en cours, 12 derniers mois en continu, ou 180 jours) en fonction de ces mesures : <ul><li>Programme d’acquisition : programme de Marketo Engage crédité pour l’acquisition de la personne.</li>
    <li>Source Personne : catégorie source de la manière dont l’enregistrement a été connu pour votre base de données (en fonction de la liste source des valeurs dans votre CRM).
    </li></ul>
    <li>Mesure les personnes créées par semaine ou par mois. Ce rapport vous fournira une mesure du taux de croissance de votre base de données et vous indiquera si vous approchez de la limite de taille de la base de données.</li>
    <li>Filtrez les mesures dans les rapports sur les performances des personnes en <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">utilisant vos listes dynamiques comme colonnes personnalisées.</a></li>
    <p><img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : créez des listes dynamiques pour les colonnes personnalisées que vous souhaitez ajouter au rapport Performance des personnes dans la base de données au lieu d’activités marketing afin que vous puissiez afficher le nom de liste dynamique correctement et clairement lorsqu’il est sélectionné dans le rapport.</td>
  </tr>
  <tr>
    <td>Rapport Performance du programme</td>
    <td><p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : Ce rapport nécessite que vos canaux, états de progression et étapes de succès soient définis dans <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Admin</strong> &gt; <strong>Balises</strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Mesurez l’efficacité de vos tactiques marketing</a> dans des programmes sélectionnés.</li>
    <li>Gérez l’appartenance au programme (à l’aide des campagnes intelligentes pour mettre à jour le programme d’acquisition, l’état, l’état de réussite) en fonction des bonnes pratiques des activités marketing.</li>
    <li>Mesure basée sur les coûts pour l'année en cours et 12 mois en cours.
    <ul><li>Souvenez-vous que la maintenance des <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">coûts de la période</a> est essentielle pour tirer parti du rapport Performance du programme.</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : pour agréger et afficher toutes les <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">listes importées</a> dans les rapports Performance du programme, assurez-vous que vos équipes sélectionnent le programme d’acquisition approprié pour le balisage. Envisagez de <a href="https://experienceleague.adobe.com/fr/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">créer un programme par défaut</a> à sélectionner comme programme d’acquisition lorsque les listes importées ne s’appliquent à aucun canal. Ainsi, toute personne importée dispose d’un programme d’acquisition valide lié à la source, l’unité opérationnelle, le canal, etc., au lieu d’une valeur vide.</td>
  </tr>
  <tr>
    <td>Rapport Performance de page d’entrée</td>
    <td><li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">rapport Performance de page d’entrée</a> comme rapport global afin de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report"> filtrer et revoir les nombres</a> de toutes vos pages d’entrée Design Studio/Activités marketing à un seul endroit.</li>
    <li>Pour les programmes avec une ou plusieurs landing pages, pensez à <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">créer un rapport local dédié dans le modèle de programme</a> afin que vous puissiez passer en revue les performances au niveau du programme.</li></td>
  </tr>
  <tr>
    <td>Rapport Activité de la page web</td>
    <td><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : seules les pages web (pages d’entrée externes et Marketo) pour lesquelles <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">le Munchkin JavaScript</a> est activé feront l’objet d’un suivi dans ce rapport. Pensez à placer le code JavaScript dans la plateforme Tag Management, par exemple <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Gestionnaire de balises Google</a>, afin d’éviter de coder en dur le code sur chaque page web.
    <p>
    <li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report"> rapport d’activité de page web </a> comme rapport global afin de pouvoir consulter le nombre de toutes vos pages web à un seul endroit. Notez que vos activités de page Web externes ne sont reflétées que dans les rapports Activité de page Web .</li></td>
  </tr>
</tbody>
</table>

## Rapports locaux {#local-reports}

Il est préférable de déployer certains rapports de Marketo Engage en tant que ressources locales dans des programmes spécifiques des activités marketing, car leur utilisation type se trouve dans un ensemble plus limité de programmes et de ressources. Envisagez de configurer des rapports de base, tels que :

<table>
<thead>
  <tr>
    <th style="width:20%">Type de rapport</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rapport Performance des liens de courriel</td>
    <td><li>Créez un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">rapport Performance de lien de courriel</a> dans les programmes qui envoient des courriers électroniques et vos campagnes au goutte à goutte pour vous donner des informations sur les liens sur lesquels les visiteurs cliquent dans vos envois de courrier électronique.</li></td>
  </tr>
  <tr>
    <td>Rapport Activité de campagne</td>
    <td><li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">rapport d’activité de campagne</a> et sélectionnez un point dans votre dossier opérationnel dans Activités marketing.</li>
    <li>Configurez des rapports pour surveiller les déclencheurs pour chaque cas d’utilisation et <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">appliquer des filtres de campagne</a> (par exemple, déclencheurs de notation de comportement, déclencheurs de qualification du cycle de vie, déclencheurs de moments intéressants).</li></td>
  </tr>
  <tr>
    <td>Rapport Performances du flux d’engagement (le cas échéant)</td>
    <td><li>Créez un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">rapport Performance de flux d’engagement</a> pour mesurer l’efficacité du contenu et du flux déployés dans votre programme d’engagement.</li>
    <li>Envisagez d’utiliser le filtre <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank"> "Segmentation" dans l’onglet Configuration du rapport </a> et de regrouper les données de rapport par le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segment</a> (par exemple, source de la personne, secteur industriel) utilisé dans votre programme d’engagement. Vous obtiendrez ainsi des informations plus approfondies sur les schémas d’engagement de chaque segment, en vous guidant pour apporter des modifications stratégiques afin d’améliorer votre programme d’engagement (contenu, diffusion en continu, cadence de diffusion, etc.).</li></td>
  </tr>
</tbody>
</table>
