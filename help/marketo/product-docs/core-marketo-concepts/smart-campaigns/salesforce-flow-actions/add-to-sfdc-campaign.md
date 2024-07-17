---
unique-page-id: 1147034
description: Ajouter à SFDC Campaign - Documents Marketo - Documentation du produit
title: Ajouter à la campagne SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 5%

---

# Ajouter à la campagne SFDC {#add-to-sfdc-campaign}

Cette étape de flux peut être utilisée dans les campagnes Marketo Engage ou en tant qu’étape de flux unique pour ajouter des personnes en tant que pistes dans une campagne Salesforce. Si la piste n’existe pas encore dans Salesforce, elle sera automatiquement synchronisée et ajoutée à la campagne avec le statut spécifié.

>[!NOTE]
>
>Disponible uniquement lorsqu’il est intégré à Salesforce.

![](assets/add-to-sfdc-campaign-1.png)

## Utilisation {#usage}

1. Recherchez et sélectionnez la campagne Salesforce à laquelle vous souhaitez ajouter vos pistes.

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >Si une campagne Salesforce n’apparaît pas dans la liste des campagnes :
   >
   >  1. Assurez-vous que la [synchronisation de campagne est activée](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
   >  1. Confirmez que votre [utilisateur de synchronisation de Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} est un [utilisateur marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} dans Salesforce.

   >[!TIP]
   >
   >Vous pouvez utiliser la campagne Salesforce [My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} pour faciliter le clonage des programmes.

1. Sélectionnez le statut de membre de campagne Salesforce que vous souhaitez affecter aux pistes lorsqu’elles sont ajoutées.

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >Si une personne est déjà membre principal de la campagne Salesforce, elle sera ignorée et son statut NE sera PAS mis à jour. Vous pouvez utiliser [modifier leur état dans une campagne SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"} à la place.
