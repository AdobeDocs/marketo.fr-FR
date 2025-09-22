---
unique-page-id: 10100257
description: FAQ sur les informations d’e-mail - Documents Marketo - Documentation du produit
title: Questions fréquentes sur Email Insights
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 1%

---

# Questions fréquentes sur Email Insights {#email-insights-faq}

## Existe-t-il des différences entre les mesures de ratio avec [!UICONTROL Informations sur les e-mails] et d’autres rapports sur les e-mails Marketo ? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Oui. [!UICONTROL  Insights sur les e-mails ] met en corrélation les mesures d’engagement avec leurs mesures de diffusion correspondantes pour le même e-mail envoyé lors du calcul des ratios de mesures d’engagement (taux d’ouverture, taux de clic-ouverture, taux de désabonnement). Par exemple, dans [!UICONTROL Informations sur les e-mails], lorsque vous examiniez un graphique de série temporelle au cours de la semaine écoulée avec des répartitions quotidiennes du taux de clic sur ouverture, nous affichons désormais le véritable ratio corrélé d’événements d’ouverture/clic/désabonnement en fonction des mesures de diffusion correspondantes. Cela contraste avec le comportement de l’Explorateur de revenus, qui résume tout simplement. [!UICONTROL Informations sur les e-mails] offre une vue plus précise des taux d’engagement.

## Pourquoi la fonction [!UICONTROL Insights sur les e-mails] ne prend-elle en charge que 10 dimensions personnalisées ? {#why-does-email-insights-only-support-custom-dimensions}

Pour de nombreux cas d’utilisation, l’extension des dimensions système par défaut avec 10 dimensions personnalisées supplémentaires est plus qu’adéquate et inclut des dimensions personnalisées basées sur des segmentations ou des balises de programme. À l’avenir, nous prévoyons d’autoriser les clients à augmenter le nombre de dimensions personnalisées autorisées.

## Pourquoi ne puis-je pas réutiliser les emplacements de dimensions personnalisées après leur attribution ? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Une fois qu’un emplacement de Dimension personnalisé donné a été alloué, un remappage entraînerait le déclenchement d’une erreur par les données précédentes lorsqu’elles sont fusionnées avec une nouvelle signification. Pour cette raison, les emplacements de Dimension personnalisés ne peuvent pas être réutilisés. Ce comportement est cohérent avec celui d’autres outils d’analyse des mesures, tels que Google Analytics.

## La fonction [!UICONTROL Informations sur les e-mails] prend-elle en charge les e-mails Marketo Sales Insight ? {#does-email-insights-support-marketo-sales-insight-emails}

Oui. Tous les e-mails envoyés via les Statistiques de vente Marketo sont inclus dans [!UICONTROL Informations sur les e-mails].

## Les [!UICONTROL informations sur les e-mails] prennent-elles en charge les e-mails opérationnels ? {#does-email-insights-support-operational-emails}

Oui. Par défaut, les e-mails opérationnels sont masqués lors de la consultation et de l’interrogation. Vous pouvez toutefois modifier ce paramètre dans le panneau Paramètres personnels.

## Les [!UICONTROL Insights d’e-mail] capturent-ils les étapes de flux d’e-mail de Campaign récurrentes planifiées ou réexécutées ? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Oui et Non. Avec la version initiale de [!UICONTROL Insights sur les e-mails], tous les événements d’e-mail sont capturés et accessibles pour toute campagne intelligente récurrente planifiée ou réexécutée. Mais vous ne pourrez pas faire de distinction entre les différentes exécutions de cette campagne intelligente. Nous ajoutons la prise en charge dans notre prochaine version pour capturer les informations d’exécution de campagne intelligente pour les événements Ouvrir, Cliquer et Désabonner afin de différencier.

## Pourquoi de nombreuses mesures indiquent-elles zéro lorsque je filtre par type d’appareil ou système d’exploitation d’appareil ? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

À l’exception des mesures Taux de clic sur ouverture, Ouvertures, Clics et Désabonnements, toutes les autres mesures prises en charge sont des événements de diffusion ou des ratios dérivés d’événements de diffusion. Étant donné que le type d’appareil et le système d’exploitation de l’appareil s’appliquent uniquement aux mesures Engagement , nous ne disposons tout simplement pas des informations à afficher. Par exemple, il s’agit d’une requête non définie visant à demander le taux de diffusion lorsqu’elle est filtrée par type d’appareil = mobile, car Marketo n’aurait reçu aucune mesure d’engagement pour les événements de diffusion et d’envoi sous-jacents. Nous étudions les moyens d’appliquer le type d’appareil et le système d’exploitation de l’appareil à partir des mesures d’engagement pour les ratios composés des mesures d’engagement et de diffusion.

## Que fait [!UICONTROL Informations sur les e-mails] lorsque certains clients de messagerie bloquent les images ? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Un problème courant du secteur est le nombre croissant de clients de messagerie qui désactivent les images par défaut. Le chargement des images est la base de l’enregistrement des ouvertures. Il est tout à fait possible qu’un utilisateur reçoive un e-mail avec des images bloquées, mais avec le texte et les liens entièrement lisibles. Si un utilisateur ou une utilisatrice fait l’expérience de cette manipulation et clique sur un lien de cet e-mail, vous vous retrouvez avec un scénario d’événement de clic, mais sans événement d’ouverture correspondant pour cet e-mail. Les Insights sur les e-mails de Marketo génèrent automatiquement les événements manquants. La logique est identique à celle de Marketo pour le rapport Performance des e-mails, ainsi que pour la zone Analyse des e-mails dans l’explorateur de revenus.
