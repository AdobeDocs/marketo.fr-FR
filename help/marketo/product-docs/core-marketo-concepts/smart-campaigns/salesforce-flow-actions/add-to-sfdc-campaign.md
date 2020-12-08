---
unique-page-id: 1147034
description: Ajoute à SFDC Campaign - Marketo Docs - Documentation sur les produits
title: Ajoute à la norme SFDC Campaign
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Ajoute à la norme SFDC Campaign {#add-to-sfdc-campaign}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Disponible uniquement lorsqu&#39;il est intégré à Salesforce.

## Présentation {#overview}

Cette étape de flux peut être utilisée dans les campagnes marketing ou comme étape de flux unique pour ajouter des personnes en tant que pistes dans une campagne Salesforce. Si le prospect n&#39;existe pas encore dans Salesforce, il est automatiquement synchronisé et ajouté à la campagne avec l&#39;état spécifié.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Utilisation {#usage}

1. Recherchez et sélectionnez la campagne Salesforce à laquelle vous souhaitez ajouter vos pistes.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Si vous ne voyez pas de campagne Salesforce dans la liste Campaign :
   >
   >    
   >    
   >    1. Assurez-vous que la synchronisation [de campagne est activée](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >    1. Vérifiez que votre utilisateur [](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) synchronisé Marketo est un utilisateur [](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) Marketing dans Salesforce.


   >[!TIP]
   >
   >Vous pouvez utiliser la campagne Salesforce [Mes jetons](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) pour faciliter le clonage des programmes.

1. Sélectionnez l&#39;état de membre de campagne Salesforce que vous souhaitez affecter aux pistes lorsqu&#39;elles sont ajoutées.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Si une personne est déjà membre principal de la campagne Salesforce, elle sera ignorée et son statut NE sera PAS mis à jour. Vous pouvez [modifier leur état dans une campagne](change-status-in-sfdc-campaign.md) SFDC à la place.

