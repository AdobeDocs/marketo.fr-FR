---
unique-page-id: 1147031
description: Supprimer une personne de SFDC - Documents Marketo - Documentation du produit
title: Supprimer individu de SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Supprimer individu de SFDC {#delete-person-from-sfdc}

Si vous devez supprimer un ensemble spécifique de pistes de Salesforce tout en les laissant comme des personnes en Marketo Engage, vous pouvez utiliser l’action Supprimer la personne de flux SFDC .

>[!NOTE]
>
>Disponible uniquement lorsqu’il est intégré à Salesforce.

1. Dans la base de données, cliquez sur la personne à supprimer de Salesforce. Cliquez ensuite sur **[!UICONTROL Actions de personne]** et sélectionnez **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Sélectionnez **[!UICONTROL Supprimer la personne de SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Assurez-vous que le paramètre **[!UICONTROL Supprimer dans Marketo]** est **[!UICONTROL false]**, puis cliquez sur **[!UICONTROL Exécuter maintenant]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Une fois l’étape de flux exécutée, votre personne ne sera plus une piste dans Salesforce, mais restera dans Marketo.

   >[!CAUTION]
   >
   >Si vous définissez **[!UICONTROL Supprimer dans Marketo]** sur **[!UICONTROL true]** et supprimez les personnes de Marketo et les prospects de Salesforce, elles disparaissent pour toujours. Cela ne peut pas être défait.
