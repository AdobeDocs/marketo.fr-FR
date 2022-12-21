---
unique-page-id: 2949716
description: Envoi et suivi d’un courrier électronique avec le module complémentaire de messagerie pour Outlook - Documents Marketo - Documentation du produit
title: Envoi et suivi d’un courrier électronique avec le module complémentaire de messagerie pour Outlook
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Envoi et suivi d’un courrier électronique avec le module complémentaire de messagerie pour Outlook {#send-and-track-an-email-with-the-email-add-in-for-outlook}

Vous pouvez envoyer des emails et en effectuer le suivi avec Marketo directement depuis Outlook.

>[!PREREQUISITES]
>
>Si vous ne l’avez pas encore fait, installez le [Module complémentaire de messagerie Marketo pour Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md).

1. Ouvrez Microsoft Outlook et créez un email.

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >Si vous incluez plusieurs destinataires dans l&#39;email, toutes les activités seront trackées sous le premier destinataire.

1. Composer votre email comme vous le feriez normalement, puis cliquez sur **Envoi et suivi**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >Si vous envoyez un courrier électronique à une personne qui n’existe pas dans votre instance Marketo, un enregistrement de personne sera automatiquement créé pour elle. Leur nom de famille sera toujours &quot;mktUnknown&quot; afin que vous puissiez facilement les trouver.

   >[!TIP]
   >
   >Si vous souhaitez utiliser un modèle Marketo, reportez-vous à la section [Envoi et suivi depuis Outlook à l’aide d’un modèle](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. Consultez l’aperçu et cliquez sur **Envoyer**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >La technologie anti-spam rejette souvent les ouvertures et les clics qui se produisent dans les 20 secondes suivant l&#39;envoi de l&#39;email. Par conséquent, attendez au moins ce temps avant d&#39;ouvrir/cliquer pendant le test.

   Pour savoir qui a reçu vos emails envoyés par le biais d’Outlook, créez une liste dynamique à l’aide du filtre &quot;A été envoyé par courrier électronique&quot;.

   ![](assets/was-sent-sales-email.png)

C&#39;est si facile ! Même si cet email a été envoyé par Outlook d’un vendeur, il sera suivi dans Marketo.

>[!MORELIKETHIS]
>
>[Connexion au courrier entrant à partir de vos pistes dans Marketo](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
