---
unique-page-id: 12983291
description: Présentation du fuseau horaire du destinataire - Documents Marketo - Documentation du produit
title: Comprendre le fuseau horaire du destinataire
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Comprendre le fuseau horaire du destinataire {#understanding-recipient-time-zone}

Les programmes de messagerie et d’engagement peuvent être configurés pour être diffusés en fonction des fuseaux horaires des destinataires, éliminant ainsi la nécessité de créer plusieurs programmes (envoyer une fois) et Marketo conserve automatiquement l’email jusqu’à l’heure locale correcte.

>[!NOTE]
>
>Le fuseau horaire du destinataire fonctionne actuellement **uniquement** avec le contenu de l’email. Cela ne fonctionnera pas pour les programmes d’engagement par défaut.

## Programmes d&#39;e-mail {#email-programs}

Il existe deux scénarios principaux lors de la [planification d’un programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) :

1. Planification de l’exécution du programme dans les 25 prochaines heures.
1. Planification de l’exécution du programme de plus de 25 heures à l’avenir (c’est-à-dire la semaine prochaine).

Afin de s&#39;adapter à chaque fuseau horaire, les programmes de messagerie planifiés avec fuseau horaire du destinataire commencent à s&#39;exécuter à minuit dans le fuseau horaire du **premier/premier** dans le monde (UTC +14:00).

## Programmes d&#39;engagement {#engagement-programs}

Lorsque vous [planifiez un flux de programme d’engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) et que le Fuseau horaire des destinataires est actif, la diffusion du programme commencera à s’exécuter à minuit au format UTC +14:00. Nous vous demandons de planifier la première diffusion d’au moins 25 heures à l’avenir (24 heures + un peu de temps pour lancer la campagne), car les participants peuvent être éligibles à chaque fuseau horaire à travers le monde. Le démarrage du traitement à cette heure en UTC +14:00 garantit que nous enverrons l&#39;email à la date et à l&#39;heure prévues pour chaque personne admissible à cette diffusion.

## Calcul du fuseau horaire {#calculating-time-zone}

Marketo calcule le fuseau horaire en fonction de la ville, de l’état, du pays ou du code postal d’une personne. Si nous ne parvenons pas à calculer le fuseau horaire d’une personne à partir de ces valeurs, nous restaurons à nos champs Ville déduite, État déduit, Pays déduit et Code postal déduit.

Dans les cas où nous avons **only** Country ou **only** State disponible :

* Pour les pays ayant trois fuseaux horaires ou moins, nous sélectionnons le fuseau horaire du milieu.
* Pour les états avec deux fuseaux horaires, nous sélectionnons le fuseau horaire précédent des deux.

Si nous ne parvenons toujours pas à déterminer le fuseau horaire d’une personne à partir d’une combinaison de ces champs, nous **et non** attribuerons un fuseau horaire et l’email sera envoyé en fonction de votre fuseau horaire d’abonnement Marketo. Ainsi, si votre programme est programmé pour 9 h 00 heure d&#39;été du Pacifique, les personnes n&#39;ayant aucun fuseau horaire attribué recevront l&#39;email à 9 h 00 heure d&#39;été du Pacifique.

>[!NOTE]
>
>Marketo recalcule automatiquement le fuseau horaire d’une personne lorsque l’un des champs de saisie ci-dessus change.

>[!MORELIKETHIS]
>
>* [Planification de programmes de messagerie avec fuseau horaire de destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start for Email Programmes](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Planification des programmes d’engagement avec fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
