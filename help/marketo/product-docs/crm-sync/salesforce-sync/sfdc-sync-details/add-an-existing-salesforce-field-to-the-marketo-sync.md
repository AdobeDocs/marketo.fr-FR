---
unique-page-id: 4719308
description: Découvrez comment ajouter un champ Salesforce existant à la synchronisation Marketo. Rendez le champ visible par l’utilisateur de la synchronisation dans Salesforce afin qu’il se synchronise lors du cycle suivant.
title: Ajouter un champ Salesforce existant à la synchronisation Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/Vb-1DhNwUPQSPYuCkVzzSDDqWd4tvO-XoPhXn58hj6E
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 173
ht-degree: 8%

---

# Ajout d’un champ de [!DNL Salesforce] existant à la synchronisation Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administration requises**

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
