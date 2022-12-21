---
unique-page-id: 12983291
description: Présentation du fuseau horaire du destinataire - Documents Marketo - Documentation du produit
title: Comprendre le fuseau horaire du destinataire
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# Comprendre le fuseau horaire du destinataire {#understanding-recipient-time-zone}

Les programmes de messagerie et d’engagement peuvent être configurés pour être diffusés en fonction des fuseaux horaires des destinataires, éliminant ainsi la nécessité de créer plusieurs programmes (envoyer une fois) et Marketo conserve automatiquement l’email jusqu’à l’heure locale correcte.

>[!NOTE]
>
>Le fuseau horaire des destinataires fonctionne actuellement. **only** avec le contenu de l’email. Cela ne fonctionnera pas pour les programmes d’engagement par défaut.

## Programmes d&#39;e-mail {#email-programs}

Il existe deux scénarios Principaux lorsque [planification d’un programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Planification de l’exécution du programme dans les 25 prochaines heures.
1. Planification de l’exécution du programme de plus de 25 heures à l’avenir (c’est-à-dire la semaine prochaine).

Afin de s’adapter à chaque fuseau horaire, les programmes de messagerie planifiés avec le fuseau horaire du destinataire commencent à s’exécuter à minuit dans la variable **first/premiers** fuseau horaire mondial (UTC +14:00).

## Programmes d&#39;engagement {#engagement-programs}

Lorsque vous [planification d’un flux de programme d’engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) et que le fuseau horaire du destinataire est principal, la diffusion du programme commencera à fonctionner à minuit au format UTC +14:00. Nous vous demandons de planifier la première diffusion d’au moins 25 heures à l’avenir (24 heures + un peu de temps pour lancer la campagne), car les participants peuvent être éligibles à chaque fuseau horaire à travers le monde. Le démarrage du traitement à cette heure en UTC +14:00 garantit que nous enverrons l&#39;email à la date et à l&#39;heure prévues pour chaque personne admissible à cette diffusion.

## Calcul du fuseau horaire {#calculating-time-zone}

Marketo calcule le fuseau horaire en fonction de la ville, de l’état, du pays ou du code postal d’une personne. Si nous ne parvenons pas à calculer le fuseau horaire d’une personne à partir de ces valeurs, nous restaurons à nos champs Ville déduite, État déduit, Pays déduit et Code postal déduit.

Dans les cas où **only** Pays ou **only** État disponible :

* Pour les pays ayant trois fuseaux horaires ou moins, nous sélectionnons le fuseau horaire du milieu.
* Pour les états avec deux fuseaux horaires, nous sélectionnons le fuseau horaire précédent des deux.

Si nous ne parvenons toujours pas à déterminer le fuseau horaire d’une personne à partir d’une combinaison de ces champs, nous **not** attribuez un fuseau horaire et l’email sera envoyé en fonction du fuseau horaire d’abonnement à Marketo. Ainsi, si votre programme est programmé pour 9 h 00 heure d&#39;été du Pacifique, les personnes n&#39;ayant aucun fuseau horaire attribué recevront l&#39;email à 9 h 00 heure d&#39;été du Pacifique.

>[!NOTE]
>
>Marketo recalcule automatiquement le fuseau horaire d’une personne lorsque l’un des champs de saisie ci-dessus change.

>[!MORELIKETHIS]
>
>* [Planification des programmes de messagerie avec un fuseau horaire de destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Prise en main des programmes de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Planification des programmes d’engagement avec fuseau horaire des destinataires](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

