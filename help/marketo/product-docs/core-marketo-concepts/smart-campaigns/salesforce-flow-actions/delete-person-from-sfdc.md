---
unique-page-id: 1147031
description: Découvrez comment supprimer une personne de Salesforce à l’aide d’une étape de flux. Supprimez le prospect ou le contact de SFDC lorsqu’il ou elle accède au flux.
title: Supprimer une personne de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 5%

---

# Supprimer une personne de SFDC {#delete-person-from-sfdc}

Si vous devez supprimer un ensemble spécifique de prospects de Salesforce, mais les laisser en tant que personnes dans Marketo Engage, vous pouvez utiliser l’action de flux Supprimer une personne de SFDC .

>[!NOTE]
>
>Disponible uniquement lorsqu’il est intégré à [!DNL Salesforce].

1. Dans la base de données, cliquez sur la personne à supprimer de Salesforce. Cliquez ensuite sur **[!UICONTROL Actions de la personne]** et sélectionnez **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Sélectionnez **[!UICONTROL Supprimer une personne de SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Assurez-vous que le paramètre **[!UICONTROL Supprimer dans Marketo]** est défini sur **[!UICONTROL false]**, puis cliquez sur **[!UICONTROL Exécuter maintenant]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Une fois l’étape de flux exécutée, votre personne ne sera plus un prospect dans [!DNL Salesforce], mais restera dans Marketo.

   >[!CAUTION]
   >
   >Si vous définissez **[!UICONTROL Supprimer dans Marketo]** sur **[!UICONTROL true]** et supprimez les personnes de Marketo et les prospects de Salesforce, leur annulation est définitive. Cette opération est irréversible.
