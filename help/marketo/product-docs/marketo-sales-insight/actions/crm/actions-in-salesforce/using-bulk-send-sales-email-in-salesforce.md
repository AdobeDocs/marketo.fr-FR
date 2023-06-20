---
description: Utilisation de l’envoi groupé de courriers électroniques de vente dans Salesforce - Documents Marketo - Documentation du produit
title: Utilisation de l’envoi groupé de courriers électroniques de vente dans Salesforce
source-git-commit: 4d88547ecdc25a2a1e0de49fab1493bbefd6800b
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Utilisation de l’envoi groupé de courriers électroniques de vente dans Salesforce {#using-bulk-send-sales-email-in-salesforce}

Découvrez comment envoyer des emails en bloc dans Salesforce pour vous aider à adapter votre communication sortante à l’aide des actions de vente.

>[!NOTE]
>
>Salesforce applique une limite de 200 enregistrements qui peuvent être sélectionnés simultanément.

>[!PREREQUISITES]
>
>Assurez-vous que vous avez installé le [dernier package Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} to your Salesforce instance and have configured the [Action buttons](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} dans les vues de vos listes de contacts et de prospects dans Salesforce.

## Envoi de courriers électroniques en bloc dans Salesforce Lightning {#sending-bulk-email-in-salesforce-lightning}

1. Dans Salesforce, accédez à la page d’accueil Leads/Contacts en cliquant sur le bouton **Prospects/contacts** .

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. Dans la liste déroulante Vue , sélectionnez la vue souhaitée des pistes/contacts que vous souhaitez envoyer par courrier électronique.

   >[!TIP]
   >
   >Vous pouvez créer un affichage en cliquant sur l’icône représentant un engrenage à droite et en sélectionnant **Nouveau**. Une fois que vous avez donné un nouveau nom à la vue et l&#39;avez enregistrée, vous pouvez cliquer sur l&#39;icône de filtrage à droite pour vous aider à filtrer vers l&#39;ensemble de Leads/Contacts que vous souhaitez envoyer par email.

1. Sélectionnez la liste de contacts ou de pistes souhaitées, puis cliquez sur le bouton **Envoyer un e-mail de vente** bouton .

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. Vous accédez à la fenêtre Compression des actions , où sont ajoutées les personnes sélectionnées.

1. Sélectionnez le modèle que vous souhaitez insérer dans l&#39;éditeur de fenêtre de composition d&#39;actions ou créez un email personnalisé.

   >[!TIP]
   >
   >Utilisation [Catégories épinglées](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} pour faciliter l’accès à vos modèles d’email favoris.

   **ÉTAPE FACULTATIVE**: Prévisualisez la personnalisation des champs dynamiques en cliquant sur le bouton **Aperçu des champs dynamiques** bouton .

   >[!TIP]
   >
   >Si vous souhaitez personnaliser un modèle pour tous les destinataires, cliquez sur l&#39;option Tous les destinataires dans la barre latérale Composer en bloc pour apporter des modifications simultanément à tous les emails des destinataires. Si vous souhaitez apporter une modification à un email spécifique, cliquez sur le nom ou l’email du destinataire dans la barre latérale Composer en bloc . Veuillez noter que si vous apportez des modifications à un email individuel, puis que vous effectuez des modifications lors de la sélection de Tous les destinataires, les modifications apportées à Tous les destinataires remplaceront les modifications apportées à l&#39;email individuel.

1. Sélectionner **Envoyer** pour envoyer immédiatement l’e-mail, ou **Définir la planification** pour définir la date et l’heure d’envoi du courrier électronique.

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## Envoi de courriers électroniques en bloc dans Salesforce Classic {#sending-bulk-email-in-salesforce-classic}

1. Dans Salesforce, cliquez sur l’icône **Prospects/contacts** .

1. Dans la liste déroulante Vue , sélectionnez la vue souhaitée des pistes/contacts que vous souhaitez envoyer par courrier électronique, puis cliquez sur **Aller**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >Vous pouvez créer une vue en cliquant sur Créer une vue et en configurant les filtres disponibles pour réduire la liste des personnes que vous ajoutez à une campagne de ventes.

1. Sélectionnez la liste de contacts ou de pistes souhaitée, puis cliquez sur le bouton **Envoyer un e-mail de vente** bouton .

1. Vous accédez à la fenêtre Compression des actions avec les destinataires que vous avez sélectionnés dans la fenêtre de composition.

1. Sélectionnez le modèle à insérer dans l’éditeur de fenêtre de composition d’actions ou créez un email personnalisé.

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >Utilisation [Catégories épinglées](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} pour faciliter l’accès à vos modèles d’email favoris.

   **ÉTAPE FACULTATIVE**: Prévisualisez la personnalisation des champs dynamiques en cliquant sur le bouton **Aperçu des champs dynamiques** bouton .

   >[!TIP]
   >
   >Si vous souhaitez personnaliser un modèle pour tous les destinataires, cliquez sur l&#39;option Tous les destinataires dans la barre latérale Composer en bloc pour apporter des modifications simultanément à tous les emails des destinataires. Si vous souhaitez apporter une modification à un email spécifique, cliquez sur le nom ou l’email du destinataire dans la barre latérale Composer en bloc . Veuillez noter que si vous apportez des modifications à un email individuel, puis que vous effectuez des modifications lors de la sélection de Tous les destinataires, les modifications apportées à Tous les destinataires remplaceront les modifications apportées à l&#39;email individuel.

1. Sélectionner **Envoyer** pour envoyer immédiatement l’e-mail, ou **Définir la planification** pour définir la date et l’heure d’envoi du courrier électronique.
