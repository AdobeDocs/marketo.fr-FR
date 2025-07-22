---
unique-page-id: 2949716
description: Envoi et suivi d’un e-mail avec le complément d’e-mail pour  [!DNL Outlook] - Documents Marketo - Documentation du produit
title: Envoyer et suivre un e-mail avec le complément d'e-mail pour  [!DNL Outlook]
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Envoi et suivi d’un e-mail avec le complément d’e-mail pour [!DNL Outlook] {#send-and-track-an-email-with-the-email-add-in-for-outlook}

Vous pouvez envoyer et suivre les e-mails avec Marketo directement depuis [!DNL Outlook].

>[!PREREQUISITES]
>
>Si vous ne l&#39;avez pas encore fait, installez le complément d&#39;e-mail [Marketo pour  [!DNL Outlook]](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md).

>[!NOTE]
>
>Les fonctionnalités Actions de Sales Insight, notamment Envoyer un e-mail de vente, Ajouter à la campagne de vente et Tâches, ne sont pas disponibles dans les plug-ins de messagerie de Sales Insight pour Gmail et Outlook. Actuellement, les utilisateurs ne peuvent envoyer qu’un e-mail trackable avec ou sans modèle d’e-mail Marketo à partir de leur client de messagerie lors de l’utilisation des modules externes d’e-mail Sales Insight.

1. Ouvrez Microsoft Outlook et créez un e-mail.

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >Si vous incluez plusieurs destinataires dans l’e-mail, toutes les activités seront suivies sous le premier destinataire.

1. Composez votre e-mail comme vous le feriez normalement, puis cliquez sur **[!UICONTROL Envoyer et suivre]**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >Si vous envoyez un e-mail à une personne qui n’existe pas dans votre instance Marketo, un enregistrement de personne est automatiquement créé pour cette personne. Leur nom de famille sera toujours « mktUnknown » afin que vous puissiez les retrouver facilement.

   >[!TIP]
   >
   >Si vous souhaitez utiliser un modèle Marketo, reportez-vous à la section [Envoi et suivi à partir de [!DNL Outlook] Utilisation d’un modèle](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. Affichez l’aperçu et cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >La technologie antispam rejette souvent les ouvertures et les clics qui se produisent dans les 20 secondes suivant l&#39;envoi de l&#39;e-mail. Attendez donc au moins cette durée pour ouvrir/cliquer lors du test.

   Pour savoir qui a reçu vos e-mails envoyés par l’intermédiaire de [!DNL Outlook], créez une liste dynamique à l’aide du filtre « E-mail de vente [!UICONTROL &#x200B; a été envoyé &#x200B;] ».

   ![](assets/was-sent-sales-email.png)

C&#39;est aussi facile que ça ! Même si cet e-mail a été envoyé par le [!DNL Outlook] d’un vendeur, il sera suivi dans Marketo.

>[!MORELIKETHIS]
>
>[Enregistrer le courrier entrant provenant de vos prospects dans Marketo](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
