---
unique-page-id: 1147021
description: Changer de propriétaire - Documents marketing - Documentation du produit
title: Changer de propriétaire
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Changer de propriétaire {#change-owner}

Si des personnes existantes sont déjà affectées à un propriétaire, vous pouvez utiliser cette étape de flux pour les réaffecter à un autre propriétaire.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Utilisation**

1. Il vous suffit de choisir le propriétaire ou la file d&#39;attente de piste vers laquelle vous souhaitez passer et de partir !

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce n&#39;autorise pas l&#39;affectation de contacts aux files d&#39;attente de piste. Pour un enregistrement qui est un contact de la DDC :
   >
   >1. Marketo crée une piste de duplicata **uniquement** lorsque le contact est synchronisé avec Salesforce. En d’autres termes, si vous utilisez l’étape de flux **[Synchroniser la personne avec SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** avec `AssignTo=<a lead queue>`, Marketo créera une piste de duplicata dans Salesforce et l’affectera à la file d’attente de piste.
      >
      >
   1. Si vous tentez d&#39;utiliser l&#39;étape de flux **Changer de propriétaire** sur un contact, aucun duplicata ne sera créé dans Salesforce.


   >[!NOTE]
   >
   >Si l&#39;enregistrement n&#39;existe pas encore dans votre compte Salesforce, nous allons le synchroniser, puis l&#39;affecter à l&#39;utilisateur sélectionné.
