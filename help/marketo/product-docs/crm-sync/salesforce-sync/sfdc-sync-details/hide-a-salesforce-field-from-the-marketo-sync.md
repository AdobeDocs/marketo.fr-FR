---
unique-page-id: 4719306
description: Découvrez comment masquer un champ Salesforce de la synchronisation Marketo pour optimiser les performances. Utilisez la sécurité au niveau du champ sur le profil utilisateur de synchronisation pour exclure les champs inutiles.
title: Masquer un champ Salesforce dans la synchronisation Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 12%

---

# Masquer un champ [!DNL Salesforce] de la synchronisation Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administration requises**

Tous les champs de Salesforce ne sont pas utiles pour le marketing. Vous pouvez optimiser les performances de synchronisation en incluant uniquement les champs dont vous avez besoin. Voici comment masquer un champ de Marketo Engage.

1. Cliquez sur le menu Nom et sélectionnez **[!UICONTROL Configuration]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Saisissez « profiles » dans la barre de recherche et cliquez sur **[!UICONTROL Profils]** sous **[!UICONTROL Gérer les utilisateurs]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Cliquez sur le profil de l’utilisateur de synchronisation.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Sous la section **[!UICONTROL Sécurité au niveau du champ]**, cliquez sur **[!UICONTROL Afficher]** en regard de l’objet qui contient le champ cible.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Décochez la case **[!UICONTROL Visible]** en regard du champ que vous souhaitez masquer. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Si le champ que vous masquez dans [!DNL Salesforce] a déjà été synchronisé avec Marketo, vous devrez également le masquer dans Marketo si vous ne souhaitez pas l’utiliser.

   Vous avez terminé. Ce champ n’apparaît plus dans Marketo une fois la synchronisation suivante terminée.

   >[!MORELIKETHIS]
   >
   >[Masquer et afficher un champ](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
