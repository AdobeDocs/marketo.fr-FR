---
unique-page-id: 12982903
description: Planification de programmes de messagerie avec Fuseau horaire du destinataire - Documents Marketo - Documentation du produit
title: Planification des programmes de messagerie avec un fuseau horaire de destinataire
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Planification des programmes de messagerie avec un fuseau horaire de destinataire {#schedule-email-programs-with-recipient-time-zone}

Il existe deux scénarios potentiels lors de la planification d’un programme de messagerie lorsque le fuseau horaire du destinataire est activé :

1. Planification de l’exécution du programme **dans les 25 heures suivantes**
1. Planification de l’exécution du programme **plus** que 25 heures dans le futur (c’est-à-dire la semaine prochaine)

## Scénario 1 : dans les 25 heures {#scenario-within-hours}

Supposons que vous approuviez un programme de messagerie avec le fuseau horaire du destinataire activé et une heure de remise planifiée dans les 25 heures suivantes. Vous pouvez avoir des personnes dans votre liste dynamique qui vivent dans des fuseaux horaires où l’heure planifiée est déjà dépassée.

Dans ce scénario, nous vous permettons de décider quoi faire de ce sous-ensemble de personnes qualifiées. Cliquez sur l’icône d’engrenage en regard de **Fuseau horaire du destinataire** dans la mosaïque **Planning** du programme de messagerie.

![](assets/image2017-12-5-10-3a46-3a42.png)

Vous disposez ainsi de deux options :

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Définition**
>
>* **Livrez le jour suivant dans le fuseau horaire du destinataire** : si l&#39;envoi de l&#39;email est programmé le mardi à 9 h 00, les personnes qualifiées qui vivent dans les fuseaux horaires où l&#39;heure planifiée est déjà passée recevront l&#39;email le *mercredi* à 9 h 00.
>
>* **Diffuser selon l&#39;heure par défaut du programme** : si l&#39;envoi de l&#39;email est programmé le mardi à 9h00, les personnes qualifiées qui vivent dans des fuseaux horaires où l&#39;heure planifiée est déjà passée recevront l&#39;email _en fonction des paramètres de fuseau horaire de votre abonnement_. Ainsi, si vos [ paramètres de fuseau horaire d&#39;abonnement ](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) sont définis sur PDT America/Los Angeles, ces destinataires recevront toujours l&#39;email le mardi à 9 h 00 heure d&#39;été (quelle que soit l&#39;heure de leur propre fuseau horaire).

>[!NOTE]
>
>[En savoir plus](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) sur la façon dont Marketo calcule les fuseaux horaires pour les destinataires.

Examinons ce scénario plus en détail. Supposons que vous soyez à San Francisco, en programmant un email à 7 h 00 pour un **9h00** envoi. Dans votre liste dynamique, il existe des personnes issues des régions suivantes :

* San Francisco
* Texas
* New York
* Italie

![](assets/image2017-12-6-10-3a52-3a41.png)

9 h 00 est déjà passé à New York et en Italie. Les personnes qualifiées dans ces deux fuseaux horaires recevront l’email en fonction des **Paramètres du fuseau horaire** :

* **Diffusez le jour suivant dans le fuseau horaire du destinataire :** mercredi à 9h00 dans leurs fuseaux horaires respectifs, **OR**

* **Diffuser en utilisant l’heure par défaut du programme** : mardi à 9 h 00 heure d’été (New York - 12 h HNE et Italie - 18 h CET).

Une fois votre programme validé, il démarre dans les 15 minutes.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Bien que le programme démarre le _processus_ d&#39;envoi des emails dans 15 minutes, les emails ne seront pas _diffusés_ à ce moment-là. Les destinataires recevront toujours des e-mails en fonction des **paramètres de fuseau horaire** que vous choisissez.

## Scénario 2 : plus de 25 heures {#scenario-more-than-hours}

Dans ce second scénario, vous approuvez un programme de messagerie avec l’activation de **Fuseau horaire du destinataire** et une heure de remise planifiée de plus de 25 heures à l’avenir. Dans ce cas, le programme démarrera à l’heure planifiée dans le fuseau horaire **au plus tôt** du monde (UTC + 14:00). Il peut y avoir des personnes qui remplissent les critères de votre liste dynamique dans chaque fuseau horaire à travers le monde. Par conséquent, le fait de commencer dans le fuseau horaire le plus ancien nous permet de diffuser l’email à la date/heure planifiée à tous les destinataires dans leurs fuseaux horaires respectifs.

**Head Start**

Maintenant, parlons du fonctionnement de [Head Start](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) avec **Recipient Time Zone**. Pour utiliser la fonctionnalité de prise en main existante, le programme doit être programmé au moins 12 heures à l’avance. Qu’est-ce que cela signifie pour le fuseau horaire des destinataires ? Souvenez-vous que lorsque le fuseau horaire des destinataires est activé, le programme de messagerie commence à être exécuté à l’heure planifiée dans le fuseau horaire le plus ancien (UTC +14:00). Par conséquent, pour activer les programmes **Head Start et Recipient Time Fuseau, les programmes de messagerie doivent être programmés** au moins 12 heures avant l&#39;heure planifiée à UTC +14:00.****

Cela signifie que si vous êtes aux États-Unis/à Los Angeles et que vous souhaitez activer Head Start et Recipient Time Zone, vous devez planifier le programme **34 heures** à l&#39;avance. Comment en sommes-nous arrivés à ce nombre ?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

En résumé, les programmes de messagerie planifiés avec le fuseau horaire du destinataire doivent commencer à s’exécuter à l’heure planifiée dans le fuseau horaire le plus ancien (c’est-à-dire, où il atteint minuit en premier) afin de s’adapter à chaque fuseau horaire. Donc, si vous programmez un programme d&#39;email...

* **avec un délai de remise _dans les_ 25 heures**, le programme commence à fonctionner dans les 15 minutes. Les destinataires qui ont déjà dépassé l&#39;heure planifiée recevront l&#39;email en fonction des paramètres de fuseau horaire que vous avez choisis.
* **avec une heure de remise _supérieure_ à 25 heures dans le futur**, le programme commence à s&#39;exécuter à l&#39;heure planifiée dans le fuseau horaire le plus ancien (UTC +14:00).
* **avec Head Start**, le programme commence à traiter 12 heures avant l’heure planifiée dans le fuseau horaire le plus ancien (UTC +14:00).

>[!CAUTION]
>
>Quiconque se désabonne entre le moment où vous commencez votre envoi d’email et celui où il est réellement remis recevra toujours l’email. Nous vous recommandons d’ajuster votre notification de désabonnement pour tenir compte du fait que le traitement des désabonnements peut prendre entre 1 et 2 jours ouvrables.

>[!MORELIKETHIS]
>
>* [Comprendre le fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Head Start for Email Programmes](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Abandonner la diffusion des programmes de messagerie planifiés avec le fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
