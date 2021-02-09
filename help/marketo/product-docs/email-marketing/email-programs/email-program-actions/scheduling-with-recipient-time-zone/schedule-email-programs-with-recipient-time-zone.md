---
unique-page-id: 12982903
description: Planification des Programmes de courriel avec fuseau horaire Destinataire - Documentation sur le marketing - Documentation du produit
title: Planification des Programmes de courriel avec fuseau horaire Destinataire
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---


# Planification des Programmes de courriel avec le fuseau horaire Destinataire {#schedule-email-programs-with-recipient-time-zone}

Il existe deux scénarios possibles lors de la planification d’un programme de courriel lorsque le fuseau horaire du Destinataire est activé :

1. Planification de l&#39;exécution du programme **dans** les 25 heures suivantes
1. Planification de l&#39;exécution du programme **plus** de 25 heures dans le futur (c&#39;est-à-dire la semaine prochaine)

## Scénario 1 : Dans les 25 heures {#scenario-within-hours}

Supposons que vous approuviez un programme de courriel avec le fuseau horaire du Destinataire activé et une heure de remise planifiée dans les 25 prochaines heures. Il se peut que des personnes de votre liste intelligente vivent dans des fuseaux horaires dont l’heure planifiée est déjà dépassée.

Dans ce scénario, nous vous permettons de décider quoi faire avec ce sous-ensemble de personnes qualifiées. Cliquez sur l’icône d’engrenage en regard de **Fuseau horaire du Destinataire** dans la mosaïque **Planification** du programme électronique.

![](assets/image2017-12-5-10-3a46-3a42.png)

Vous disposez ainsi de deux options :

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Définition**
>
>* **Effectuez le lendemain dans le fuseau horaire** du destinataire : si l&#39;e-mail doit sortir le mardi à 9 h 00, les personnes qualifiées qui vivent dans des fuseaux horaires dont l&#39;heure est déjà passée recevront l&#39;e-mail le  ** mercredi à 9 h 00.
   >
   >
* **Diffusez à l’aide de l’heure** par défaut du programme : si le courrier électronique doit sortir le mardi à 9 h 00, les personnes qualifiées qui vivent dans des fuseaux horaires dont l’heure planifiée est déjà passée recevront le courrier électronique  _en fonction des paramètres_ de fuseau horaire de votre abonnement. Ainsi, si vos [paramètres de fuseau horaire de l&#39;abonnement](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) sont définis sur PDT America/Los Angeles, ces destinataires recevront toujours le courriel mardi à 9 h (quelle que soit l&#39;heure de leur fuseau horaire).


>[!NOTE]
>
>[Découvrez ](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) comment Marketo calcule les fuseaux horaires pour les destinataires.

Examinons ce scénario plus en détail. Supposons que vous soyez à San Francisco et que vous planifiez un courriel à 7h00 pour un **9h00** envoi. Dans votre liste intelligente, il y a des personnes des régions suivantes :

* San Francisco
* Texas
* New York
* Italie

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00 am est déjà passé à New York et en Italie, donc les personnes qualifiées dans ces deux fuseaux horaires recevront l&#39;e-mail en fonction des **Paramètres du fuseau horaire** :

* **Livrer le lendemain dans le fuseau horaire du destinataire :** mercredi à 9 h 00 dans leur fuseau horaire respectif,  **OU**

* **Diffusez à l’aide de l’heure** par défaut du programme : Mardi à 9h00 HAE (New York - 12h HAE et Italie - 18h CET).

Une fois votre programme approuvé, il début en cours d’exécution dans les 15 minutes.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Bien que le programme début le _processus_ d&#39;envoi de courriers électroniques dans 15 minutes, les courriers électroniques ne seront pas _remis_ à ce moment-là. Les destinataires recevront toujours des courriels en fonction des **paramètres de fuseau horaire** que vous choisissez.

## Scénario 2 : Plus de 25 heures {#scenario-more-than-hours}

Dans ce second scénario, vous approuvez un programme de messagerie avec **fuseau horaire du Destinataire** activé et un délai de livraison planifié supérieur à 25 heures dans le futur. Dans ce cas, le programme s’exécute à l’heure planifiée dans le fuseau horaire **le plus ancien** du monde (UTC + 14:00). Il peut y avoir des personnes qui remplissent les conditions requises pour votre liste intelligente dans chaque fuseau horaire à travers le monde. Par conséquent, en commençant par le fuseau horaire le plus ancien, nous pouvons livrer le courriel à la date et à l&#39;heure prévues à tous les destinataires de leur fuseau horaire respectif.

**Début**

Parlons maintenant du fonctionnement de [Head Début](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) avec **Destinataire Time Fuseau**. Notre fonction de Début-tête actuel exige que le programme soit programmé au moins 12 heures à l&#39;avance. Qu&#39;est-ce que cela signifie pour le fuseau horaire Destinataire ? Rappelez-vous que lorsque le fuseau horaire du Destinataire est activé, nous débuts d’exécuter le programme de messagerie à l’heure planifiée dans le fuseau horaire le plus ancien (UTC +14:00). Par conséquent, pour activer **à la fois** Début principal et fuseau horaire du Destinataire, les programmes de courriel doivent être programmés **au moins 12 heures avant l&#39;heure planifiée en UTC +14:00.**

Cela signifie que si vous êtes en Amérique/Los Angeles et que vous souhaitez activer à la fois le fuseau horaire Début et Destinataire, vous devez planifier le programme **34 heures** à l&#39;avance. Comment en sommes-nous arrivés à ce chiffre ?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

En bref, les programmes de messagerie planifiés avec le fuseau horaire Destinataire doivent s’début à l’heure planifiée dans le fuseau horaire le plus ancien (c’est-à-dire, où il atteint minuit en premier) afin de prendre en compte chaque fuseau horaire. Donc, si vous planifiez un programme de courriel...

* **avec une diffusion  _dans_ 25 heures**, le programme début fonctionne dans un délai de 15 minutes. Les destinataires qui ont déjà dépassé l’heure planifiée recevront le courrier électronique en fonction des paramètres de fuseau horaire que vous avez choisis.
* **avec une diffusion de  _plus_  de 25 heures à l&#39;avenir**, le programme début s&#39;exécute à l&#39;heure planifiée dans le fuseau horaire le plus ancien (UTC +14:00).
* **avec Début** principal, le programme début traite 12 heures avant l&#39;heure planifiée dans le fuseau horaire le plus ancien (UTC +14:00).

>[!CAUTION]
>
>Toute personne qui se désabonne entre le moment où vous début votre envoi de courrier électronique et celui où il est effectivement livré recevra toujours ce message. Nous vous recommandons de modifier votre notification de désabonnement afin de tenir compte du fait que le traitement des désabonnements peut prendre entre 1 et 2 jours ouvrables.

>[!MORELIKETHIS]
>
>* [Présentation du fuseau horaire Destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Début principal pour les Programmes électroniques](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Abandonner la Diffusion des Programmes de courriel planifiés avec le fuseau horaire Destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

