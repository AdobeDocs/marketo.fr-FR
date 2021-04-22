---
unique-page-id: 1147031
description: Supprimer une personne de SFDC - Marketo Docs - Documentation du produit
title: Supprimer individu de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 8%

---

# Supprimer individu de SFDC {#delete-person-from-sfdc}

Si vous devez supprimer un ensemble spécifique de pistes de Salesforce mais les laisser en tant que personnes à Marketo, vous pouvez utiliser l’action de flux Supprimer une personne de SFDC.

>[!NOTE]
>
>Disponible uniquement lorsqu&#39;il est intégré à Salesforce.

1. Dans la base de données, cliquez sur la personne que vous souhaitez supprimer de Salesforce. Cliquez ensuite sur **Actions personnelles** et sélectionnez **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Sélectionnez **Supprimer une personne de SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Assurez-vous que le paramètre **Supprimer dans Marketo** est **false**, puis cliquez sur **Exécuter maintenant**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Une fois l&#39;étape de flux exécutée, votre personne ne sera plus une piste dans Salesforce mais restera à Marketo.

   >[!CAUTION]
   >
   >Si vous définissez **Supprimer dans Marketo** sur **true** et supprimez les personnes de Marketo et les prospects de Salesforce, ils sont partis pour toujours. Cette ne peut pas être annulée.
