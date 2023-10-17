---
unique-page-id: 1147021
description: Changer de propriétaire - Documents Marketo - Documentation du produit
title: Modifier détenteur
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 2%

---

# Modifier détenteur {#change-owner}

Si des personnes existantes sont déjà affectées à un propriétaire, vous pouvez utiliser cette étape de flux pour les réaffecter à un autre propriétaire.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Utilisation**

1. Il vous suffit de choisir le propriétaire ou la file d’attente de piste vers laquelle vous souhaitez passer et de partir !

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce n’autorise pas l’affectation de contacts aux files d’attente de piste. Pour un enregistrement qui est un contact de la DDC :
   >
   >1. Marketo crée un prospect en double **only** lorsque le contact est synchronisé avec Salesforce. En d’autres termes, si vous utilisez la variable **[Personne synchronisée avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** étape de flux avec `AssignTo=<a lead queue>`, Marketo crée une piste en double dans Salesforce et l’affecte à la file d’attente de piste.
   >
   >1. Si vous utilisez la variable **[!UICONTROL Modifier le propriétaire]** étape de flux sur un contact, Marketo crée un prospect en double dans Salesforce. Pour éviter cela, utilisez un filtre sur le champ &quot;Type SFDC&quot; qui limite l’action aux pistes uniquement.

   >[!NOTE]
   >
   >Si l’enregistrement n’existe pas encore dans votre compte Salesforce, nous le synchronisons, puis nous l’affectons à l’utilisateur sélectionné.
