---
unique-page-id: 4719306
description: Masquer un champ Salesforce de la synchronisation Marketo - Documents Marketo - Documentation du produit
title: Masquer un champ Salesforce de la synchronisation Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# Masquer un champ Salesforce de la synchronisation Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Tous les champs de Salesforce ne sont pas utiles pour le marketing. Vous pouvez optimiser les performances de synchronisation en incluant uniquement les champs dont vous avez besoin. Voici comment masquer un champ du Marketo Engage.

1. Cliquez sur le menu de votre nom et sélectionnez **[!UICONTROL Configuration]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Saisissez &quot;profiles&quot; dans la barre de recherche, puis cliquez sur **[!UICONTROL Profiles]** sous **[!UICONTROL Gérer les utilisateurs]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Cliquez sur le profil de l’utilisateur de synchronisation.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Dans la section **[!UICONTROL Sécurité au niveau du champ]**, cliquez sur **[!UICONTROL Afficher]** en regard de l’objet qui contient le champ cible.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Décochez la case **[!UICONTROL Visible]** en regard du champ que vous souhaitez masquer. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Si le champ que vous masquez dans Salesforce a déjà été synchronisé avec Marketo, vous devrez également le masquer dans Marketo si vous ne souhaitez pas l’utiliser.

   C&#39;est tout ! Vous ne verrez plus ce champ dans Marketo une fois la synchronisation suivante terminée.

   >[!MORELIKETHIS]
   >
   >[Masquer et afficher un champ](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
