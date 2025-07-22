---
unique-page-id: 12979858
description: FAQ sur Performance Insights - Documents Marketo - Documentation du produit
title: FAQ sur Performance Insights
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 0%

---

# [!UICONTROL FAQ sur Performance Insights] {#performance-insights-faq}

## Quelle est la définition du terme « succès » dans l’onglet [!UICONTROL Engagement] ? {#what-is-the-definition-of-success-in-the-engagement-tab}

La réussite est une mesure d’interaction significative dans Marketo. L&#39;objectif d&#39;un programme est de créer une interaction significative avec la personne ou le prospect. La réussite est marquée lorsqu’une personne atteint le statut qui permet d’atteindre cet objectif. Il peut s’agir de participer à un webinaire, de cliquer sur un lien dans un e-mail ou de remplir un formulaire web. Le succès varie en fonction du canal du programme.

>[!NOTE]
>
>Dans un programme de webinaire, il peut y avoir plusieurs statuts, tels que : Invité, Enregistré et Participé. Les interactions invitées ou enregistrées ne sont pas significatives, car les gens ne regardent pas le webinaire. Dans ce cas, le statut Terminé est considéré comme une réussite.

## MPI fonctionnera-t-il avec un CRM ? {#will-mpi-work-with-any-crm}

Oui. Techniquement, MPI n’interagit pas directement avec le CRM pour la synchronisation des données. MPI utilise les données stockées dans le Data Warehouse Marketo Analytics. Comme la synchronisation CRM se produit dans l’application de gestion des leads, tout CRM pris en charge par Marketo intégré à l’application de gestion des leads affichera correctement les données. Toutefois, les champs d’opportunité CRM doivent être correctement mappés aux champs d’opportunité Marketo.

## Je n’ai aucun autre produit d’analyse marketing (ARB, RCE, RCA, analyse de programme). MPI fonctionnera-t-il pour moi ? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI est un module complémentaire indépendant de l’application de gestion des prospects. Il ne nécessite pas l’utilisation d’autres produits d’analyse.

## RCA me montre aussi des données sur le rendement des programmes. Existe-t-il une différence entre les données affichées dans l’IPM et l’ARC ? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Non. MPI fournit des données du même entrepôt de données que RCA. Par conséquent, vous ne verrez aucune différence de données entre les deux. RCA vous permet de créer vos propres rapports à la volée. MPI vous donne accès à des tableaux de bord visuels faciles à comprendre.

## Je ne veux pas que certains de mes programmes (p. ex. opérationnels) s’affichent dans l’IPM. Comment puis-je contrôler la visibilité de programmes spécifiques ? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Vous pouvez contrôler la visibilité de vos programmes en définissant le comportement Analytics de vos programmes sur Opérationnel. Le programme sera alors exclu des calculs d’analyse.

