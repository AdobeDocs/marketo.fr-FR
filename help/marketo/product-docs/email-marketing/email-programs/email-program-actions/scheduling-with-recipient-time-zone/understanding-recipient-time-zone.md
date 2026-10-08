---
unique-page-id: 12983291
description: Découvrez la planification du fuseau horaire du destinataire pour les programmes de messagerie. Diffuser des e-mails au même moment local pour chaque destinataire.
title: Présentation du fuseau horaire du destinataire
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
TQID: 'https://experienceleague.adobe.com/KAj3dO4Md7Zel5SqR4m2OrTjp93ZD735gNWWRinNV5k'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: c0f0afc1-a5a8-4b01-8b43-cc38f9169499
    internal-label: Email programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 2%
---
# Présentation du fuseau horaire du destinataire {#understanding-recipient-time-zone}

Les programmes d’e-mail et d’engagement peuvent être configurés pour diffuser en fonction des fuseaux horaires des destinataires, ce qui élimine la nécessité de créer plusieurs programmes, à envoyer une seule fois, et Marketo retient automatiquement l’e-mail jusqu’à l’heure locale appropriée.

>[!NOTE]
>
>[!UICONTROL Fuseau horaire du destinataire] fonctionne actuellement **uniquement** avec le contenu des e-mails. Cela ne fonctionne pas pour les programmes d’engagement par défaut.

## Programmes d’e-mail {#email-programs}

Il existe deux scénarios principaux lors de la [planification d’un programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) :

1. Planification de l’exécution du programme au cours des 25 prochaines heures.
1. Planification de l’exécution du programme à plus de 25 heures dans le futur (c’est-à-dire la semaine prochaine).

Pour s’adapter à chaque fuseau horaire, les programmes d’e-mail planifiés avec [!UICONTROL Fuseau horaire du destinataire] commencent à fonctionner à minuit dans le **premier/premier** fuseau horaire au monde (UTC +14:00).

## Programmes d’engagement {#engagement-programs}

Lorsque vous [planifiez un flux de programme d’engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) et que le [!UICONTROL fuseau horaire du destinataire] est actif, le cast du programme commence à fonctionner à minuit en UTC +14:00. Nous exigeons que vous planifiiez le premier casting au moins 25 heures à l&#39;avenir (24 heures + un peu de temps pour démarrer la campagne) parce que les gens peuvent se qualifier pour le cast dans tous les fuseaux horaires à travers le monde. Le fait de commencer le traitement à cette heure au format UTC +14:00 garantit que l’e-mail est envoyé à la date et à l’heure planifiées pour chaque personne éligible à ce cast.

## Calcul du fuseau horaire {#calculating-time-zone}

Marketo calcule le fuseau horaire en fonction de la ville, de l’état, du pays ou du code postal d’une personne. Si nous ne parvenons pas à calculer le fuseau horaire d’une personne à partir de ces valeurs, nous revenons à nos champs Ville déduite, État déduit, Pays déduit et Code postal déduit .

Dans les cas où nous avons **uniquement** Pays ou **uniquement** État disponible :

* Pour les pays disposant de trois fuseaux horaires ou moins, nous sélectionnons le fuseau horaire intermédiaire.
* Pour les états comportant deux fuseaux horaires, nous sélectionnons le premier des deux.

Si nous ne parvenons toujours pas à déterminer le fuseau horaire d’une personne à partir de n’importe quelle combinaison de ces champs, nous n’attribuerons **pas** de fuseau horaire et l’e-mail sera envoyé en fonction du fuseau horaire de votre abonnement à Marketo. Ainsi, si votre programme est planifié à 9 h 00 PDT, les personnes sans fuseau horaire affecté recevront l’e-mail à 9 h 00 PDT.

>[!NOTE]
>
>Marketo recalcule automatiquement le fuseau horaire d’une personne lorsque l’un des champs de saisie ci-dessus change.

>[!MORELIKETHIS]
>
>* [Planification de programmes de messagerie avec [!UICONTROL fuseau horaire du destinataire]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Prise en main des programmes de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Planification des programmes d’engagement avec [!UICONTROL Fuseau horaire du destinataire]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
