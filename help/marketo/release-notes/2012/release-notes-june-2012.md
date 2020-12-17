---
unique-page-id: 2951114
description: Notes de mise à jour - Juin 2012 - Documentation sur le marketing - Documentation du produit
title: Notes de mise à jour - Juin 2012
translation-type: tm+mt
source-git-commit: 48330e8f6f1ad8883d74d80e6f64faba4fdfa52e
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---


# Notes de mise à jour : Juin 2012 {#release-notes-june}

>[!NOTE]
>
>**Plongée profonde**
>
>Pour les autres versions, consultez les [Notes de mise à jour](http://docs.marketo.com/display/docs/release+notes) plongée en profondeur.

## Améliorations de la gestion des pistes marketing {#marketo-lead-management-enhancements}

### Renommer {#rename}

Vous pouvez renommer vos Listes dynamiques, vos listes statiques et vos campagnes. Si vous utilisez ces ressources dans des filtres, des triggers ou des flux, le nom y sera automatiquement mis à jour. Vous avez toujours été en mesure de renommer vos courriels, formulaires et dossiers.

Et, en bonus, nous avons amélioré la saisie et l&#39;affichage du texte de description des actifs.

![](assets/image2014-9-23-10-3a23-3a10.png)

## Mappage des champs d’importation {#import-field-mapping}

Nous avons rendu l&#39;importation d&#39;une liste dans Marketo beaucoup plus facile ! Au cours du processus d’importation, vous pouvez associer le nom du champ Marketo au nom de l’en-tête de colonne dans le fichier d’importation. En outre, dans Admin, vous pouvez configurer des noms d’alias associés au nom du champ dans Marketing Cloud, afin que vos utilisateurs sélectionnent le champ approprié à chaque fois.

Au fur et à mesure que vous continuez à importer et à mapper des champs, Marketo se souviendra et affichera les mappages pendant l’importation, pour une utilisation aisée. Et pour simplifier la vie, vous pouvez cliquer sur l’en-tête Valeur d’exemple pour afficher les différentes valeurs qui seront renseignées dans le champ. Cela vous permet de faire correspondre le bon champ à chaque fois !

![](assets/image2014-9-23-10-3a23-3a27.png)

## Page de résumé des Listes dynamiques et des Listes statiques {#summary-page-for-smart-lists-and-static-lists}

Vous êtes-vous déjà demandé où vos listes sont utilisées ? Ou qui a créé la liste, ou l&#39;a modifiée pour la dernière fois ? La nouvelle page de résumé disponible sur les Listes dynamiques et les listes statiques vous fournira ces informations importantes.

![](assets/image2014-9-23-10-3a23-3a40.png)

Sur les pages de Programme et de résumé de Campaign existantes, nous avons ajouté les informations Date/Utilisateur créé et Date/Utilisateur Dernière modification ainsi que les informations sur Utilisateur !

![](assets/image2014-9-23-10-3a23-3a54.png)

## Utilisé par pour les ressources {#used-by-for-assets}

Nous avons ajouté un nouvel onglet à nos pages de résumé des ressources, appelé Utilisé par !

![](assets/image2014-9-23-10-3a24-3a5.png)

Exemple : Utilisé par pour les Listes statiques

## Quadrillage du landing page {#landing-page-gridlines}

L’ajout de quadrillage de landing page facilite considérablement l’alignement du texte, des graphiques et des formulaires sur votre landing page. Activez-la et désactivez-la pour un landing page donné, et ajustez également la largeur entre les lignes !

![](assets/image2014-9-23-10-3a24-3a19.png)

![](assets/image2014-9-23-10-3a24-3a33.png)

## Pistes bloquées à partir de messages {#leads-blocked-from-mailings}

Lors de la planification d&#39;une campagne, vous pouvez cliquer sur le lien pour voir la liste des pistes bloquées de votre publipostage.

![](assets/image2014-9-23-10-3a24-3a51.png)

## Étape d&#39;attente - Jeton de piste et jeton Mon {#wait-step-lead-token-and-my-token}

Dans notre version de mai, nous avons ajouté des options avancées à l’étape de flux d’attente. Ces modifications vous permettent de spécifier un jour ouvré, une date et une heure. Dans cette version, nous avons ajouté la possibilité d’utiliser un jeton lors de l’étape d’attente. Par exemple, vous pouvez utiliser `{{lead.Birthday}}` pour envoyer un courriel le jour de l’anniversaire ou `{{my.Event Date}}` pour envoyer un dernier rappel de webinaire.

![](assets/image2014-9-23-10-3a25-3a57.png)

## Vue de miniatures dans Design Studio {#view-as-thumbnails-in-design-studio}

Basculez votre vue d’une liste d’images vers une vue de miniature !

![](assets/image2014-9-23-10-3a26-3a13.png)

Remarque : A compter de cette version, le tri précédent sur les grilles de listes dynamiques ne s’appliquera pas à la prochaine liste intelligente que vous vue. Par exemple, si vous triez une liste intelligente par nom de Société, nous ne trierons pas automatiquement la prochaine liste intelligente vue par ce même champ.

Rappel : Mise à niveau du rapport de performances du courriel en cours !

## Améliorations des analyses du cycle des recettes marketing {#marketo-revenue-cycle-analytics-enhancements}

### Nouvelles mesures dans l&#39;Analyse d&#39;opportunités de Programme {#new-metrics-in-program-opportunity-analysis}

Vous pouvez maintenant obtenir des informations sur le nombre moyen de touches marketing avant la création ou la fermeture d’opportunités, ainsi que sur la valeur moyenne d’une touche marketing.

![](assets/image2014-9-23-10-3a26-3a30.png)

![](assets/image2014-9-23-10-3a26-3a41.png)

## Affichage de plusieurs graphiques {#displaying-multi-charts}

La fonction multigraphique vous permet d’afficher plusieurs graphiques dans un seul rapport de l’explorateur de cycles de recettes. Vous pouvez, par exemple, utiliser cette fonction lorsque vous souhaitez afficher les mêmes données sur plusieurs mois. Cette fonctionnalité vous évite également d’avoir à créer des filtres et des rapports distincts.

![](assets/image2014-9-23-10-3a27-3a41.png)

## Type de graphique à grille thermique {#heat-grid-chart-type}

Les grilles thermiques vous permettent de visualiser les données afin que vous puissiez identifier les schémas des performances marketing. Ce type de visualisation permet de coder en couleur vos résultats afin que vous puissiez vue à une analyse professionnelle complexe dans une visualisation facile à comprendre.

![](assets/image2014-9-23-10-3a28-3a21.png)

## Type de graphique de dispersion {#scatter-chart-type}

Les graphiques de dispersion vous aident à visualiser les données sur plusieurs dimensions dans un même graphique. Ce type de visualisation trace une bulle sur un graphique en fonction des attributs utilisés. Vous pouvez ensuite utiliser une mesure pour coder par couleur la bulle et/ou utiliser une mesure pour spécifier la taille de la bulle.

![](assets/image2014-9-23-10-3a29-3a7.png)