>[!NOTE]
>
>En savoir plus sur la définition du comportement des analyses [ici](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## J’exécute une campagne multicanal pour le lancement d’un nouveau produit. Comment puis-je afficher les performances de cette campagne sur tous les canaux en un seul endroit ? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Nous vous recommandons d’utiliser les balises de programme pour les programmes qui font partie d’une telle campagne. Les balises de programme sont automatiquement synchronisées avec MPI et vous pouvez les filtrer dans tous les tableaux de bord MPI pour afficher les performances de votre campagne multicanal.

## Vais-je avoir accès aux paramètres d’attribution si je ne dispose pas de l’autorisation RCA ? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Vous avez accès aux paramètres d’attribution si vous disposez de l’API, que vous disposiez ou non de l’application RCA.

## Une alerte s’affiche dans l’API lorsque je me connecte pour me signaler que mes paramètres d’attribution sont incorrects. Qu’est-ce qui ne va pas ? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcule si toutes vos opportunités sont incluses ou non dans Analytics. Si ce n’est pas le cas, vous serez invité à envisager de modifier vos paramètres d’attribution (explicite, implicite, hybride) afin d’inclure d’autres opportunités.

Vous pouvez également manquer des opportunités en raison de l’absence du coût du programme dans vos programmes. Veuillez vérifier le comportement d’Analytics de vos programmes. Il peut s’agir :

1. Par défaut - Le comportement par défaut est que le programme est inclus dans MPI SEULEMENT s&#39;il y a au moins un coût de période, même si aucun montant n&#39;est affecté.

1. Inclusif - Cette option garantit que le programme est disponible dans MPI, que vous ayez inclus ou non un coût de période.

1. [Opérationnel](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Cette option fait en sorte que le programme n’apparaît pas dans l’indicateur de performance clé.

>[!NOTE]
>
>Le coût de la période **a** doit être configuré pour le compte rendu des performances Succès et Nouveaux noms dans le tableau de bord de l&#39;engagement. Ce tableau de bord utilise les données de coût de la période pour agréger les succès et les nouveaux noms. Si le coût de la période n’est pas configuré, le tableau de bord de l’engagement ne s’affiche pas correctement, quels que soient les paramètres de comportement Analytics ci-dessus.

## Pourquoi suis-je en train de rater des opportunités dans MPI ? {#why-am-i-missing-some-opportunities-in-mpi}

Deux raisons principales peuvent expliquer pourquoi vous manquez des opportunités dans MPI :

1. Le paramètre d’attribution est défini sur Explicite, mais aucun rôle de contact n’est affecté aux opportunités
1. Le coût de la période n’est pas inclus dans vos programmes

MPI calcule si toutes vos opportunités sont incluses ou non dans Analytics. Si ce n’est pas le cas, vous serez invité à envisager de modifier vos paramètres d’attribution (explicite, implicite, hybride) afin d’inclure d’autres opportunités.

Vous pouvez également manquer des opportunités en raison de l’absence du coût du programme dans vos programmes. L&#39;alerte sera lancée, mais ne vous indiquera pas quels programmes n&#39;ont pas de coûts. Veuillez vérifier la configuration de votre programme pour inclure les coûts, afin de vous assurer que tous vos programmes et opportunités sont inclus dans MPI.

## Pourquoi les champs personnalisés, le type d’opportunité et les filtres ABM ne s’affichent-ils pas sur le tableau de bord de l’engagement ? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Les champs personnalisés, le type d’opportunité et les filtres ABM sont tous des attributs liés à une opportunité. Le tableau de bord de l’engagement vous permet de mesurer votre engagement et l’acquisition de prospects, qu’ils soient associés ou non à une opportunité. Comme le tableau de bord de l’engagement ne prend pas en compte les opportunités, les champs personnalisés, le type d’opportunité et les filtres ABM ne s’appliquent pas.

## Je souhaite utiliser un champ d’opportunité Salesforce personnalisé pour le compte rendu des performances au lieu du champ montant de l’opportunité Salesforce standard. Est-ce que MPI me le permettra? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Oui. La prise en charge de [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) peut remapper le champ Montant de l’opportunité de Marketo vers un champ d’opportunité Salesforce personnalisé tant que le type de champ est devise. Comme MPI pointe vers le champ Montant de l’opportunité Marketo , MPI peut utiliser les données du champ Salesforce personnalisé remappé.

>[!NOTE]
>
>Après le remappage, MPI affichera les données à partir de maintenant. Le montant historique ne sera pas modifié.

## Si je n’utilise pas les opportunités, puis-je quand même utiliser MPI ? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI est conçu pour vous permettre de mesurer les performances des programmes du haut de l’entonnoir jusqu’à leur impact sur les recettes. Si vous n’utilisez pas les opportunités, vous pourrez toujours :

* Affichez les performances de vos programmes de formation pour l’engagement du public.
* Affichez les performances de vos programmes d’acquisition de prospects.
* Affichez les performances des campagnes multicanal à l’aide des balises de programme.
* Consultez les tendances d’engagement des audiences des 12 derniers mois.
* Enregistrer et exporter les données de performances dans PowerPoint.

## Puis-je mesurer le succès des stratégies basées sur les comptes dans MPI ? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Oui. MPI s&#39;intègre à [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) pour extraire les listes de comptes ABM dans MPI de manière transparente. Vous pouvez utiliser le filtre Liste des comptes ABM pour choisir la liste ABM souhaitée en fonction de laquelle filtrer les données.

## L’attribution est-elle disponible instantanément lorsque j’achète MPI ? {#is-attribution-instantly-available-when-i-purchase-mpi}

Les fonctionnalités d’attribution de Marketo sont disponibles pour nos clients lorsqu’ils achètent MPI. Toutefois, [une configuration appropriée](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) est nécessaire pour garantir que les opportunités et les données de programme sont correctement transmises à MPI.

## Que dois-je faire pour configurer l’attribution ? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuration de l’opportunité

   1. Assurez-vous que les opportunités sont synchronisées avec votre CRM
   1. Si vos paramètres d’attribution sont définis sur Explicite, assurez-vous que les rôles de contact sur les opportunités sont renseignés
   1. Nous vous recommandons de définir le paramètre d’attribution sur Hybride
   1. Configuration du programme

      1. Inclure le coût du programme dans vos programmes
      1. Examinez le comportement des analyses pour indiquer si un programme doit être inclus dans les analyses
      1. Définissez les critères de réussite pour chaque canal que vous possédez
      1. Lier la personne aux programmes

         1. Assurez-vous que le Programme d’acquisition et la Date d’acquisition ont été définis pour chaque personne de votre base de données afin que l’attribution du premier contact fonctionne.
         1. Assurez-vous que vos programmes définissent des états de succès pour les personnes de votre base de données

>[!TIP]
>
>Toutes les étapes de configuration requises sont décrites dans [cet article](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Quelle est la différence entre MPI et l&#39;analyseur de programmes ? {#whats-the-difference-between-mpi-and-the-program-analyzer}

L’analyseur de programmes vous permet de comparer vos programmes sur un maximum de quatre mesures. MPI vous permet d’analyser la contribution de votre canal et de votre programme par rapport à une mesure choisie telle que le succès, les nouvelles opportunités créées, etc. Il vous permet également d’afficher la tendance du canal sur 12 mois en fonction d’une mesure spécifique que vous avez choisie.

## Quelle est la différence entre MPI et le Report Builder avancé ? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Le Report Builder avancé (parfois appelé RCE) est conçu pour le reporting en libre-service (ou ad hoc), généralement effectué par les opérations marketing. L’API est conçue pour permettre aux responsables marketing et aux marketeurs d’accéder en un clic à l’analyse des performances. Une configuration minimale est requise.

## Qu’est-il advenu de l’option « Année précédente » dans le filtre de date de la contribution ? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Nous avons temporairement supprimé la sélection « Année précédente ». Vous avez toujours la possibilité d’afficher les données de performances de l’année entière à l’aide de la sélection de Période personnalisée .
