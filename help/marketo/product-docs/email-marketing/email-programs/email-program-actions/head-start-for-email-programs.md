---
unique-page-id: 10097202
description: Prise en main des programmes de messagerie - Documents Marketo - Documentation du produit
title: Prise en main des programmes de messagerie
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Prise en main des programmes de messagerie {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Création d’un programme de courrier électronique](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Lorsque vous choisissez une date/heure pour un programme de messagerie, il détermine le moment auquel le traitement commencera. Si vous souhaitez que vos emails soient lancés à l’heure sélectionnée, cette option est proposée en traitant le programme à l’avance.

## Début d’en-tête standard {#standard-head-start}

1. Cliquez sur **Activités marketing**.

   ![](assets/one-1.png)

1. Recherchez et sélectionnez votre programme de messagerie.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Il n’est pas possible d’utiliser Head Start avec les tests A/B.

1. Dans la mosaïque Planification , planifiez votre email, puis sélectionnez l’option **Début** de la boîte.

   ![](assets/three-1.png)

   Lorsque l’option Début anticipé est sélectionnée, le traitement du programme commencera environ 12 heures avant l’heure planifiée. Une fois le traitement démarré, le programme est verrouillé.

   >[!CAUTION]
   >
   >Toute personne de votre audience qui se désinscrit après le verrouillage du programme recevra toujours l’email. Nous vous recommandons d’ajuster votre notification de désabonnement pour tenir compte du fait que le traitement des désabonnements peut prendre entre 1 et 2 jours ouvrables.

1. Cliquez sur **Programme d’approbation**.

   ![](assets/four-1.png)

   Après l’approbation du programme, vous pouvez voir quatre statuts différents sur la mosaïque Approbation .

   * **En attente d’exécution :** Une fois le programme approuvé.
   * **Le traitement a commencé, en attente d’exécution :** Le traitement est en cours.
   * **Traitement terminé, en attente d’exécution :** Traitement terminé, courrier électronique en attente de l’heure planifiée de lancement.
   * **Terminé :** Programme terminé.

   >[!TIP]
   >
   >Vous souhaitez annuler après le verrouillage du programme, mais avant l&#39;envoi de l&#39;email ? Pas de problème ! Cliquez simplement sur **Programme d’abandon** dans le coin inférieur droit de la mosaïque Approbation .

   >[!NOTE]
   >
   >Si vous annulez l’approbation de votre programme de messagerie avec moins de 12 heures avant l’heure d’exécution planifiée, mais que vous changez d’avis, vous devrez choisir une nouvelle date/heure qui est au moins 12 heures avant la date d’approbation.

## Début avec le fuseau horaire du destinataire {#head-start-with-recipient-time-zone}

Pour utiliser la fonctionnalité de prise en main existante, le programme doit être programmé au moins 12 heures à l’avance. Qu’est-ce que cela signifie pour le fuseau horaire des destinataires ? Rappelez-vous que lorsque le fuseau horaire du destinataire est principal, nous commençons à exécuter le programme d’email à minuit dans le fuseau horaire le plus proche (UTC +14:00). Ainsi, pour activer **both** Heure de début et fuseau horaire du destinataire, les programmes doivent être planifiés. **au moins 12 heures avant le premier fuseau horaire (UTC +14:00**.)

Cela signifie que si vous êtes aux États-Unis/à Los Angeles et que vous souhaitez activer à la fois Head Start et Recipient Time Zone, vous devez planifier le programme. **34 heures** à l&#39;avance. Comment en sommes-nous arrivés à ce nombre ?

![](assets/image2017-12-5-13-3a11-3a46.png)

[En savoir plus](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) sur la planification des programmes de messagerie avec le fuseau horaire du destinataire.

>[!MORELIKETHIS]
>
>* [Planification de votre programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Planification des programmes de messagerie avec un fuseau horaire de destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Comprendre le fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

