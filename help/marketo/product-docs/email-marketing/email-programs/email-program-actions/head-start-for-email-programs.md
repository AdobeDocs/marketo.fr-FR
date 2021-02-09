---
unique-page-id: 10097202
description: Début principal pour les Programmes électroniques - Documents marketing - Documentation du produit
title: Début principal pour les Programmes électroniques
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---


# Début principal pour les Programmes de courriel {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Créer un Programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Lorsque vous choisissez une date/heure pour un Programme de courriel, il détermine à quel moment le programme commencera à se traiter. Si vous souhaitez que vos courriers électroniques soient lancés à l’heure sélectionnée, Head Début vous offre cette option en traitant le programme à l’avance.

## Début principal standard {#standard-head-start}

1. Cliquez sur **Activités marketing**.

   ![](assets/one-1.png)

1. Recherchez et sélectionnez votre Programme de messagerie.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Le Début d’en-tête ne peut pas être utilisé avec les tests A/B.

1. Dans la mosaïque Planification, planifiez votre adresse électronique, puis sélectionnez la zone **Début d’en-tête**.

   ![](assets/three-1.png)

   Le Début principal étant sélectionné, le programme commencera à traiter environ 12 heures avant l’heure prévue. Une fois les débuts de traitement traités, le programme est verrouillé.

   >[!CAUTION]
   >
   >Toute personne de votre audience qui se désabonne après le verrouillage du programme recevra toujours le courrier électronique. Nous vous recommandons de modifier votre notification de désabonnement afin de tenir compte du fait que le traitement des désabonnements peut prendre entre 1 et 2 jours ouvrables.

1. Cliquez sur **Approuver le Programme**.

   ![](assets/four-1.png)

   Après l’approbation du programme, vous pouvez afficher quatre états différents sur le volet Approbation.

   * **En attente d’exécution :** après l’approbation du programme.
   * **Le traitement a démarré, en attente d’exécution : le** traitement est en cours.
   * **Traitement terminé, en attente d’exécution :** Traitement terminé, envoi d’un courrier électronique en attente de lancement planifié.
   * **Terminé :** Programme terminé.

   >[!TIP]
   >
   >Voulez-vous annuler après le verrouillage du programme mais avant l&#39;envoi du courriel ? Pas de problème ! Il vous suffit de cliquer sur **Abandonner le Programme** dans l’angle inférieur droit de la mosaïque Approbation.

   >[!NOTE]
   >
   >Si vous désapprouvez votre programme de messagerie avec moins de 12 heures avant son exécution planifiée, mais que vous changez d’avis, vous devez choisir une nouvelle date/heure qui est au moins 12 heures en avance par rapport à son approbation.

## Début principal avec fuseau horaire Destinataire {#head-start-with-recipient-time-zone}

Notre fonction de Début-tête actuel exige que le programme soit programmé au moins 12 heures à l&#39;avance. Qu&#39;est-ce que cela signifie pour le fuseau horaire Destinataire ? Rappelez-vous que lorsque le fuseau horaire du Destinataire est principal, nous débuts à exécuter le programme électronique à minuit dans le fuseau horaire le plus proche (UTC +14:00). Ainsi, pour activer **à la fois** Début principal et fuseau horaire Destinataire, les programmes doivent être programmés **au moins 12 heures avant le fuseau horaire le plus ancien (UTC +14:00**).

Cela signifie que si vous êtes en Amérique/Los Angeles et que vous souhaitez activer à la fois le fuseau horaire Début et Destinataire, vous devez planifier le programme **34 heures** à l&#39;avance. Comment en sommes-nous arrivés à ce chiffre ?

![](assets/image2017-12-5-13-3a11-3a46.png)

[En savoir ](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) plus sur la planification des programmes de messagerie avec fuseau horaire Destinataire.

>[!MORELIKETHIS]
>
>* [Planification de votre Programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Planification des Programmes de courriel avec fuseau horaire Destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Présentation du fuseau horaire Destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

