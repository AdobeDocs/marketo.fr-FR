---
description: Configurez la section Analytics pour votre nouvelle instance de Marketo Engage.
title: Bonnes pratiques relatives aux nouvelles instances - Liste de contrôle Analytics
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: a7b1ede27b8286f13fcb850ee49757e86e23dbd5
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 1%

---

# Bonnes pratiques relatives aux nouvelles instances : liste de contrôle Analytics {#new-instance-best-practices-analytics-checklist}

La section Analytics propose des rapports globaux qui analysent les performances de vos efforts marketing. Découvrez les étapes nécessaires pour les parcourir.

N’oubliez pas de [télécharger les listes de contrôle](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) et suivez vos progrès.

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
    <td><li>Utilisez une convention d’affectation des noms de rapport pour différencier les rapports dans l’onglet Rapports globaux .</li>
    <ul><li>Un exemple de bonne pratique de convention d’affectation des noms est [Type de rapport] [Balise globale ou spécifique à une unité d’exploitation] [Description du rapport], par exemple [Performance de messagerie]-[Global]-[Engagement de messagerie de 180 jours].</li></ul> <li>Identifiez les rapports qui doivent être partagés avec différents groupes d’utilisateurs au sein de votre organisation (par exemple, l’équipe commerciale, la direction marketing) et organisez les rapports par dossier dans le dossier Rapports de groupe d’Analytics pour les rapports globaux.</li> 
    <li>L’archivage doit être limité au dossier Rapports globaux, car il s’agit de rapports toujours actifs.   <ul><li>Limitez l’archivage aux modifications organisationnelles, telles que la réduction ou l’ajout d’unités opérationnelles pertinentes si vous créez des rapports en fonction d’une structure d’unités opérationnelles.</li></ul></td>
  </tr>
  <tr>
    <td>Espaces de travail (le cas échéant)</td>
    <td><li>Répliquez les rapports globaux et la structure de dossiers dans les espaces de travail, si vous utilisez Workspace, afin de maintenir des rapports cohérents pour vos équipes. Ces rapports seront contenus dans le dossier Rapports de groupe .</li></td>
  </tr>
  <tr>
    <td>Mes rapports</td>
    <td><li>Identifiez et créez les rapports nécessaires à votre utilisation dans la variable <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Mes rapports</a> . Utilisez cette section de rapport privé comme environnement de test pour les rapports globaux. Elles ne sont disponibles que pour l’utilisateur qui crée le rapport.</li>
    <li>Utilisez la convention d’affectation des noms de votre organisation pour identifier le rapport et son utilisation afin de pouvoir réconcilier vos rapports dans Mes rapports avec les rapports dans Rapports de groupe.</li></td>
  </tr>
  <tr>
    <td>Rapports de groupe</td>
    <td><li>Les rapports de groupe sont les rapports globaux de votre organisation et doivent générer des rapports sur l’activité globale de votre organisation Marketo Engage.</li>
    <li>Créer <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">rapports principaux clonables</a> vous attendez de chaque unité opérationnelle qu’elle utilise le plus pour réduire le temps nécessaire à l’extraction du rapport et pour garantir l’exactitude des données. Consultez les détails dans le tableau "Création de rapports de base - Rapports globaux" [INSÉRER LE LIEN VERS LA SECTION SIGNALÉE].
    <ul><li>Rapport Performance des personnes (tout temps et en fonction du temps) - par source, mois</li>
    <li>Rapport Performance du programme (par mois de coût, en fonction du temps)</li>
    <li>Rapport Performance des emails (en fonction du temps)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Activation du "reporting global"</a> dans l’onglet Configuration du rapport afin d’inclure les données de tous vos espaces de travail dans les rapports Performance de messagerie et Performance de lien de courriel . Si vous disposez de plusieurs espaces de travail, vous n’avez qu’à les activer dans l’espace de travail par défaut.</li>
    <br>CONSEIL : Créez la variable <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">Liste dynamique</a> avec les filtres que vous souhaitez inclure dans la plupart de vos rapports, dans la section "Base de données". Lorsque vous devez mettre à jour les critères de liste dynamique, vous pouvez les mettre à jour à un seul emplacement au lieu de les mettre à jour dans tous les rapports globaux.</td>
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
    <br>CONSEIL : les emails d’abonnement sont généralement envoyés la nuit. Si vous souhaitez que les utilisateurs accèdent aux données du rapport en temps réel, vous devez ajouter des personnes en tant qu’utilisateurs afin qu’ils puissent directement vérifier le rapport.
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Configuration des abonnements</a> selon la cadence désirable (quotidienne/hebdomadaire/mensuelle) pour la surveillance continue de chaque équipe. Vous pouvez également <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">afficher tous vos abonnements ;</a> à un emplacement sous l’onglet Abonnements dans Analytics.</li></td>
  </tr>
