---
description: Utilisation de l’envoi en bloc d’e-mails commerciaux dans Salesforce - Documents Marketo - Documentation du produit
title: Utilisation de l’option Envoyer des e-mails de vente en masse dans Salesforce
exl-id: 4886109d-c2b8-4186-922b-8a15cf1e742e
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 2%

---

# Utilisation de l’option Envoyer des e-mails de vente en masse dans Salesforce {#using-bulk-send-sales-email-in-salesforce}

Découvrez comment envoyer des e-mails en bloc dans Salesforce pour adapter votre communication sortante à l’aide d’actions de vente.

>[!NOTE]
>
>Salesforce applique une limite de 200 enregistrements pouvant être sélectionnés à la fois.

>[!PREREQUISITES]
>
>Assurez-vous d’avoir installé le [dernier package Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} sur votre instance Salesforce et d’avoir configuré les [&#x200B; boutons d’action](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} dans les vues de liste de contacts et de leads dans Salesforce.

## Envoi d’e-mails en bloc dans Salesforce Lightning {#sending-bulk-email-in-salesforce-lightning}

1. Dans Salesforce, accédez à la page d’accueil Leads/Contacts en cliquant sur l’onglet **Leads/Contacts**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. Dans la liste déroulante Affichage , sélectionnez l’affichage souhaité des prospects/contacts à envoyer par e-mail.

   >[!TIP]
   >
   >Vous pouvez créer une nouvelle vue en cliquant sur l’icône représentant un engrenage à droite et en sélectionnant **Nouveau**. Une fois que vous avez donné un nouveau nom à la vue et que vous l’avez enregistrée, vous pouvez cliquer sur l’icône de filtre à droite pour filtrer l’ensemble de prospects/contacts que vous souhaitez envoyer par e-mail.

1. Choisissez la liste de leads ou de contacts souhaitée, puis cliquez sur le bouton **Envoyer un e-mail de vente**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. Vous accédez à la fenêtre de composition Actions, avec les personnes que vous avez sélectionnées ajoutées.

1. Sélectionnez le modèle à insérer dans l’éditeur de fenêtre de composition d’actions ou écrivez un e-mail personnalisé.

   >[!TIP]
   >
   >Utilisez [Catégories épinglées](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} pour faciliter l’accès à vos modèles d’e-mail préférés.

   **ÉTAPE FACULTATIVE** : prévisualisez toute personnalisation de champ dynamique en cliquant sur le bouton **Prévisualiser les champs dynamiques**.

   >[!TIP]
   >
   >Si vous souhaitez personnaliser un modèle pour tous les destinataires, cliquez sur l’option Tous les destinataires dans la barre latérale Composer en bloc pour apporter des modifications simultanément à tous les e-mails des destinataires. Si vous souhaitez apporter une modification à un e-mail spécifique, cliquez sur le nom ou l’e-mail du destinataire dans la barre latérale Composer en bloc. Veuillez noter que si vous apportez des modifications à un e-mail individuel puis que vous le modifiez en sélectionnant Tous les destinataires, les modifications apportées à Tous les destinataires remplaceront les modifications apportées à l’e-mail individuel.

1. Sélectionnez **Envoyer** pour envoyer l’e-mail immédiatement, ou **Définir le planning** pour définir la date et l’heure d’envoi de l’e-mail.

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## Envoi d’e-mails en bloc dans Salesforce Classic {#sending-bulk-email-in-salesforce-classic}

1. Dans Salesforce, cliquez sur l’onglet **Leads/contacts**.

1. Dans la liste déroulante Affichage , sélectionnez l’affichage des prospects/contacts à envoyer par e-mail, puis cliquez sur **Aller**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >Vous pouvez créer une vue en cliquant sur Créer une vue et en configurant les filtres disponibles pour réduire la liste des personnes que vous ajoutez à une campagne de ventes.

1. Sélectionnez la liste de leads ou de contacts souhaitée et cliquez sur le bouton **Envoyer un e-mail de vente**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-5.png)

1. Vous accédez à la fenêtre de composition Actions avec les destinataires que vous avez sélectionnés dans la fenêtre de composition.

1. Sélectionnez le modèle à insérer dans l’éditeur de fenêtre de composition d’actions ou écrivez un e-mail personnalisé.

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >Utilisez [Catégories épinglées](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} pour faciliter l’accès à vos modèles d’e-mail préférés.

   **ÉTAPE FACULTATIVE** : prévisualisez toute personnalisation de champ dynamique en cliquant sur le bouton **Prévisualiser les champs dynamiques**.

   >[!TIP]
   >
   >Si vous souhaitez personnaliser un modèle pour tous les destinataires, cliquez sur l’option Tous les destinataires dans la barre latérale Composer en bloc pour apporter des modifications simultanément à tous les e-mails des destinataires. Si vous souhaitez apporter une modification à un e-mail spécifique, cliquez sur le nom ou l’e-mail du destinataire dans la barre latérale Composer en bloc. Veuillez noter que si vous apportez des modifications à un e-mail individuel puis que vous le modifiez en sélectionnant Tous les destinataires, les modifications apportées à Tous les destinataires remplaceront les modifications apportées à l’e-mail individuel.

1. Sélectionnez **Envoyer** pour envoyer l’e-mail immédiatement, ou **Définir le planning** pour définir la date et l’heure d’envoi de l’e-mail.
