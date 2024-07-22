---
unique-page-id: 13795727
description: Abandonner la diffusion des programmes de messagerie planifiés avec le fuseau horaire du destinataire - Documents Marketo - Documentation du produit
title: Abandonner la diffusion des programmes de messagerie planifiés avec le fuseau horaire du destinataire
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Abandonner la diffusion des programmes de messagerie planifiés avec le fuseau horaire du destinataire {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

En cas d’urgence, vous pouvez interrompre la diffusion d’un programme de messagerie qui a déjà commencé à s’exécuter avec l’option Fuseau horaire du destinataire activée.

Comme les programmes de messagerie programmés avec le fuseau horaire des destinataires peuvent s’exécuter pendant 24 heures au maximum, l’abandon de la diffusion du programme annule les envois ultérieurs.

1. Sélectionnez le programme de messagerie que vous souhaitez annuler, puis cliquez sur **Abandonner la diffusion** sous la mosaïque Approbation du panneau de contrôle.

   ![](assets/ptz-abortdelivery.png)

1. Confirmez que vous souhaitez annuler la diffusion en cliquant sur **Abandonner**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Après l&#39;annulation, la grille **Résultats** de votre programme de messagerie ressemblera à celle ci-dessous. Tous les envois suivants sont annulés et s’afficheront comme &quot;Email Bounce Soft&quot; dans la colonne **Type d’activité**.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Les emails annulés **not** s’affichent en tant que soft bounce *jusqu’à* la date initialement prévue pour leur diffusion dans leurs fuseaux horaires respectifs. Jusqu’à ce moment-là, ils s’afficheront toujours comme &quot;Envoyer un courrier électronique&quot;.

1. Dans la grille, vous pouvez cliquer sur n’importe quel email pour afficher les détails de l’activité. Pour un envoi annulé, la fenêtre contextuelle des détails se présente comme suit :

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Comprendre le fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Planification de programmes de messagerie avec fuseau horaire de destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
