---
unique-page-id: 13795727
description: Abandon de la diffusion des programmes de messagerie programmés avec le fuseau horaire du destinataire - Documents Marketo - Documentation du produit
title: Abandonner la diffusion des programmes de messagerie programmés avec le fuseau horaire du destinataire
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Abandonner la diffusion des programmes de messagerie programmés avec le fuseau horaire du destinataire {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

En cas d’urgence, vous pouvez abandonner l’envoi d’un programme de messagerie qui a déjà commencé à s’exécuter avec le fuseau horaire du destinataire activé.

Comme les programmes d’e-mail planifiés avec le fuseau horaire du destinataire peuvent durer jusqu’à 24 heures, l’abandon de la diffusion du programme annule tous les envois suivants après ce moment.

1. Sélectionnez le programme de messagerie que vous souhaitez annuler, puis cliquez sur **[!UICONTROL Abandonner la diffusion]** sous la mosaïque [!UICONTROL Validation] du panneau de contrôle.

   ![](assets/ptz-abortdelivery.png)

1. Confirmez votre choix en cliquant sur **[!UICONTROL Abandonner]**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Après l’annulation, la grille **[!UICONTROL Résultats]** de votre programme d’e-mail ressemblera à celle ci-dessous. Tous les envois suivants sont annulés et s’afficheront sous la forme « E-mail rebond soft » dans la colonne **[!UICONTROL Type d’activité]**.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Les e-mails annulés **ne s** affichent pas comme soft bounce *jusqu&#39;à* l&#39;heure à laquelle leur diffusion était initialement prévue dans leurs fuseaux horaires respectifs. Jusque là, ils s’affichent toujours sous la forme « Envoyer un e-mail ».

1. Dans la grille, vous pouvez cliquer sur n’importe quel e-mail pour afficher les détails de l’activité. Pour un envoi annulé, le pop-up de détails ressemble à ceci :

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Présentation du fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Planification de programmes de messagerie avec fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
