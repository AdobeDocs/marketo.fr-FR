---
unique-page-id: 4719308
description: Ajout d’un champ Salesforce existant à la Synchronisation de Marketo - Documents Marketo - Documentation du produit
title: Ajout d’un champ Salesforce existant à la synchronisation Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 1%

---

# Ajout d’un champ de [!DNL Salesforce] existant à la synchronisation Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

En règle générale, les nouveaux champs personnalisés de Salesforce se synchronisent automatiquement avec Marketo Engage. Si ce n’est pas le cas, les champs peuvent ne pas être visibles pour l’utilisateur de la synchronisation Marketo. Voici comment résoudre ce problème.

1. Cliquez sur votre nom, puis sélectionnez **[!UICONTROL Configuration]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Saisissez « profile » dans la barre de recherche de gauche, puis cliquez sur **[!UICONTROL Profils]** sous **[!UICONTROL Gérer les utilisateurs]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Cliquez sur le profil de l’utilisateur de synchronisation.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Sous la section **[!UICONTROL Sécurité au niveau du champ]**, cliquez sur **[!UICONTROL Afficher]** en regard de l’objet qui contient le champ.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Cochez la case **[!UICONTROL Visible]** du champ à ajouter à la synchronisation, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Lors du prochain cycle de synchronisation, Marketo verra le champ et commencera la magie.

   >[!NOTE]
   >
   > Si le champ contient déjà des valeurs dans [!DNL Salesforce], celles-ci ne sont pas synchronisées avec Marketo avant la prochaine mise à jour de l’enregistrement.
