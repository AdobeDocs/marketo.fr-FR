---
description: Configurez la section Analytics pour votre nouvelle instance Marketo Engage.
title: Bonnes pratiques relatives aux nouvelles instances - Liste de contrôle Analytics
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 1%

---

# Bonnes pratiques relatives aux nouvelles instances : liste de contrôle d’Analytics {#new-instance-best-practices-analytics-checklist}

La section Analytics propose des rapports globaux qui analysent la performance de vos efforts marketing. Découvrez les étapes nécessaires pour y accéder.

N’oubliez pas de [télécharger les listes de contrôle](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) et de suivre vos progrès.

## Arborescence {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Organisation : nommage, dossiers et archivage</td>
    <td><li>Utilisez une convention de nommage des rapports pour différencier les rapports dans l’onglet Rapports globaux .
    <ul><li>Un exemple de bonne pratique en matière de convention d’affectation des noms est [Type de rapport] [Balise globale ou spécifique à l’unité opérationnelle] [Description du rapport] telle que [Performances des e-mails]-[Global]-[Engagement des e-mails pendant 180 jours].</li></ul><br>
    <li>Identifiez les rapports qui doivent être partagés avec différents groupes d’utilisateurs au sein de votre organisation (par exemple, l’équipe des ventes, la direction marketing) et organisez les rapports par dossier dans le dossier Rapports de groupe dans Analytics pour les rapports globaux.</li>
    <li>L’archivage doit être limité au dossier Rapports globaux, car il s’agit de rapports permanents.   <ul><li>Limitez l’archivage aux changements organisationnels tels que la réduction ou l’ajout d’unités opérationnelles pertinentes si vous créez des rapports basés sur une structure d’unité opérationnelle.</li></ul>
    </td>
  </tr>
  <tr>
    <td>Espaces de travail (le cas échéant)</td>
    <td><li>Répliquez les rapports globaux et la structure de dossiers sur les espaces de travail afin de maintenir la cohérence des rapports pour vos équipes. Ces rapports se trouvent dans le dossier Rapports de groupe.</li></td>
  </tr>
  <tr>
    <td>Mes rapports</td>
    <td><li>Identifiez et créez les rapports à utiliser dans la section <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Mes rapports</a>. Utilisez cette section de rapport privée comme sandbox pour les rapports globaux. Ils ne sont disponibles que pour l’utilisateur ou l’utilisatrice qui crée le rapport.</li>
    <li>Utilisez la convention de nommage de votre organisation pour identifier le rapport et l’utilisation afin de réconcilier les rapports dans Mes rapports avec les rapports dans les rapports de groupe.</li></td>
  </tr>
  <tr>
    <td>Rapports de groupe</td>
    <td><li>Les rapports de groupe sont les rapports globaux de votre organisation et doivent générer des rapports sur l’activité globale de votre organisation.</li>
    <li>Pensez à créer des <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">rapports principaux clonables</a> que chaque unité opérationnelle utilisera le plus souvent afin de réduire le temps nécessaire à l’extraction du rapport et de garantir l’exactitude des données. Consultez les détails dans le <a href="#global-reports">tableau Rapports globaux ci-dessous</a>.
    <ul><li>Rapport sur les performances des personnes (à tout moment et basé sur l’heure) par source, mois</li>
    <li>Rapport sur l'exécution du programme (par mois de coût, par période)</li>
    <li>Rapport sur les performances des e-mails (basé sur le temps)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Activez le « reporting global »</a> dans l'onglet Configuration du rapport pour inclure les données de tous vos espaces de travail dans les rapports Performance des e-mails et Performance des liens d'e-mail. Si vous disposez de plusieurs espaces de travail, il vous suffit de les activer dans l’espace de travail par défaut.</li>
    <p><img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : créez la <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">liste dynamique</a> avec les filtres que vous souhaitez inclure dans la plupart de vos rapports dans la section Base de données . Lorsque vous devez mettre à jour les critères de la liste dynamique, vous pouvez le faire à un seul endroit au lieu de le faire dans tous les rapports globaux.</td>
  </tr>
</tbody>
</table>

