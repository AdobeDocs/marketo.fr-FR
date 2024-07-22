---
description: Utilisation de l’envoi groupé de courriers électroniques de vente dans Salesforce - Documents Marketo - Documentation du produit
title: Utilisation de l’envoi groupé de courriers électroniques de vente dans Salesforce
exl-id: 4886109d-c2b8-4186-922b-8a15cf1e742e
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# Utilisation de l’envoi groupé de courriers électroniques de vente dans Salesforce {#using-bulk-send-sales-email-in-salesforce}

Découvrez comment envoyer des emails en bloc dans Salesforce pour vous aider à adapter votre communication sortante à l’aide des actions de vente.

>[!NOTE]
>
>Salesforce applique une limite de 200 enregistrements qui peuvent être sélectionnés simultanément.

>[!PREREQUISITES]
>
>Assurez-vous d’avoir installé le [dernier package Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} sur votre instance Salesforce et d’avoir configuré les [boutons d’action](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} sur vos vues de contacts et de listes de pistes dans Salesforce.

## Envoi de courriers électroniques en bloc dans Salesforce Lightning {#sending-bulk-email-in-salesforce-lightning}

1. Dans Salesforce, accédez à la page d’accueil Leads/Contacts en cliquant sur l’onglet **Leads/Contacts** .

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. Dans la liste déroulante Vue , sélectionnez la vue souhaitée des pistes/contacts que vous souhaitez envoyer par courrier électronique.

   >[!TIP]
   >
   >Vous pouvez créer une nouvelle vue en cliquant sur l’icône représentant un engrenage à droite et en sélectionnant **Nouveau**. Une fois que vous avez donné un nouveau nom à la vue et l&#39;avez enregistrée, vous pouvez cliquer sur l&#39;icône de filtrage à droite pour vous aider à filtrer vers l&#39;ensemble de Leads/Contacts que vous souhaitez envoyer par email.

1. Sélectionnez la liste de pistes ou de contacts souhaitée et cliquez sur le bouton **Envoyer le courrier électronique de vente** .

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. Vous accédez à la fenêtre Compression des actions , où sont ajoutées les personnes sélectionnées.

1. Sélectionnez le modèle que vous souhaitez insérer dans l&#39;éditeur de fenêtre de composition d&#39;actions ou créez un email personnalisé.

   >[!TIP]
   >
   >Utilisez les [catégories épinglées](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} pour faciliter l’accès à vos modèles d’email favoris.

   **ÉTAPE FACULTATIVE** : prévisualisez la personnalisation des champs dynamiques en cliquant sur le bouton **Prévisualiser les champs dynamiques** .

   >[!TIP]
   >
   >Si vous souhaitez personnaliser un modèle pour tous les destinataires, cliquez sur l&#39;option Tous les destinataires dans la barre latérale Composer en bloc pour apporter des modifications simultanément à tous les emails des destinataires. Si vous souhaitez apporter une modification à un email spécifique, cliquez sur le nom ou l’email du destinataire dans la barre latérale Composer en bloc . Veuillez noter que si vous apportez des modifications à un email individuel, puis que vous effectuez des modifications lors de la sélection de Tous les destinataires, les modifications apportées à Tous les destinataires remplaceront les modifications apportées à l&#39;email individuel.

1. Sélectionnez **Envoyer** pour envoyer immédiatement l&#39;email ou **Définir la planification** pour définir une date et une heure pour l&#39;envoi de l&#39;email.

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## Envoi de courriers électroniques en bloc dans Salesforce Classic {#sending-bulk-email-in-salesforce-classic}

1. Dans Salesforce, cliquez sur l&#39;onglet **Leads/Contacts** .

1. Dans la liste déroulante Vue , sélectionnez la vue souhaitée des pistes/contacts que vous souhaitez envoyer par courrier électronique et cliquez sur **Aller**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >Vous pouvez créer une vue en cliquant sur Créer une vue et en configurant les filtres disponibles pour réduire la liste des personnes que vous ajoutez à une campagne de ventes.

1. Sélectionnez la liste de pistes ou de contacts souhaitée et cliquez sur le bouton **Envoyer le courrier électronique de vente** .

   ![](assets/using-bulk-send-sales-email-in-salesforce-5.png)

1. Vous accédez à la fenêtre Compression des actions avec les destinataires que vous avez sélectionnés dans la fenêtre de composition.

1. Sélectionnez le modèle à insérer dans l’éditeur de fenêtre de composition d’actions ou créez un email personnalisé.

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >Utilisez les [catégories épinglées](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} pour faciliter l’accès à vos modèles d’email favoris.

   **ÉTAPE FACULTATIVE** : prévisualisez la personnalisation des champs dynamiques en cliquant sur le bouton **Prévisualiser les champs dynamiques** .

   >[!TIP]
   >
   >Si vous souhaitez personnaliser un modèle pour tous les destinataires, cliquez sur l&#39;option Tous les destinataires dans la barre latérale Composer en bloc pour apporter des modifications simultanément à tous les emails des destinataires. Si vous souhaitez apporter une modification à un email spécifique, cliquez sur le nom ou l’email du destinataire dans la barre latérale Composer en bloc . Veuillez noter que si vous apportez des modifications à un email individuel, puis que vous effectuez des modifications lors de la sélection de Tous les destinataires, les modifications apportées à Tous les destinataires remplaceront les modifications apportées à l&#39;email individuel.

1. Sélectionnez **Envoyer** pour envoyer immédiatement l&#39;email ou **Définir la planification** pour définir une date et une heure pour l&#39;envoi de l&#39;email.
