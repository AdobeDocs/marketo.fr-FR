---
description: Webinaires à la demande - Documents Marketo - Documentation du produit
title: Webinaires On-Demand
feature: Interactive Webinars
source-git-commit: c3819373fbd49f7ea67f6eb6661d63ad5ba86d57
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Webinaires On-Demand {#on-demand-webinars}

Les webinaires à la demande capturent et affinent les pistes enregistrées pour votre événement et qui n’y ont pas assisté, mais souhaitent obtenir des informations relatives à l’événement en regardant l’enregistrement. Des informations telles que le nom, l’ID de courrier électronique et la date/durée de contrôle peuvent être capturées dans Marketo Engage et utilisées pour cibler ces pistes sans affichage.

L’URL de jointure du webinaire qui a été partagée avec les inscrits avant l’événement peut être utilisée pour regarder l’enregistrement à la demande. Une fois qu’un inscrit qui n’a pas assisté à l’événement en direct (par exemple, un prospect dont le statut de programme est &quot;Non-affichage&quot;), clique sur l’URL de jointure du webinaire, l’état du programme de cette piste passe de &quot;Pas de programme&quot; à &quot;Participé à la demande&quot;. L’état du programme des responsables ayant visionné l’événement en direct et ayant le statut &quot;Participé&quot; ne serait pas affecté s’ils décidaient de visiter l’URL de jointure et de regarder l’enregistrement à la demande.

Adobe Connect, la technologie qui alimente les webinaires interactifs, effectue le suivi de la visite, ainsi que de la durée de la montre relative aux pistes qui regardent l’enregistrement, et rapporte les informations à Marketo quotidiennement. L’enregistrement est disponible à l’adresse URL de jointure pendant 30 jours après l’événement. La durée ne peut pas être modifiée.

Marketo fournit les statistiques de surveillance pour les webinaires à la demande sur l’onglet Tableau de bord à l’aide des widgets suivants :

* Résumé à la demande : indique le nombre de visiteurs (Aucun affichage) qui regardent l’enregistrement après l’événement un ou plusieurs jours donnés.

* Statistiques On-Demand : ce widget fournit des informations sur :
   * Jours pendant lesquels l’enregistrement à la demande est disponible pour affichage : aide les marketeurs à effectuer des actions, telles que l’exécution des campagnes par e-mail vers la fin de la durée d’enregistrement de disponibilité de 30 jours.
   * Nombre total de visiteurs pour les webinaires à la demande à ce jour : nombre de tous les inscrits sans affichage qui ont consulté l’enregistrement à la demande à ce jour.
   * Durée moyenne de visionnage en minutes pour tous les visiteurs : donne aux marketeurs une idée de la quantité d’enregistrement visualisée et des campagnes intelligentes pouvant être utilisées pour cibler les pistes au-dessus d’une certaine durée de visionnage.

![](assets/on-demand-webinars-1.png)

Les filtres et déclencheurs des webinaires interactifs ont été modifiés pour prendre en charge les webinaires à la demande. Le déclencheur &quot;Assiste à l’événement&quot; et le filtre &quot;A assisté à l’événement&quot; sont ajoutés avec une contrainte supplémentaire (&quot;Mode événement&quot;), où un marketeur peut choisir si la cible est une audience en ligne ou une audience à la demande. Si la contrainte &quot;Mode événement&quot; n’est pas sélectionnée, les audiences On-Demand et On-Demand sont ciblées. D’autres contraintes, telles que &quot;Date de contrôle&quot; et &quot;Durée de contrôle&quot;, peuvent être utilisées avec le mode d’événement &quot;On-Demand&quot;. Le filtre d’inactivité &quot;N’a pas assisté à un événement&quot; peut également être utilisé pour les webinaires à la demande avec le mode d’événement &quot;On-Demand&quot;.
