---
unique-page-id: 10097202
description: Démarrage rapide des programmes de messagerie - Documents Marketo - Documentation du produit
title: Démarrage rapide des programmes d’e-mail
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 2%

---

# Démarrage rapide des programmes d’e-mail {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Créer un programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Lorsque vous choisissez une date/heure pour un programme d’e-mail, il détermine à quel moment le programme commencera le traitement. Si vous souhaitez que vos e-mails soient lancés à l’heure sélectionnée, le menu Démarrer vous offre cette option en traitant le programme à l’avance.

## Démarrage anticipé standard {#standard-head-start}

1. Cliquez sur **[!UICONTROL Activités marketing]**.

   ![](assets/one-1.png)

1. Recherchez et sélectionnez votre programme de messagerie.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Le démarrage anticipé ne peut pas être utilisé avec les tests A/B.

1. Dans la mosaïque [!UICONTROL  Planifier ], planifiez votre e-mail, puis sélectionnez la zone **[!UICONTROL Démarrage rapide]**.

   ![](assets/three-1.png)

   Une fois [!UICONTROL Démarrage rapide] sélectionné, le programme commencera à traiter environ 12 heures avant l’heure prévue. Une fois le traitement démarré, le programme est verrouillé.

   >[!CAUTION]
   >
   >Toute personne de votre audience qui se désabonne après le verrouillage du programme recevra toujours l’e-mail. Nous vous recommandons d’ajuster votre notification de désabonnement pour tenir compte du fait que le traitement des désabonnements peut prendre entre 1 et 2 jours ouvrables.

1. Cliquez sur **[!UICONTROL Approuver le programme]**.

   ![](assets/four-1.png)

   Après l’approbation du programme, quatre statuts différents peuvent s’afficher sur la mosaïque Approbation .

   * **[!UICONTROL En attente d’exécution] :** une fois le programme approuvé.
   * **[!UICONTROL Traitement démarré, en attente d’exécution]:** Le traitement est en cours.
   * **[!UICONTROL Traitement terminé, en attente d’exécution]:** Traitement terminé, l’e-mail attend désormais l’heure de lancement planifiée.
   * **[!UICONTROL Terminé]:** Le programme est terminé.

   >[!TIP]
   >
   >Vous souhaitez annuler après le verrouillage du programme, mais avant l’envoi de l’e-mail ? Pas de problème ! Il vous suffit de cliquer sur **[!UICONTROL Abandonner le programme]** dans le coin inférieur droit de la mosaïque Approbation.

   >[!NOTE]
   >
   >Si vous désapprouvez votre programme de messagerie moins de 12 heures avant son heure d’exécution prévue, mais que vous changez ensuite d’avis, vous devez choisir une nouvelle date/heure avec au moins 12 heures d’avance sur la date de votre approbation.

## Prise en main du fuseau horaire du destinataire {#head-start-with-recipient-time-zone}

Notre fonctionnalité Bon départ exige que le programme soit planifié au moins 12 heures à l&#39;avance. Qu’est-ce que cela signifie pour le fuseau horaire du destinataire ? Rappelez-vous que lorsque le fuseau horaire du destinataire est actif, nous commençons à exécuter le programme d’e-mail à minuit dans le premier fuseau horaire (UTC +14:00). Ainsi, pour activer **à la fois** le démarrage rapide et le fuseau horaire du destinataire, les programmes doivent être planifiés **au moins 12 heures avant le fuseau horaire le plus proche (UTC +14:00**).

Cela signifie que si vous êtes en Amérique/Los Angeles et que vous souhaitez activer les fuseaux horaires Head Start et Recipient, vous devez planifier le programme **34 heures** à l&#39;avance. Comment en sommes-nous arrivés à ce chiffre ?

![](assets/image2017-12-5-13-3a11-3a46.png)

[En savoir plus](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) sur la planification de programmes d’e-mail avec le fuseau horaire du destinataire.

>[!MORELIKETHIS]
>
>* [Planifier Votre Programme De Messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Planification de programmes de messagerie avec fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Présentation du fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
