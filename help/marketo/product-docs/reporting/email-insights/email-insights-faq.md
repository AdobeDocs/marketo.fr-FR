---
unique-page-id: 10100257
description: FAQ sur les statistiques par e-mail - Documentation Marketo - Documentation du produit
title: FAQ sur les statistiques sur les emails
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# FAQ sur les statistiques sur les emails {#email-insights-faq}

## Existe-t-il des différences entre les mesures de ratio avec les statistiques sur les courriers électroniques et d’autres rapports Marketo Email ? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Oui. Insights établit une corrélation entre les mesures d’engagement et les mesures de diffusion correspondantes pour le même email envoyé lors du calcul des ratios d’engagement (Taux d’ouverture, Taux de clics jusqu’à l’ouverture, Taux de désabonnement). Par exemple, dans la section Informations sur les emails, lorsque vous observez un graphique de série temporelle de la semaine dernière avec des ventilations quotidiennes du taux de clic pour ouverture, nous affichons désormais le ratio réel d’événements d’ouverture/clic/désabonnement en fonction des mesures de diffusion correspondantes. Ceci contraste avec le comportement de l’Explorateur de recettes, qui résume simplement tout. Informations sur les emails présente une vue plus précise des taux d’engagement.

## Pourquoi la fonction Email Insights ne prend-elle en charge que 10 Dimensions personnalisées ? {#why-does-email-insights-only-support-custom-dimensions}

Pour de nombreux cas d’utilisation, l’extension des dimensions système par défaut avec 10 dimensions personnalisées supplémentaires sera plus qu’appropriée et inclut des dimensions personnalisées basées sur des segments ou des balises de programme. À l’avenir, nous prévoyons de permettre aux clients d’augmenter le nombre de Dimensions personnalisées autorisées.

## Pourquoi ne puis-je pas réutiliser les emplacements de Dimensions personnalisées une fois qu’ils ont été attribués ? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Une fois qu’un emplacement de Dimension personnalisée donné a été attribué, le fait de le remapper provoquerait une erreur lors de la fusion avec une nouvelle signification pour les données précédentes. Pour cette raison, les emplacements de Dimension personnalisés ne peuvent pas être réutilisés. Ce comportement est cohérent avec celui d’autres outils d’analyse des mesures, tels que les Google Analytics.

## Les informations sur les courriers électroniques prennent-elles en charge les courriers électroniques de Marketo Sales Insight ? {#does-email-insights-support-marketo-sales-insight-emails}

Oui. Tous les emails envoyés par le biais de Marketo Sales Insights sont inclus dans Email Insights.

## Les informations sur les courriers électroniques prennent-elles en charge les courriers électroniques opérationnels ? {#does-email-insights-support-operational-emails}

Oui. Par défaut, les emails opérationnels sont masqués pour être vus et interrogés. Vous pouvez toutefois modifier ce paramètre dans le panneau Paramètres personnels .

## Les statistiques sur les emails capturent-elles les étapes de flux d’emails planifiées de manière récurrente ou exécutent-elles à nouveau la campagne dynamique ? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Oui et non. Avec la version initiale d’Email Insights, tous les événements de courrier électronique sont capturés et accessibles pour toute campagne dynamique planifiée récurrente ou réexécutée. Mais vous ne pourrez pas distinguer les différentes exécutions de cette campagne dynamique. Nous ajoutons la prise en charge dans notre prochaine version pour capturer les informations d’exécution Smart Campaign pour les événements Open, Click et Unsubscribe afin de différencier les événements.

## Pourquoi de nombreuses mesures affichent-elles zéro lorsque je filtre par type d’appareil ou système d’exploitation d’appareil ? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

À l’exception des mesures Taux de clics jusqu’à l’ouverture, Ouvertures, Clics et Désabonnements, toutes les autres mesures prises en charge sont des événements de diffusion ou des rapports dérivés d’événements de diffusion. Puisque Type de périphérique et Système d’exploitation du périphérique s’appliquent uniquement aux mesures d’engagement, nous ne disposons tout simplement pas des informations à afficher. Par exemple, il s’agit d’une requête non définie qui demande le taux de diffusion lorsqu’il est filtré par Type de périphérique = mobile, puisque Marketo n’aurait reçu aucune mesure d’engagement pour les événements de diffusion et d’envoi sous-jacents. Nous explorons les moyens d’appliquer le type de périphérique et le système d’exploitation du périphérique à partir des mesures Engagement pour les ratios, qui comprennent à la fois les mesures Engagement et Diffusion.

## Que fait la fonction Email Insights lorsque certains clients de messagerie bloquent les images ? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problème courant du secteur est qu’un nombre croissant de clients de messagerie désactivent les images par défaut. Le chargement d’images est la base de l’enregistrement des ouvertures. Il est tout à fait possible qu&#39;un utilisateur puisse recevoir un email avec des images bloquées, mais avec le texte et les liens entièrement lisibles. Si un utilisateur a fait l’expérience de cela et cliqué sur un lien dans ce courrier électronique, vous obtenez un scénario d’événement Click , mais aucun événement Open correspondant pour ce courrier électronique. Marketo Email Insights génère automatiquement les événements manquants. La logique est identique à la manière dont Marketo effectue cette opération pour le rapport Performance des emails , ainsi que pour la zone Analyse des emails dans l’Explorateur de recettes.