## Abonnements {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Abonnements</td>
    <td><li>Alignez-vous sur votre responsable marketing concernant les personnes qui doivent examiner les résultats des rapports et leur cadence pendant la mise en œuvre.</li> <li>Utilisez les abonnements pour distribuer des données aux personnes qui ont besoin de connaître votre entreprise sans épuiser une licence utilisateur nommée.</li>
    <p><img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : si vous souhaitez que les utilisateurs accèdent aux données des rapports en temps réel, vous devez les ajouter en tant qu’utilisateurs afin qu’ils puissent consulter le rapport.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Configurez les abonnements</a> à la cadence souhaitée (quotidienne/hebdomadaire/mensuelle) pour la surveillance continue de chaque équipe. Vous pouvez également <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">afficher tous vos abonnements</a> au même endroit sous l’onglet Abonnements dans Analytics.</li></td>
  </tr>
</tbody>
</table>

## Rapports globaux {#global-reports}

Identifiez les rapports qui doivent être partagés avec différents groupes d’utilisateurs au sein de votre organisation (par exemple, l’équipe des ventes, la direction marketing). Créez une structure de dossiers appropriée pour chaque équipe, groupe d’utilisateurs ou unité opérationnelle afin d’organiser les rapports clonés dans les rapports de groupe. Envisagez de configurer des rapports globaux, tels que :

<table>
<thead>
  <tr>
    <th style="width:20%">Type de rapport</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rapport des performances des e-mails</td>
    <td><li>Créez des rapports globaux, Workspace/au niveau de l’unité opérationnelle avec les e-mails corrects sélectionnés.</li>
    <li>Créez un rapport local sur les performances des e-mails dans tous vos modèles de programme clonables.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Utilisez un délai approprié</a> (par exemple, YTD, 90 derniers jours, etc.) pour que le rapport fournisse une vue précise de l’engagement des e-mails standard et des mesures de délivrabilité.</li>
    <p><img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Activez le filtrage 'Activité des robots' dans <strong>Admin &gt; E-mail</strong></a> pour éviter la journalisation ou déterminer si celle-ci est activée pour les activités des robots. Incluez le filtre pour autoriser uniquement les activités <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Ouvertes/ayant fait l’objet d’un clic avec la contrainte « Est une activité de robot » définie sur « False »</a> dans la liste dynamique de vos rapports globaux pouvant être clonés.</td>
  </tr>
  <tr>
    <td>Rapport sur les performances des personnes</td>
    <td><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : il est recommandé d’adopter une stratégie <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">canal et balises)</a> appropriée pour chaque implémentation de Marketo Engage avant de pouvoir suivre les personnes acquises et le retour sur investissement de vos investissements marketing par canal.
    <p>
    <li>Déterminez les critères que vous utiliserez pour mesurer les performances de vos programmes d’acquisition de prospects et créer vos rapports standard temporels (année en cours, vue des 12 derniers mois variable ou 180 derniers jours) en fonction de ces mesures : <ul><li>Programme d’acquisition : programme Marketo Engage crédité pour l’acquisition de la personne.</li>
    <li>Source de la personne : catégorie source pour la manière dont votre base de données a appris à connaître l’enregistrement (en fonction de la liste source des valeurs dans votre CRM)
    </li></ul>
    <li>Mesurez les personnes créées par semaine ou par mois. Ce rapport vous permet de mesurer le taux de croissance de votre base de données et de déterminer si vous approchez de la limite de taille de votre base de données.</li>
    <li>Filtrez les mesures dans les rapports de performances des personnes en <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">utilisant vos listes dynamiques comme colonnes personnalisées.</a></li>
    <p><img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : créez des listes dynamiques pour les colonnes personnalisées que vous souhaitez ajouter au rapport Performances des personnes dans la base de données au lieu des activités marketing afin de voir correctement et clairement le nom de la liste dynamique lorsqu’il est sélectionné dans le rapport.</td>
  </tr>
  <tr>
    <td>Rapport sur l'exécution du programme</td>
    <td><p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : ce rapport nécessite que vos canaux, statuts de progression et étapes de succès soient définis dans <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Admin</strong> &gt; <strong>Balises</strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Mesurez l’efficacité de vos tactiques marketing</a> dans le cadre de programmes sélectifs.</li>
    <li>Gérez l’appartenance au programme (à l’aide de campagnes intelligentes pour mettre à jour le programme d’acquisition, le statut, les statuts de réussite) en fonction des bonnes pratiques des activités marketing.</li>
    <li>Mesure fondée sur les coûts pour l'année en cours et les 12 mois consécutifs.
    <ul><li>N’oubliez pas que le maintien des <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">coûts de la période</a> est essentiel pour tirer parti du rapport sur le rendement du programme.</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="icône de note"> CONSEIL : pour agréger et afficher les listes <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">importées</a> dans les rapports de performance du programme, assurez-vous que vos équipes sélectionnent le programme d’acquisition approprié pour le balisage. Pensez à <a href="https://experienceleague.adobe.com/fr/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">créer un programme par défaut</a> à sélectionner comme programme d’acquisition lorsque les listes importées ne s’appliquent à aucun canal. Cela permet de s’assurer qu’une personne importée dispose d’un programme d’acquisition valide lié à la source, à l’unité opérationnelle, au canal, etc., au lieu d’une valeur vide.</td>
  </tr>
  <tr>
    <td>Rapport sur les performances des pages de destination</td>
    <td><li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Rapport de performances sur les pages de destination</a> sous la forme d’un rapport global afin de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrer et passer en revue les chiffres</a> de toutes vos pages de destination Design Studio/Activités marketing au même endroit.</li>
    <li>Pour les programmes dotés de page(s) de destination, pensez à <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">créer un rapport local dédié dans le modèle de programme</a> afin que vous puissiez examiner les performances au niveau du programme.</li></td>
  </tr>
  <tr>
    <td>Rapport d’activité de la page web</td>
    <td><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : seules les pages web (pages de destination externes et Marketo) pour lesquelles le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">JavaScript Munchkin</a> est activé seront suivies dans ce rapport. Pensez à placer le code JavaScript dans la plateforme Tag Management, par exemple dans le <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Gestionnaire de balises Google</a>, pour éviter de le coder en dur sur chaque page web.
    <p>
    <li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Rapport d’activité de la page web</a> en tant que rapport global afin de pouvoir consulter les numéros de toutes vos pages web au même endroit. Notez que les activités de vos pages web externes ne sont reflétées que dans les rapports Activité des pages web .</li></td>
  </tr>