</tbody>
</table>

## Rapports globaux {#global-reports}

Identifiez les rapports qui doivent être partagés avec différents groupes d’utilisateurs au sein de votre organisation (équipe commerciale, direction marketing, par exemple). Créez une structure de dossiers appropriée pour chaque équipe, groupe d’utilisateurs ou unité opérationnelle afin d’organiser les rapports dans les rapports de groupe lors du clonage des rapports. Envisagez de configurer des rapports globaux tels que :

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
    <td><li>Créez des rapports globaux Workspace/Business Unit à l’échelle de l’entreprise avec les emails corrects sélectionnés.</li>
    <li>Créez un rapport de performance email local dans tous vos modèles de programme clonables.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Utiliser une période appropriée</a> (par exemple, JJ, les 90 derniers jours, etc.) pour que le rapport vous fournisse une vue exacte des mesures standard d’engagement et de délivrabilité des emails.</li>
    <br>CONSEIL : <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Activez le filtrage "Activité du robot" dans "Admin&gt;Email".</a> pour éviter de journaliser ou de déterminer si la journalisation est activée pour les activités de robots. <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Incluez le filtre pour autoriser uniquement les activités Ouvert/Cliqué avec l’option "Is Bot Activity" contrainte définie sur "False".</a> dans la liste dynamique de vos rapports globaux clonables.</td>
  </tr>
  <tr>
    <td>Rapport Performances des personnes</td>
    <td>REMARQUE : Il est recommandé d’avoir une <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">stratégie de canal et de balise</a> pour chaque mise en oeuvre de Marketo Engage avant de pouvoir effectuer le suivi des personnes acquises par le biais de chacune d’elles, ainsi que du retour sur investissement de vos investissements marketing par canal.
    <br>
    <li>Déterminez les critères que vous utiliserez pour mesurer les performances de vos programmes d’acquisition de prospects et créez vos rapports standard en fonction du temps (année en cours, 12 derniers mois en continu, ou 180 jours) en fonction de ces mesures :</li> <ul><li>Programme d’acquisition : programme de Marketo Engage crédité pour l’acquisition du prospect.</li>
    <li>Source de personne : catégorie source de la manière dont l’enregistrement a été connu pour votre base de données (basée sur la liste source des valeurs dans votre CRM).</li></ul>
    <li>Mesure les personnes créées par semaine ou par mois. Ce rapport vous donnera une mesure du taux de croissance de votre base de données et vous indiquera si vous approchez ou dépasserez bientôt votre limite de taille de base de données.</li>
    <li>Filtrez les mesures dans les rapports sur les performances des personnes en <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">en utilisant vos listes dynamiques comme colonnes personnalisées.</a></li>
    <br>CONSEIL : créez les listes dynamiques pour les colonnes personnalisées que vous souhaitez ajouter au rapport Performances des personnes dans la base de données au lieu des activités marketing. Vous pouvez ainsi afficher le nom de la liste dynamique correctement et clairement lorsqu’il est sélectionné dans le rapport.</td>
  </tr>
  <tr>
    <td>Rapport Performance du programme</td>
    <td>REMARQUE : pour ce rapport, les canaux, les états de progression et les étapes de succès doivent être définis dans la variable <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel">Admin &gt; Zone Balises</a>. <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Mesurer l’efficacité de vos tactiques marketing</a> dans des programmes sélectifs.</li>
    <li>Gérez l’appartenance au programme (à l’aide des campagnes intelligentes pour mettre à jour le programme d’acquisition, l’état, l’état de réussite) en fonction des bonnes pratiques des activités marketing.</li>
    <li>Mesure basée sur les coûts de l'année en cours et variable de 12 mois.
    <ul><li>N’oubliez pas que la maintenance <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">Coûts de la période</a> est essentiel pour tirer parti du rapport Performance du programme.</li>
    <br>CONSEIL : pour agréger et afficher toute <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">listes importées</a> dans les rapports de performances du programme, assurez-vous que vos équipes sélectionnent le programme d’acquisition approprié pour le balisage. Étudier <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">création d’un programme par défaut</a> à sélectionner comme programme d’acquisition lorsque les listes importées ne s’appliquent à aucun canal. Ainsi, toute personne importée dispose d’un programme d’acquisition valide lié à sa source, son unité opérationnelle, son canal, etc. au lieu d’une valeur vide.</td>
  </tr>
  <tr>
    <td>Rapport Performance de page d’entrée</td>
    <td><li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Rapport Performance de page d’entrée</a> en tant que rapport global afin que vous puissiez <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrer et vérifier les nombres</a> de toutes vos pages d’entrée ou d’entrée d’activités marketing de Design Studio au même endroit.</li>
    <li>Pour les programmes avec une ou plusieurs landing pages, envisagez <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">créer un rapport local dédié dans le modèle de programme</a> vous pouvez ainsi examiner les performances au niveau du programme.</li></td>
  </tr>
  <tr>
    <td>Rapport Activité de la page web</td>
    <td>REMARQUE : seules les pages web (pages externes et de destination Marketo) qui comportent des <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">le code JavaScript Munchkin</a> enabled sera suivi dans ce rapport. Envisagez de placer le code JavaScript dans la plateforme Tag Management, par exemple <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Gestionnaire de balises de Google</a>, afin d’éviter de coder en dur le code sur chaque page web.
    <br>
    <li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Rapport Activité de la page web</a> en tant que rapport global, afin que vous puissiez consulter le nombre de toutes vos pages web au même endroit. Notez que vos activités de page Web externes ne sont reflétées que dans les rapports Activité de page Web .</li></td>
  </tr>
