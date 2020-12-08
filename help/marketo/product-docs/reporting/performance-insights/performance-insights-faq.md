---
unique-page-id: 12979858
description: FAQ sur les statistiques de performances - Documents marketing - Documentation sur les produits
title: FAQ sur les statistiques de performances
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---


# FAQ sur les statistiques de performances {#performance-insights-faq}

## Quelle est la définition de &quot;réussite&quot; dans l’onglet Engagement ? {#what-is-the-definition-of-success-in-the-engagement-tab}

Le succès est une mesure de l&#39;interaction significative dans Marketo. Le but d&#39;un programme est de créer une interaction significative avec la personne ou la prospect. Le succès est marqué lorsqu’une personne atteint l’état qui lui permet d’atteindre cet objectif. Il peut s’agir de participer à un webinaire, de cliquer sur un lien dans un courriel ou de remplir un formulaire Web. Le succès varie en fonction du canal du programme.

>[!NOTE]
>
>**Exemple**
>
>Dans un programme de webinaire, il peut y avoir plusieurs états, tels que : Invité, enregistré et assisté. Invité ou Inscrit ne sont pas des interactions significatives parce que les gens ne regardent pas vraiment le webinaire. Participé est considéré comme un succès dans ce cas.

## Est-ce que MPI fonctionnera avec n&#39;importe quel CRM ? {#will-mpi-work-with-any-crm}

Oui. Techniquement, MPI n’interagit pas directement avec la gestion de la relation client pour la synchronisation des données. MPI utilise les données stockées dans le Data Warehouse Analytics de Marketing Cloud. Puisque la synchronisation CRM se produit dans l’application Gestion des pistes, toute gestion de la relation client prise en charge par Marketing intégrée à l’application Gestion des pistes affichera correctement les données. Toutefois, les champs d’opportunité CRM doivent être correctement mappés aux champs d’opportunité Marketo.

## Je n’ai aucun autre produit Marketing Analytics (ARB, RCE, RCA, Programme Analyse). Est-ce que MPI va fonctionner pour moi ? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI est un module complémentaire indépendant de l&#39;application Gestion des pistes. Il ne nécessite pas l’utilisation d’autres produits d’analyse.

## RCA me montre également les données de performances du programme. Existe-t-il une différence entre les données affichées dans MPI et RCA ? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Non. MPI crée des données à partir du même entrepôt de données que RCA. Par conséquent, vous ne verrez aucune différence de données entre les deux. RCA vous permet de créer vos propres rapports à la volée. MPI vous donne accès à des tableaux de bord visuels faciles à comprendre.

## Je ne veux pas que certains de mes programmes (p. ex. Opérationnels) s’affichent dans MPI. Comment contrôler la visibilité de certains programmes ? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Vous pouvez contrôler la visibilité de vos programmes en définissant le comportement Analytics de vos programmes sur Opérationnel. Le programme sera ainsi exclu des calculs d’analyse.

