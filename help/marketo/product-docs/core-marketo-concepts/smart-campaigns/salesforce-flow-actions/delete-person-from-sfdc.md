---
unique-page-id: 1147031
description: Supprimer une personne de SFDC - Documents Marketo - Documentation du produit
title: Supprimer individu de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 8%

---

# Supprimer individu de SFDC {#delete-person-from-sfdc}

Si vous devez supprimer un ensemble spécifique de pistes de Salesforce tout en les laissant comme des personnes en Marketo Engage, vous pouvez utiliser l’action Supprimer la personne de flux SFDC .

>[!NOTE]
>
>Disponible uniquement lorsqu’il est intégré à Salesforce.

1. Dans la base de données, cliquez sur la personne à supprimer de Salesforce. Cliquez ensuite sur **[!UICONTROL Actions de personne]** et sélectionnez **[!DNL Salesforce]**.

   ![](assets/person-actions-salesforce.png)

1. Sélectionner **[!UICONTROL Supprimer une personne de SFDC]**.

   ![](assets/delete-person-from-sfdc.png)

1. Assurez-vous que la variable **[!UICONTROL Supprimer dans Marketo]** paramètre **[!UICONTROL false]**, puis cliquez sur **[!UICONTROL Exécuter maintenant]**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Une fois l’étape de flux exécutée, votre personne ne sera plus une piste dans Salesforce, mais restera dans Marketo.

   >[!CAUTION]
   >
   >Si vous définissez **[!UICONTROL Supprimer dans Marketo]** to **[!UICONTROL true]** et supprimez les personnes de Marketo et les prospects de Salesforce, ils sont partis pour toujours. Cette ne peut pas être annulée.
