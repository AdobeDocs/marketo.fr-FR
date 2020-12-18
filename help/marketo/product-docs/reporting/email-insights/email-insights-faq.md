---
unique-page-id: 10100257
description: FAQ sur les connaissances par courriel - Documentation sur le marketing - Documentation sur le produit
title: FAQ sur les statistiques d'e-mail
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# FAQ sur les connaissances par courriel {#email-insights-faq}

## Existe-t-il des différences entre les mesures de ratio avec les statistiques d’e-mail et d’autres rapports de messagerie de Marketo ? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Oui. Les statistiques par courriel corrélent les mesures d’engagement avec leurs mesures de diffusion correspondantes pour le même courrier électronique envoyé lors du calcul des ratios d’engagement (Taux d’ouverture, Taux de clics jusqu’à l’ouverture, Taux de désabonnement). Par exemple, dans les statistiques par courriel, lorsque vous observez un graphique de séries chronologiques de la semaine écoulée avec des ventilations quotidiennes du taux de clics à ouverture, nous présentons maintenant le rapport réel corrélé des événements d’ouverture/clic/désabonnement en fonction des mesures de diffusion correspondantes. Ceci contraste avec le comportement de l&#39;Explorateur de recettes, qui résume tout simplement. Les statistiques par courriel présentent une vue plus précise des taux d’engagement.

## Pourquoi Email Insights ne prend-il en charge que 10 Dimensions personnalisées ? {#why-does-email-insights-only-support-custom-dimensions}

Pour de nombreux cas d’utilisation, l’extension des dimensions système par défaut avec 10 dimensions personnalisées supplémentaires sera plus qu’adéquate et inclut des dimensions personnalisées basées sur des segments ou des balises de Programme. A l’avenir, nous prévoyons de permettre aux clients d’augmenter le nombre de Dimensions personnalisées autorisées.

## Pourquoi ne puis-je pas réutiliser les emplacements de Dimensions personnalisées après leur attribution ? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Une fois qu’un emplacement de Dimension personnalisée donné a été attribué, le remappage entraîne une erreur des données précédentes lorsqu’elles sont fusionnées avec une nouvelle signification. De ce fait, il est possible que les emplacements de Dimension personnalisés ne soient pas réutilisés. Ce comportement est cohérent avec celui d’autres outils d’analyse des mesures, tels que les Google Analytics.

## Est-ce que les statistiques par courriel prennent en charge les courriels de Marketing-to Sales Insight ? {#does-email-insights-support-marketo-sales-insight-emails}

Oui. Tous les courriels envoyés par l&#39;intermédiaire des statistiques commerciales de Marketo sont inclus dans les statistiques par courriel.

## Est-ce que Email Insights prend en charge les courriels opérationnels ? {#does-email-insights-support-operational-emails}

Oui. Par défaut, les courriers électroniques opérationnels sont masqués de la vue et de l’interrogation. Vous pouvez toutefois modifier ce paramètre dans le panneau Paramètres personnels.

## Est-ce que les statistiques de messagerie capturent les étapes de flux de courrier électronique Smart Campaign planifiées ou réexécutées de manière récurrente ? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Oui et Non. Avec la première version de Email Insights, tous les événements de messagerie électronique sont capturés et accessibles pour tout Campaign récurrent planifié ou réexécuté. Mais vous ne serez pas capable de différencier les différentes exécutions de cette Campaign Intelligente. Dans notre prochaine version, nous ajouterons la prise en charge de la capture des informations d’exécution de Smart Campaign pour les événements Ouvrir, Cliquer et Désabonner afin de différencier les données.

## Pourquoi de nombreuses mesures affichent-elles zéro lorsque je filtre par type de périphérique ou système d’exploitation de périphérique ? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

À l’exception des mesures de taux de clics à l’ouverture, d’ouvertures, de clics et de désabonnements, toutes les autres mesures prises en charge sont des événements de diffusion ou des ratios dérivés de événements de diffusion. Puisque le type de périphérique et le système d’exploitation du périphérique ne s’appliquent qu’aux mesures Engagement, nous ne disposons simplement pas des informations à afficher. Par exemple, il s’agit d’une requête non définie de demander le taux de Diffusion lorsqu’il est filtré par Type de périphérique = mobile, puisque Marketo n’aurait reçu aucune mesure Engagement pour les événements de Diffusion sous-jacents et Envoyé. Nous étudions les moyens d&#39;appliquer le type de périphérique et le système d&#39;exploitation du périphérique à partir des mesures Engagement pour les ratios comprenant à la fois les mesures Engagement et Diffusion.

## Que fait Email Insights lorsque certains clients de messagerie bloquent les images ? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problème courant du secteur est que de plus en plus de clients de messagerie désactivent les images par défaut. Le chargement des images est la base de l’enregistrement des ouvertures. Il est tout à fait possible qu&#39;un utilisateur reçoive un e-mail avec des images bloquées, mais avec le texte et les liens entièrement lisibles. Si un utilisateur a fait l’expérience de ce problème et cliqué sur un lien dans ce courrier électronique, vous obtenez un scénario de événement de clics, mais aucun événement d’ouverture correspondant pour ce courrier électronique. Les statistiques d’e-mail marketing généreront automatiquement les événements manquants. La logique est identique à la manière dont Marketo effectue cette opération pour le rapport Performances du courriel, ainsi que pour la zone Analyse du courriel dans l’Explorateur de recettes.
