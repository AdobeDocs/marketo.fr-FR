---
description: Webinaires À La Demande - Documents Marketo - Documentation Du Produit
title: Webinaires à la demande
feature: Interactive Webinars
exl-id: 65bfc1d2-6382-4cfa-9560-69cbb0c37c42
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Webinaires à la demande {#on-demand-webinars}

Les webinaires à la demande capturent et affinent les leads qui se sont inscrits à votre événement et qui n’y ont pas assisté, mais qui souhaitent obtenir des informations relatives à l’événement en regardant l’enregistrement. Des informations telles que le nom, l’ID d’e-mail et la date/durée de l’observation peuvent être capturées dans Marketo Engage et utilisées pour cibler ces prospects.

L’URL de jointure du webinaire qui a été partagée avec les personnes inscrites avant l’événement peut être utilisée pour regarder l’enregistrement à la demande. Une fois qu’un inscrit qui n’a pas assisté à l’événement en direct (par exemple, un prospect dont le statut de programme est « Pas affiché ») clique sur l’URL de participation au webinaire, le statut de programme de ce prospect passe de « Pas affiché » à « Participé à la demande ». Le statut du programme des prospects qui ont regardé l’événement en direct et qui ont le statut « Participé » ne sera pas affecté s’ils décident de consulter l’URL d’inscription et de regarder l’enregistrement à la demande.

Adobe Connect, la technologie qui alimente les webinaires interactifs, effectue le suivi de la visite ainsi que de la durée de visionnage des leads qui regardent l’enregistrement, et transmet les informations à Marketo Engage quotidiennement. Le suivi des webinaires à la demande s’arrête 30 jours après l’événement. La durée ne peut pas être modifiée.

Marketo Engage fournit les statistiques de surveillance des webinaires à la demande dans l’onglet Tableau de bord à l’aide des widgets suivants :

* Résumé à la demande : fournit un résumé du nombre de visiteurs (sans affichage) qui regardent l’enregistrement après l’événement un jour donné

* Statistiques à la demande : ce widget fournit des informations sur les éléments suivants :
   * Nombre de jours pendant lesquels l&#39;enregistrement à la demande peut être consulté : permet aux spécialistes du marketing d&#39;effectuer des actions, telles que l&#39;exécution de campagnes par e-mail, vers la fin de la durée de disponibilité d&#39;enregistrement de 30 jours.
   * Nombre total de visiteurs pour les webinaires à la demande à ce jour : nombre de tous les inscrits qui n’ont pas assisté à l’enregistrement à la demande à ce jour.
   * Durée moyenne de visionnage en minutes pour tous les visiteurs : donne aux marketeurs une idée de la quantité d’enregistrement visionné et des campagnes intelligentes qui peuvent être utilisées pour cibler les prospects au-dessus d’une certaine durée de visionnage.

![](assets/on-demand-webinars-1.png)

>[!NOTE]
>
>Les vues ne sont comptabilisées que lorsque la durée de la montre dépasse une minute.

Les filtres et les déclencheurs des webinaires interactifs ont été modifiés pour répondre aux webinaires à la demande. Le déclencheur « Assiste à l’événement » et le filtre « A assisté à l’événement » sont ajoutés avec une contrainte supplémentaire (« Mode d’événement »), où un spécialiste marketing peut choisir si la cible est l’audience en direct ou l’audience à la demande. Si la contrainte « Mode événement » n’est pas sélectionnée, les audiences En direct et À la demande sont ciblées. D’autres contraintes telles que « Date de surveillance » et « Durée de surveillance » peuvent être utilisées avec le mode d’événement « À la demande ». Le filtre d’inactivité « N’a pas assisté à un événement » peut également être utilisé pour les webinaires à la demande avec le mode d’événement « À la demande ».
