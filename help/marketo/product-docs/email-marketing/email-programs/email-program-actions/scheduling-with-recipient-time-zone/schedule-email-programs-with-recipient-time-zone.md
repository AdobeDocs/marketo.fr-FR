---
unique-page-id: 12982903
description: Planification de programmes de messagerie avec fuseau horaire du destinataire - Documents Marketo - Documentation du produit
title: Planification de programmes de messagerie électronique avec fuseau horaire du destinataire
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Planification de programmes de messagerie électronique avec fuseau horaire du destinataire {#schedule-email-programs-with-recipient-time-zone}

Deux scénarios sont possibles lors de la planification d’un programme de messagerie lorsque le fuseau horaire du destinataire est activé :

1. Planification de l’exécution du programme **dans** les 25 heures suivantes
1. Planification de l’exécution du programme **plus** 25 heures à l’avenir (c’est-à-dire la semaine prochaine)

## Scénario 1 : Dans Les 25 Heures {#scenario-within-hours}

Supposons que vous approuviez un programme d’e-mail avec le fuseau horaire du destinataire activé et une heure de diffusion planifiée dans les 25 heures qui suivent. Il se peut que des personnes de votre liste dynamique vivent dans des fuseaux horaires où l’heure planifiée est déjà passée.

Dans ce scénario, nous vous permettons de décider de ce qu’il convient de faire avec ce sous-ensemble de personnes qualifiées. Cliquez sur l’icône d’engrenage en regard de **[!UICONTROL Fuseau horaire du destinataire]** dans la mosaïque **[!UICONTROL Planifier]** du programme de messagerie.

![](assets/image2017-12-5-10-3a46-3a42.png)

Vous disposez ainsi de deux options :

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Définition**
>
>* **[!UICONTROL Envoyez le jour suivant dans le fuseau horaire du destinataire]** : si l’envoi de l’e-mail est prévu pour mardi à 9 heures:00am, les personnes qualifiées qui vivent dans des fuseaux horaires où l’heure prévue est déjà passée recevront l’e-mail le *mercredi* à 9 heures:00am.
>
>* **[!UICONTROL Envoyez l’e-mail en utilisant l’heure définie par défaut du programme]** : si l’envoi de l’e-mail est prévu pour mardi à 9 heures:00am, les personnes qualifiées qui vivent dans des fuseaux horaires où l’heure planifiée est déjà passée recevront l’e-mail *en fonction des paramètres de fuseau horaire de votre abonnement*. Ainsi, si les paramètres de votre [fuseau horaire d&#39;abonnement](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) sont définis sur PDT Amérique/Los Angeles, ces destinataires recevront toujours l&#39;email le mardi à 9:00am PDT (quelle que soit l&#39;heure qui se trouve dans leur propre fuseau horaire).

>[!NOTE]
>
>[En savoir plus](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) sur la manière dont Marketo calcule les fuseaux horaires pour les destinataires.

Examinons ce scénario plus en détail. Supposons que vous soyez à San Francisco et que vous planifiez un e-mail à 7 :00am pour un envoi de 9 **:00am**. Dans votre liste dynamique, il y a des personnes des régions suivantes :

* San Francisco
* Texas
* New York
* Italie

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00am est déjà passé à New York et en Italie, donc les personnes qualifiées dans ces deux fuseaux horaires recevront l&#39;email en fonction des **Paramètres de fuseau horaire** :

* **[!UICONTROL Diffusez le jour suivant dans le fuseau horaire du destinataire]:** mercredi à 9:00am dans ses fuseaux horaires respectifs, **OU**

* **[!UICONTROL Livrer en utilisant l&#39;heure par défaut du programme]** : mardi à 9:00am PDT (New York - 12:00pm EDT et Italie - 6:00pm CET).

Une fois que vous avez approuvé votre programme, il commence à s’exécuter dans les 15 minutes.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Bien que le programme lance le *processus* d’envoi d’e-mails dans 15 minutes, les e-mails ne seront pas *envoyés* à ce moment-là. Les destinataires recevront toujours des e-mails en fonction des **[!UICONTROL paramètres de fuseau horaire]** de votre choix.

## Scénario 2 : plus de 25 heures {#scenario-more-than-hours}

Dans ce deuxième scénario, vous approuvez un programme d’e-mail dont le **[!UICONTROL fuseau horaire du destinataire]** est activé et dont l’heure de diffusion planifiée remonte à plus de 25 heures. Dans ce cas, le programme commencera à fonctionner à l’heure planifiée dans le fuseau horaire **le plus proche** au monde (UTC + 14:00). Il peut y avoir des personnes qui remplissent les critères de votre liste dynamique dans tous les fuseaux horaires à travers le monde, donc commencer dans le premier fuseau horaire nous permet de diffuser l’e-mail à la date/heure planifiée à tous les destinataires dans leurs fuseaux horaires respectifs.

**Démarrage rapide**

Maintenant, parlons de la façon dont [[!UICONTROL Head Start]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) fonctionne avec **[!UICONTROL Recipient Time Zone]**. Notre fonctionnalité Bon départ exige que le programme soit planifié au moins 12 heures à l&#39;avance. Qu’est-ce que cela signifie pour le fuseau horaire du destinataire ? Rappelez-vous que lorsque le fuseau horaire du destinataire est activé, nous commençons à exécuter le programme d’e-mail à l’heure planifiée dans le premier fuseau horaire (UTC +14:00). Ainsi, pour activer **à la fois** le démarrage rapide et le fuseau horaire du destinataire, les programmes d’e-mail doivent être planifiés **au moins 12 heures en avance sur l’heure planifiée au format UTC +14:00.**

Cela signifie que si vous êtes en Amérique/Los Angeles et que vous souhaitez activer les fuseaux horaires Head Start et Recipient, vous devez planifier le programme **34 heures** à l&#39;avance. Comment en sommes-nous arrivés à ce chiffre ?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

En résumé, les programmes d’e-mail planifiés avec le fuseau horaire du destinataire doivent commencer à s’exécuter à l’heure planifiée dans le fuseau horaire le plus proche (c’est-à-dire là où il atteint minuit en premier) afin de s’adapter à chaque fuseau horaire. Donc, si vous planifiez un programme de messagerie...

* **avec un délai de livraison *dans les* 25 heures**, le programme commence à fonctionner dans les 15 minutes. Les destinataires qui ont déjà dépassé l’heure planifiée recevront l’e-mail en fonction des paramètres de fuseau horaire que vous avez choisis.
* **avec un délai de livraison *supérieur à 25 heures*** le programme commence à s’exécuter à l’heure planifiée dans le fuseau horaire le plus proche (UTC +14:00).
* **avec Head Start**, le programme commence à traiter 12 heures avant l’heure planifiée dans le fuseau horaire le plus proche (UTC +14:00).

>[!CAUTION]
>
>Toute personne qui se désabonne entre le moment où vous commencez l’envoi de votre e-mail et celui où il est réellement envoyé recevra toujours l’e-mail. Nous vous recommandons d’ajuster votre notification de désabonnement pour tenir compte du fait que le traitement des désabonnements peut prendre entre 1 et 2 jours ouvrables.

>[!MORELIKETHIS]
>
>* [Présentation du fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Prise en main des programmes de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Abandonner la diffusion des programmes de messagerie programmés avec le fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
