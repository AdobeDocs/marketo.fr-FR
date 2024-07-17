---
unique-page-id: 1147021
description: Changer de propriétaire - Documents Marketo - Documentation du produit
title: Modifier le détenteur
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 2%

---

# Modifier le détenteur {#change-owner}

Si des personnes existantes sont déjà affectées à un propriétaire, vous pouvez utiliser cette étape de flux pour les réaffecter à un autre propriétaire.

![](assets/change-owner-1.png)

1. Il vous suffit de choisir le propriétaire ou la file d’attente de piste vers laquelle vous souhaitez passer et de partir !

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >Salesforce n’autorise pas l’affectation de contacts aux files d’attente de piste. Pour un enregistrement qui est un contact de la DDC :
   >
   >* Marketo crée un prospect **uniquement** en double lorsque le contact est synchronisé avec Salesforce. En d’autres termes, si vous utilisez l’étape de flux **[Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** avec `AssignTo=<a lead queue>`, Marketo crée une piste en double dans Salesforce et l’affecte à la file d’attente de piste.
   >
   >* Si vous utilisez l’étape de flux **[!UICONTROL Changer de propriétaire]** sur un contact, Marketo crée un prospect en double dans Salesforce. Pour éviter cela, utilisez un filtre sur le champ &quot;Type SFDC&quot; qui limite l’action aux pistes uniquement.

   >[!NOTE]
   >
   >Si l’enregistrement n’existe pas encore dans votre compte Salesforce, nous le synchronisons, puis nous l’affectons à l’utilisateur sélectionné.
