---
unique-page-id: 1147031
description: Supprimer une personne de SFDC - Documents marketing - Documentation du produit
title: Supprimer une personne de SFDC
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---


# Supprimer une personne de la collecte de données régionale {#delete-person-from-sfdc}

Si vous devez supprimer un ensemble spécifique de pistes de Salesforce mais les laisser en tant que personnes dans Marketo, vous pouvez utiliser l’action Supprimer une personne de SFDC.

>[!NOTE]
>
>Disponible uniquement lorsqu&#39;il est intégré à Salesforce.

1. Dans la base de données, cliquez sur la personne que vous souhaitez supprimer de Salesforce. Cliquez ensuite sur **Actions personnelles** et sélectionnez **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Sélectionnez **Supprimer une personne de SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Assurez-vous que le paramètre **Supprimer dans Marketo** est **false**, puis cliquez sur **Exécuter maintenant**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Une fois l’étape de flux exécutée, votre personne ne sera plus une piste dans Salesforce, mais restera sur le marché.

   >[!CAUTION]
   >
   >Si vous définissez **Supprimer dans Marketo** sur **true** et supprimez les personnes de Marketo et les pistes de Salesforce, elles sont définitivement disparues. Cela ne peut pas être annulé.
