---
unique-page-id: 12979858
description: FAQ sur les informations de performance - Documents Marketo - Documentation du produit
title: FAQ sur les statistiques sur les performances
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 0%

---

# FAQ sur les statistiques sur les performances {#performance-insights-faq}

## Quelle est la définition de la &quot;réussite&quot; dans l’onglet Engagement ? {#what-is-the-definition-of-success-in-the-engagement-tab}

Le succès est une mesure de l’interaction significative dans Marketo. Le but d&#39;un programme est de créer une interaction significative avec la personne ou le prospect. Le succès est marqué lorsqu’une personne atteint l’état qui atteint cet objectif. Il peut assister à un webinaire, cliquer sur un lien dans un email ou remplir un formulaire web. Le succès varie en fonction du canal du programme.

>[!NOTE]
>
>Dans un programme de webinaire, plusieurs statuts peuvent être associés, par exemple : Invité, Enregistré et Participant. Invité ou Enregistré ne sont pas des interactions significatives parce que les gens ne regardent pas vraiment le webinaire. Participé est considéré comme une réussite dans ce cas.

## Les MPI fonctionneront-ils avec n’importe quel CRM ? {#will-mpi-work-with-any-crm}

Oui. Techniquement, MPI n’interagit pas directement avec le CRM pour la synchronisation des données. MPI utilise les données stockées dans le Data Warehouse Marketo Analytics. Comme la synchronisation CRM se produit dans l’application de gestion de la piste, tout CRM pris en charge par Marketo intégré à l’application de gestion de la piste affichera correctement les données. Toutefois, les champs d&#39;opportunité CRM doivent être correctement mappés aux champs d&#39;opportunité Marketo.

## Je n’ai aucun autre produit Marketing Analytics (ARB, RCE, RCA, Program Analysis). MPI fonctionnera-t-il pour moi ? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI est un module complémentaire indépendant de l’application Lead Management. Elle ne nécessite l’utilisation d’aucun autre produit d’analyse.

## RCA m’affiche également les données de performances du programme. Y a-t-il une différence entre les données affichées dans MPI et RCA ? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Nombre MPI génère des données à partir du même entrepôt de données que RCA. Par conséquent, vous ne verrez aucune différence de données entre les deux. RCA vous permet de créer vos propres rapports à la volée. MPI vous donne accès à des tableaux de bord visuels faciles à comprendre.

## Je ne veux pas que certains de mes programmes (p. ex. Opérationnels) s’affichent dans MPI. Comment contrôler la visibilité de programmes spécifiques ? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Vous pouvez contrôler la visibilité de vos programmes en définissant le comportement Analytics de vos programmes sur Opérationnel. Le programme sera alors exclu des calculs d’analyse.

