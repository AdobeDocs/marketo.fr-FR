---
unique-page-id: 1147034
description: Ajoute à la DDC Campaign - Marketo Docs - Documentation du produit
title: Ajouter à la campagne SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 5%

---

# Ajouter à la campagne SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Disponible uniquement lorsqu&#39;il est intégré à Salesforce.

## Aperçu {#overview}

Cette étape de flux peut être utilisée dans les campagnes Marketo ou comme étape de flux unique pour ajouter des personnes en tant que pistes dans une campagne Salesforce. Si le prospect n&#39;existe pas encore dans Salesforce, il est automatiquement synchronisé et ajouté à la campagne avec l&#39;état spécifié.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Utilisation {#usage}

1. Recherchez et sélectionnez la campagne Salesforce à laquelle vous souhaitez ajouter vos pistes.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Si vous ne voyez pas de campagne Salesforce dans la liste Campaign :
   >
   >  1. Assurez-vous que la synchronisation de campagne [est activée](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Vérifiez que votre [utilisateur Marketo Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) est [utilisateur Marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) dans Salesforce.


   >[!TIP]
   >
   >Vous pouvez utiliser la campagne Salesforce [Mes jetons](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) pour faciliter le clonage des programmes.

1. Sélectionnez l&#39;état de membre de campagne Salesforce que vous souhaitez affecter aux pistes lorsqu&#39;elles sont ajoutées.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Si une personne est déjà membre principal de la campagne Salesforce, elle sera ignorée et son statut NE sera PAS mis à jour. Vous pouvez à la place utiliser [modifier leur état dans une campagne SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).