>[!NOTE]
>
>En savoir plus sur la définition du comportement des analyses [ici](http://docs.marketo.com/display/public/DOCS/Edit+Analytics+Behavior+Settings).

## J’exécute une campagne multi-canal pour le lancement d’un nouveau produit. Comment puis-je vue les performances de cette campagne sur tous les différents canaux au même endroit ? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Nous vous recommandons d’utiliser des balises de programme pour les programmes d’une telle campagne. Les balises de programme sont automatiquement synchronisées avec MPI et vous pouvez les filtrer dans tous les tableaux de bord MPI pour vue les performances de vos campagnes à canaux multiples.

## Ai-je accès aux paramètres d’attribution si je n’ai pas de RCA ? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Vous avez accès aux paramètres d’attribution si vous disposez d’une MPI, que vous possédiez ou non une RCA.

## Je reçois une alerte dans MPI lorsque je me connecte pour me signaler que mes paramètres d’attribution sont incorrects. Qu&#39;est-ce qui ne va pas ? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI calcule si toutes vos opportunités sont incluses ou non dans les analyses. Sinon, vous serez invité à modifier vos paramètres d’attribution (explicite, implicite, hybride) afin d’inclure davantage d’opportunités.

Il se peut également que vous manquiez des opportunités en raison du manque de coûts de Programme dans vos programmes. Veuillez vérifier le comportement Analytics de vos programmes. Ils peuvent être :

1. Par défaut : le comportement par défaut est que le programme est inclus dans MPI uniquement s&#39;il y a au moins un coût de période, même si un coût nul est affecté.
1. Inclusif : cette option garantit que le programme est disponible dans MPI, que vous ayez inclus ou non un coût de période.
1. [Opérationnel](http://docs.marketo.com/display/DOCS/Best+Practice%3A+How+to+Organize+your+Programs#BestPractice:HowtoOrganizeyourPrograms-OperationalPrograms) : cette option a pour effet que le programme ne s’affiche pas dans MPI.

>[!NOTE]
>
>Le coût de la période **doit** être configuré pour le rapports Réussite et Noms dans le tableau de bord d’engagement. Ce tableau de bord utilise les données de coût de période pour les réussites des agrégats et les nouveaux noms. Si le coût de la période n’est pas configuré, le tableau de bord d’engagement ne génère pas de rapports corrects, quels que soient les paramètres de comportement d’Analytics ci-dessus.

## Pourquoi manque-t-il certaines opportunités dans MPI ? {#why-am-i-missing-some-opportunities-in-mpi}

Deux raisons clés peuvent vous empêcher de saisir des opportunités dans MPI :

1. Le paramètre d’attribution est défini sur Explicite mais les rôles de contact ne sont pas affectés aux opportunités
1. Le coût de la période n&#39;est pas inclus dans vos programmes

MPI calcule si toutes vos opportunités sont incluses ou non dans les analyses. Sinon, vous serez invité à modifier vos paramètres d’attribution (explicite, implicite, hybride) afin d’inclure davantage d’opportunités.

Il se peut également que vous manquiez des opportunités en raison du manque de coûts de Programme dans vos programmes. L&#39;alerte apparaîtra mais ne vous indique pas quels programmes manquent de coûts. Veuillez consulter la configuration de votre programme pour y inclure les coûts, afin de vous assurer que tous vos programmes et opportunités sont inclus dans MPI.

## Pourquoi ne vois-je pas les champs personnalisés, le type d’opportunité et les filtres ABM sur le tableau de bord d’engagement ? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Les champs personnalisés, le type d&#39;opportunité et les Filtres ABM sont tous des attributs liés à une opportunité. Le tableau de bord d’engagement vous permet de mesurer votre engagement et votre acquisition de pistes, qu’ils soient ou non associés à une opportunité. Comme le tableau de bord d&#39;engagement ne tient pas compte des opportunités, les champs personnalisés, le type d&#39;opportunité et les Filtres ABM ne s&#39;appliquent pas.

## Je souhaite utiliser un champ Opportunité Salesforce personnalisé pour le rapports des recettes au lieu du champ Montant opportunité Salesforce standard. Est-ce que MPI me permettra de faire ça ? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Oui. [L&#39;assistance](http://docs.marketo.com/cdn-cgi/l/email-protection#b5c6c0c5c5dac7c1f5d8d4c7ded0c1da9bd6dad8) marketing peut faire correspondre le champ Montant de l&#39;opportunité du marketing à un champ Opportunité Salesforce personnalisé tant que le type de champ est devise. Puisque MPI pointe vers le champ Montant de l&#39;opportunité marketing, MPI peut utiliser les données du champ Salesforce personnalisé mappé.

>[!NOTE]
>
>Une fois le mappage effectué, MPI affiche les données en cours. Le montant historique ne sera pas modifié.

## Si je n’utilise pas les opportunités, puis-je toujours utiliser MPI ? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI est conçu pour vous permettre de mesurer les performances du programme du haut de l&#39;entonnoir jusqu&#39;à l&#39;impact sur les recettes. Si vous n&#39;utilisez pas les opportunités, vous pourrez toujours :

* Performances de vue de vos programmes d&#39;alimentation pour l&#39;engagement audience.
* Performances vues de vos programmes d&#39;acquisition de pistes.
* Performances vues des campagnes à canaux multiples par le biais de balises de programme.
* Voir les tendances de l’engagement des audiences au cours des 12 derniers mois.
* Enregistrez et exportez les données de performances dans PowerPoint.

## Puis-je mesurer le succès des stratégies basées sur les comptes dans MPI ? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Oui. MPI s&#39;intègre à [Marketo ABM](http://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) pour extraire en toute transparence les listes de compte ABM dans MPI. Vous pouvez utiliser le filtre Liste de compte ABM pour choisir la liste ABM de votre choix pour filtrer les données selon.

## L’attribution est-elle instantanément disponible lorsque j’achète MPI ? {#is-attribution-instantly-available-when-i-purchase-mpi}

Les fonctionnalités d’attribution du marketing sont disponibles pour nos clients lorsqu’ils achètent des MPI. Toutefois, une configuration [](http://docs.marketo.com/x/mRPG) adéquate est nécessaire pour s’assurer que les opportunités et les données de programme se déplacent correctement dans les MPI.

## Que dois-je faire pour configurer l’attribution ? {#what-do-i-have-to-do-to-set-up-attribution}

1. Configuration de l&#39;opportunité

   1. Vérifier que les opportunités sont synchronisées avec votre gestion de la relation client
   1. Si les paramètres d’attribution sont définis sur Explicite, assurez-vous que les rôles de contact sur les opportunités sont renseignés.
   1. Nous vous recommandons de remplacer le paramètre Attribution par Hybrid.
   1. Configuration du programme

      1. Inclure le coût du programme dans vos programmes
      1. Examiner le comportement des analyses pour indiquer si un programme doit être inclus dans les analyses
      1. Définissez les critères de réussite pour chaque canal que vous avez
      1. Lier la personne aux Programmes

         1. Assurez-vous que le Programme d’acquisition et la date d’acquisition ont été définis pour chaque personne de votre base de données afin que l’attribution Première touche fonctionne.
         1. Vérifier que vos programmes définissent les états de réussite des personnes de votre base de données

>[!TIP]
>
>Toutes les étapes de configuration requises sont détaillées dans [cet article](http://docs.marketo.com/x/mRPG).

## Quelle est la différence entre MPI et l’analyseur de Programme ? {#whats-the-difference-between-mpi-and-the-program-analyzer}

L’analyseur de Programme vous permet de comparer vos programmes selon quatre mesures au maximum. MPI vous permet d&#39;analyser votre contribution canal et programme à une mesure choisie, telle que Réussite, Nouvelles opportunités créées, etc. Il vous permet également de vue de la tendance des canaux de 12 mois en fonction d’une mesure spécifique que vous avez choisie.

## Quelle est la différence entre MPI et le Report Builder avancé ? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Le Report Builder avancé (parfois appelé RCE) est conçu pour le rapports libre-service (ou ad hoc), généralement effectué par les opérations marketing. MPI est conçu pour permettre aux responsables marketing et aux marketeurs d’accéder en un clic à l’analyse des performances. Une configuration minimale est requise.

## Qu’est-il advenu de l’option &quot;Année précédente&quot; dans le filtre de dates des contributions ? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Nous avons temporairement supprimé la sélection &quot;Année précédente&quot;. Vous avez toujours la possibilité d’afficher les données de performances de l’année entière à l’aide de la sélection Période personnalisée.