>[!NOTE]
>
>En savoir plus sur la définition du comportement d’analyse [ici](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## J’exécute une campagne multicanal pour un nouveau lancement de produit. Comment puis-je visualiser les performances de cette campagne sur tous les différents canaux au même endroit ? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Nous vous recommandons d’utiliser des balises de programme pour les programmes faisant partie d’une telle campagne. Les balises de programme sont automatiquement synchronisées avec MPI et vous pouvez les filtrer dans tous les tableaux de bord MPI pour afficher les performances de votre campagne multicanal.

## Ai-je accès aux paramètres d’attribution si je ne dispose pas de RCA ? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Vous avez accès aux paramètres d’attribution si vous disposez d’une MPI, que vous ayez ou non une RCA.

## Une alerte s’affiche dans MPI lorsque je me connecte pour me signaler que mes paramètres d’attribution sont incorrects. Qu&#39;est-ce qui ne va pas ? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcule si toutes vos opportunités sont incluses ou non dans les analyses. Dans le cas contraire, vous serez invité à modifier vos paramètres d’attribution (explicite, implicite, hybride) afin d’inclure davantage d’opportunités.

Il se peut également que vous manquiez des opportunités en raison de l’absence du coût du programme dans vos programmes. Veuillez consulter le comportement d’Analytics de vos programmes. Ils peuvent être :

1. Par défaut : le comportement par défaut est que le programme serait inclus en MPI UNIQUEMENT s’il existe au moins un coût de période, même si aucun dollar est affecté.

1. Inclusif : cette option garantit que le programme est disponible en MPI, que vous ayez inclus ou non un coût de période.

1. [Opérationnel](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Cette option entraîne l’affichage du programme dans MPI.

>[!NOTE]
>
>Le coût de la période **doit être configuré pour la création de rapports Succès et Noms dans le tableau de bord Engagement.** Ce tableau de bord utilise les données de coût de période pour agréger les succès et les nouveaux noms. Si le coût de la période n’est pas configuré, le tableau de bord de l’engagement ne sera pas correctement reporté, quels que soient les paramètres de comportement d’Analytics ci-dessus.

## Pourquoi manque-t-il certaines opportunités dans MPI ? {#why-am-i-missing-some-opportunities-in-mpi}

Voici deux raisons clés pour lesquelles vous ne disposez peut-être pas d’opportunités dans MPI :

1. Le paramètre d’attribution est défini sur Explicite, mais les rôles de contact ne sont pas attribués aux opportunités.
1. Le coût de la période n’est pas inclus dans vos programmes

MPI calcule si toutes vos opportunités sont incluses ou non dans les analyses. Dans le cas contraire, vous serez invité à modifier vos paramètres d’attribution (explicite, implicite, hybride) afin d’inclure davantage d’opportunités.

Il se peut également que vous manquiez des opportunités en raison de l’absence du coût du programme dans vos programmes. L&#39;alerte apparaîtra mais ne vous indique pas quels programmes manquent de coûts. Veuillez consulter la configuration de votre programme pour inclure les coûts, afin de vous assurer que tous vos programmes et opportunités sont inclus dans l’API.

## Pourquoi ne vois-je pas les filtres Champs personnalisés, Type d’opportunité et ABM dans le tableau de bord Engagement ? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Les champs personnalisés, le type d’opportunité et les filtres ABM sont tous des attributs liés à une opportunité. Le tableau de bord Engagement vous permet de mesurer votre engagement et l’acquisition de prospects, qu’ils soient associés ou non à une opportunité. Comme le tableau de bord Engagement ne prend pas en compte l’opportunité, les champs personnalisés, le type d’opportunité et les filtres ABM ne s’appliquent pas.

## Je souhaite utiliser un champ Opportunité Salesforce personnalisé pour la création de rapports de recettes au lieu du champ Montant d’opportunité Salesforce standard. Est-ce que MPI me permettra de faire ça ? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Oui. [ L’assistance de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) peut mapper le champ Montant de l’opportunité de Marketo sur un champ Opportunité Salesforce personnalisé tant que le type de champ est une devise. Puisque MPI pointe vers le champ Montant d’opportunité Marketo, MPI peut utiliser les données du champ personnalisé Salesforce mappé.

>[!NOTE]
>
>Après le mappage, MPI affichera les données à venir. Le montant historique ne sera pas modifié.

## Si je n’utilise pas les opportunités, puis-je toujours utiliser MPI ? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI est conçu pour vous permettre de mesurer les performances du programme du haut de l’entonnoir jusqu’à l’impact sur les recettes. Si vous n’utilisez pas les opportunités, vous pourrez toujours :

* Affichez les performances de vos programmes de formation pour l’engagement de l’audience.
* Afficher les performances de vos programmes d’acquisition de prospects.
* Afficher les performances des campagnes multicanaux par le biais de balises de programme.
* Voir les tendances d’engagement de l’audience pour les 12 derniers mois.
* Enregistrez et exportez les données de performances dans PowerPoint.

## Puis-je mesurer le succès des stratégies basées sur les comptes dans MPI ? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Oui. MPI s’intègre à [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) pour extraire en toute transparence les listes de comptes ABM en MPI. Vous pouvez utiliser le filtre Liste des comptes ABM pour choisir la liste ABM dont vous souhaitez filtrer les données.

## L’attribution est-elle instantanément disponible lorsque j’achète des MPI ? {#is-attribution-instantly-available-when-i-purchase-mpi}

Les fonctionnalités d’attribution Marketo sont disponibles pour nos clients lorsqu’ils achètent des MPI. Cependant, la [configuration appropriée](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) est requise pour s’assurer que les opportunités et les données de programme se déplacent correctement dans MPI.

## Que dois-je faire pour configurer l’attribution ? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuration de l’opportunité

   1. Vérifiez que les opportunités sont synchronisées avec votre CRM
   1. Si vos paramètres d’attribution sont définis sur Explicite, assurez-vous que les rôles de contact sur les opportunités sont renseignés.
   1. Nous vous recommandons de modifier le paramètre d’attribution en Hybride.
   1. Configuration du programme

      1. Inclure le coût du programme dans vos programmes
      1. Examinez le comportement des analyses pour indiquer si un programme doit être inclus dans les analyses.
      1. Définissez les critères de réussite pour chaque canal que vous avez
      1. Liaison de personne à un programme

         1. Assurez-vous que le programme d’acquisition et la date d’acquisition ont été définis pour chaque personne de votre base de données afin que l’attribution Première touche fonctionne.
         1. S’assurer que vos programmes définissent des états de réussite pour les personnes de votre base de données

>[!TIP]
>
>Toutes les étapes de configuration requises sont détaillées dans [cet article](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Quelle est la différence entre MPI et l’analyseur de programme ? {#whats-the-difference-between-mpi-and-the-program-analyzer}

L’analyseur de programme vous permet de comparer vos programmes pour quatre mesures au maximum. MPI vous permet d’analyser la contribution de votre canal et de votre programme à une mesure choisie, comme Réussite, Nouvelles opportunités créées, etc. Il vous permet également d’afficher la tendance de canal sur 12 mois en fonction d’une mesure spécifique que vous avez choisie.

## Quelle est la différence entre MPI et le Report Builder avancé ? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Le Report Builder avancé (parfois appelé RCE) est conçu pour les rapports en libre-service (ou ad hoc), généralement effectués par les opérations marketing. MPI est conçu pour permettre aux responsables marketing et aux marketeurs d’accéder en un clic à l’analyse des performances. Une configuration minimale est requise.

## Qu’est-il advenu de l’option &quot;Année précédente&quot; dans le filtre de dates des contributions ? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Nous avons temporairement supprimé la sélection &quot;Année précédente&quot;. Vous avez toujours la possibilité d’afficher les données de performances de l’année entière à l’aide de la sélection Période personnalisée .
