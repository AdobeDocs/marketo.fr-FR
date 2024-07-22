---
unique-page-id: 4719308
description: Ajouter un champ Salesforce existant à la synchronisation Marketo - Documents Marketo - Documentation du produit
title: Ajout d’un champ Salesforce existant à la synchronisation Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Ajout d’un champ Salesforce existant à la synchronisation Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

En règle générale, les nouveaux champs personnalisés dans Salesforce sont automatiquement synchronisés dans Marketo Engage. Si ce n’est pas le cas, les champs peuvent ne pas être visibles par l’utilisateur de synchronisation Marketo. Voici comment vous pouvez réparer ceci.

1. Cliquez sur votre nom, puis sélectionnez **[!UICONTROL Setup]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Saisissez &quot;profile&quot; dans la barre de recherche de gauche, puis cliquez sur **[!UICONTROL Profils]** sous **[!UICONTROL Gérer les utilisateurs]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Cliquez sur le profil de l’utilisateur de synchronisation.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Dans la section **[!UICONTROL Sécurité au niveau du champ]**, cliquez sur **[!UICONTROL Afficher]** en regard de l’objet qui contient le champ.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Cochez la case **[!UICONTROL Visible]** pour le champ que vous souhaitez ajouter à la synchronisation et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Lors du cycle de synchronisation suivant, Marketo voit le champ et démarre la magie.

   >[!NOTE]
   >
   > Si le champ contient déjà des valeurs dans Salesforce, celles-ci ne sont pas synchronisées avec Marketo tant que l’enregistrement suivant n’est pas mis à jour.