</tbody>
</table>

## Rapports locaux {#local-reports}

Il est préférable de déployer certains rapports Marketo Engage en tant que ressources locales au sein de programmes spécifiques dans les activités marketing, car leur utilisation classique se fait dans un ensemble plus limité de programmes et de ressources. Envisagez de configurer des rapports de base, tels que :

<table>
<thead>
  <tr>
    <th style="width:20%">Type de rapport</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rapport sur les performances des liens d’e-mail</td>
    <td><li>Créez un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">Rapport de performances des liens d’e-mail</a> dans les programmes qui envoient des e-mails et vos campagnes drip pour obtenir des informations sur les liens sur lesquels les personnes cliquent dans votre e-mail envoyé.</li></td>
  </tr>
  <tr>
    <td>Rapport d’activité de campagne</td>
    <td><li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Rapport d’activité de campagne</a> et choisissez une période dans votre dossier opérationnel dans Activités marketing.</li>
    <li>Configurez des rapports pour surveiller les déclencheurs pour chaque cas d’utilisation et <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">appliquez des filtres de campagne</a> (par exemple, déclencheurs de score de comportement, déclencheurs de qualification du cycle de vie, déclencheurs de moments significatifs).</li></td>
  </tr>
  <tr>
    <td>Rapport sur les performances du flux d'engagement (le cas échéant)</td>
    <td><li>Créez un <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">rapport de performance du flux d’engagement</a> pour mesurer l’efficacité du contenu et du flux déployés dans votre programme d’engagement.</li>
    <li>Utilisez le filtre <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank"> « Segmentation » dans l’onglet Configuration du rapport</a> et regroupez les données de rapport par le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segment</a> (par exemple, source de la personne, secteur) utilisé dans votre programme d’engagement. Vous obtiendrez ainsi des informations plus précises sur les modèles d’engagement de chaque segment, ce qui vous aidera à apporter des changements stratégiques pour améliorer votre programme d’engagement (contenu, flux, cadence de diffusion, etc.).</li></td>
  </tr>
</tbody>
</table>
