---
unique-page-id: 1147021
description: Changer de propriétaire - Marketo Docs - Documentation du produit
title: Modifier détenteur
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# Modifier détenteur {#change-owner}

Si des personnes existantes sont déjà affectées à un propriétaire, vous pouvez utiliser cette étape de flux pour les réaffecter à un autre propriétaire.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Utilisation**

1. Il vous suffit de choisir le propriétaire ou la file d&#39;attente de piste vers laquelle vous souhaitez passer et de partir !

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce n&#39;autorise pas l&#39;affectation de contacts aux files d&#39;attente de piste. Pour un enregistrement qui est un contact de la DDC :
   >
   >1. Marketo créera une piste de duplicata **uniquement** lorsque le contact sera synchronisé avec Salesforce. En d’autres termes, si vous utilisez l’étape de flux **[Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** avec `AssignTo=<a lead queue>`, Marketo créera une piste de duplicata dans Salesforce et l’affectera à la file d’attente de piste.
      >
      >
   1. Si vous tentez d’utiliser l’étape de flux **Changer de propriétaire** sur un contact, aucun duplicata ne sera créé dans Salesforce.


   >[!NOTE]
   >
   >Si l&#39;enregistrement n&#39;existe pas encore dans votre compte Salesforce, nous allons le synchroniser, puis l&#39;affecter à l&#39;utilisateur sélectionné.
