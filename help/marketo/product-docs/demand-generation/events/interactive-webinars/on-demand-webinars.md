---
description: Webinaires à la demande - Documents Marketo - Documentation du produit
title: Webinaires On-Demand
hide: true
hidefromtoc: true
feature: Interactive Webinars
source-git-commit: 49a75b6aef25787a68554dff3a847279ef8ba12a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Webinaires On-Demand {#on-demand-webinars}

Les webinaires à la demande capturent et affinent les pistes enregistrées pour votre événement et qui n’y ont pas assisté, mais souhaitent obtenir des informations relatives à l’événement en regardant l’enregistrement. Des informations telles que le nom, l’ID de message électronique et la date/durée de contrôle peuvent être capturées en Marketo Engage et utilisées pour cibler ces pistes sans affichage.

L’URL de jointure du webinaire qui a été partagée avec les inscrits avant l’événement peut être utilisée comme lien pour regarder l’enregistrement à la demande. Une fois qu’un inscrit, qui n’a pas assisté à l’événement en direct, c’est-à-dire un prospect dont le statut de programme est &quot;Pas de programme&quot;, clique sur l’URL de jointure du webinaire, l’état du programme d’un tel prospect passe de &quot;Pas de programme&quot; à &quot;Participé à la demande&quot;. Notez que l’état du programme des prospects qui ont visionné l’événement en direct et dont le statut est &quot;Participé&quot; ne serait pas affecté même s’ils consultent l’URL de jointure et regardent l’enregistrement à la demande.

Adobe Connect, la technologie qui alimente les webinaires interactifs, effectue le suivi de la visite et de la durée de visionnage des pistes qui ont consulté l’enregistrement et qui signalent les mêmes informations quotidiennement à Marketo. L’enregistrement est disponible à l’adresse URL de jointure pendant une durée de 30 jours après l’événement et la durée est fixe.

Marketo fournit les statistiques de surveillance pour les webinaires à la demande dans l’onglet Tableau de bord à l’aide des deux widgets suivants :
1. Résumé à la demande : il s’agit d’un résumé quotidien du nombre de visiteurs (Aucun affichage) ayant visionné l’enregistrement après l’événement.
2. Statistiques On-Demand : ces widgets fournissent des informations sur : a. Jours pendant lesquels l’enregistrement On-Demand est disponible pour affichage. Cela peut aider les marketeurs à prendre des mesures telles que l’exécution de campagnes par e-mail plus près de la fin de la durée de disponibilité de l’enregistrement de 30 jours.
b. Nombre total de visiteurs pour les webinaires à la demande jusqu’à ce jour. Il s’agit du décompte de tous les inscrits sans programme qui ont regardé l’enregistrement à la demande jusqu’à la date.
c. Durée moyenne de la montre en minutes pour tous les visiteurs. Cela permet au marketeur de savoir quelle partie de l’enregistrement est visionnée et quelles campagnes intelligentes peuvent être utilisées pour cibler les pistes au-dessus d’une certaine durée de visionnage.

CAPTURE D’ÉCRAN

Les filtres et déclencheurs des webinaires interactifs ont été modifiés pour prendre en charge les webinaires à la demande. Le déclencheur &quot;Assiste à l’événement&quot; et le filtre &quot;A assisté à l’événement&quot; sont ajoutés avec une contrainte supplémentaire &quot;Mode événement&quot; où un marketeur peut choisir si la cible est une audience en direct ou une audience à la demande. Si la contrainte &quot;Mode événement&quot; n’est pas sélectionnée, les audiences On-Demand et On-Demand sont ciblées. D’autres contraintes telles que &quot;Date de contrôle&quot; et &quot;Durée de contrôle&quot; peuvent être utilisées avec le mode d’événement &quot;On-Demand&quot;. Le filtre d’inactivité &quot;N’a pas assisté à un événement&quot; peut également être utilisé pour les webinaires à la demande avec le mode d’événement &quot;On-Demand&quot;.
