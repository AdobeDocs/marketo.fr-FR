---
unique-page-id: 12983291
description: Fuseau horaire du Destinataire - Documents marketing - Documentation du produit
title: Présentation du fuseau horaire Destinataire
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Présentation du fuseau horaire du Destinataire {#understanding-recipient-time-zone}

Les programmes de messagerie et d’engagement peuvent être configurés pour être distribués selon les fuseaux horaires des destinataires, ce qui évite d’avoir à créer plusieurs programmes : envoyer une fois et Marketo conserve automatiquement le courriel jusqu’à l’heure locale correcte.

>[!NOTE]
>
>Le fuseau horaire du destinataire fonctionne actuellement **uniquement** avec le contenu du courrier électronique. Elle ne fonctionnera pas pour les programmes d’engagement par défaut.

## Programmes de courriel {#email-programs}

Il existe deux scénarios Principaux lorsque [planifie un programme de courriel](schedule-email-programs-with-recipient-time-zone.md) :

1. Planification de l’exécution du programme au cours des 25 prochaines heures.
1. Planification de l’exécution du programme de plus de 25 heures à l’avenir (c.-à-d. la semaine prochaine).

Afin de prendre en compte chaque fuseau horaire, les programmes électroniques planifiés avec le début de fuseau horaire Destinataire s’exécutant à minuit dans le fuseau horaire **premier/premier** du monde (UTC +14:00).

## Programmes d’engagement {#engagement-programs}

Lorsque vous [planifiez un flux de programme d’engagement](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) et que le fuseau horaire du Destinataire est principal, la diffusion du programme s’début à minuit en UTC +14:00. Nous vous demandons de programmer la première diffusion au moins 25 heures dans le futur (24 heures + un certain temps pour lancer la campagne) parce que les gens peuvent être admissibles à la diffusion dans chaque fuseau horaire à travers le monde. En commençant le traitement à cette heure en UTC +14:00 nous garantissons que nous livrerons le courriel à la date et à l&#39;heure prévues pour chaque personne admissible à cette distribution.

## Calcul du fuseau horaire {#calculating-time-zone}

Marketo calcule le fuseau horaire en fonction de la ville, de l’état, du pays ou du code postal d’une personne. Si nous ne parvenons pas à calculer le fuseau horaire d’une personne à partir de ces valeurs, nous retournons à nos champs Ville déduite, État déduit, Pays déduit et Code postal déduit.

Dans les cas où nous avons **only **Country ou **only** State available :

* Pour les pays avec trois fuseaux horaires ou moins, nous sélectionnons le fuseau horaire moyen.
* Pour les états avec deux fuseaux horaires, nous sélectionnons le premier des deux.

Si nous ne parvenons toujours pas à déterminer le fuseau horaire d’une personne à partir de n’importe quelle combinaison de ces champs, nous n’affecterons **pas** un fuseau horaire et le courrier électronique sera distribué en fonction de votre fuseau horaire de l’abonnement de marketing. Ainsi, si votre programme est prévu pour 9 h 00 HAP, les personnes qui n&#39;ont pas de fuseau horaire assigné recevront le courriel à 9 h 00 HAP.

>[!NOTE]
>
>Marketo recalcule automatiquement le fuseau horaire d’une personne lorsque l’un des champs d’entrée ci-dessus change.

>[!MORELIKETHIS]
>
>* [Planification des Programmes de courriel avec fuseau horaire Destinataire](schedule-email-programs-with-recipient-time-zone.md)
>* [Début principal pour les Programmes électroniques](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [Planification des Programmes d’engagement avec fuseau horaire Destinataire](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

>