</tbody>
</table>

## Rapports locaux {#local-reports}

Il est préférable de déployer certains rapports de Marketo Engage en tant que ressources locales dans des programmes spécifiques des &quot;Activités marketing&quot;, car leur meilleure utilisation est dans un ensemble plus limité de programmes et de ressources. Envisagez de configurer des rapports de base, tels que :

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
    <td><li>Créer <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">Rapport Performance des liens de courriel</a> dans les programmes qui envoient des emails et vos campagnes gouttes pour vous donner des informations sur les liens sur lesquels les utilisateurs cliquent dans vos envois de courrier électronique.</li></td>
  </tr>
  <tr>
    <td>Rapport Activité de campagne</td>
    <td><li>Créez le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Rapport Activité de campagne</a> et choisissez une période dans votre dossier opérationnel dans "Activités marketing".</li>
    <li>Configuration de rapports pour surveiller les déclencheurs pour chaque cas d’utilisation et <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">appliquer des filtres de campagne ;</a>, par exemple, les déclencheurs de notation de comportement, les déclencheurs de qualification de cycle de vie, les déclencheurs de moments intéressants.</li></td>
  </tr>
  <tr>
    <td>Rapport Performances du flux d’engagement (le cas échéant)</td>
    <td><li>Créer <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">Rapport Performances du flux d’engagement</a> pour mesurer l’efficacité du contenu et de la diffusion déployés dans le cadre de votre programme d’engagement.</li>
    <li>Étudier <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">en utilisant le filtre "Segmentation" dans l’onglet Configuration du rapport.</a> et regrouper les données du rapport par le <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segment</a> (source de personnes, secteur d’activité, par exemple) utilisé dans votre programme d’engagement. Vous obtiendrez ainsi des informations plus approfondies sur les schémas d’engagement de chaque segment, en vous guidant pour apporter des modifications stratégiques afin d’améliorer votre programme d’engagement (contenu, diffusion en continu, cadence de diffusion, etc.).</li></td>
  </tr>
</tbody>
</table>
