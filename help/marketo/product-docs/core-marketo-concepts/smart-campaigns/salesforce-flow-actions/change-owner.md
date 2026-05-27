---
unique-page-id: 1147021
description: Découvrez comment modifier le propriétaire de Salesforce au cours d’une étape de flux. Affecter un nouveau prospect ou propriétaire de contact lorsque des personnes rejoignent le flux.
title: Modifier l’entité propriétaire
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/VU0fT4giNqfkF5g15q0IGIh8XuO2505nz89UuUfqZro
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 2%

---

# Modifier l’entité propriétaire {#change-owner}

Si des personnes existantes sont déjà affectées à un propriétaire, vous pouvez utiliser cette étape de flux pour les réaffecter à un autre propriétaire.

![](assets/change-owner-1.png)

1. Il vous suffit de sélectionner le propriétaire ou la file d’attente de leads vers laquelle vous souhaitez apporter des modifications et de quitter !

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >[!DNL Salesforce] ne permet pas d’affecter des contacts aux files d’attente de leads. Pour un enregistrement qui est un contact SFDC :
   >
   >* Marketo crée un prospect en double **uniquement** lorsque le contact est synchronisé avec Salesforce. En d’autres termes, si vous utilisez l’étape de flux **[Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** avec `AssignTo=<a lead queue>`, Marketo crée un prospect en double dans Salesforce et l’affecte à la file d’attente de prospects.
   >
   >* Si vous utilisez l’étape de flux **[!UICONTROL Modifier le propriétaire]** sur un contact, Marketo crée un prospect en double dans Salesforce. Pour éviter cela, utilisez un filtre sur le champ « Type de SFDC » qui limite l’action aux prospects uniquement.

   >[!NOTE]
   >
   >Si l’enregistrement n’existe pas encore dans votre compte [!DNL Salesforce], nous le synchroniserons, puis l’affecterons à l’utilisateur sélectionné.
