---
unique-page-id: 4719306
description: Masquer un champ Salesforce de la synchronisation du marché - Docs marketing - Documentation du produit
title: Masquer un champ Salesforce de la synchronisation du marketing
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---


# Masquer un champ Salesforce de la synchronisation du marché {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Tous les champs de Salesforce ne sont pas utiles pour le marketing. Vous pouvez optimiser les performances de synchronisation en incluant uniquement les champs dont vous avez besoin. Voici comment vous pouvez masquer un champ de Marketo.

1. Cliquez sur le menu de votre nom et sélectionnez **Configuration**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Saisissez **profils** dans la barre de recherche et cliquez sur **Profils** sous **Gérer les utilisateurs**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Cliquez sur le profil de l’utilisateur de synchronisation.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Sous la section **Sécurité au niveau du champ**, cliquez sur **Vue** en regard de l’objet qui contient le champ de cible.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Cliquez sur **Modifier**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Décochez la case **Visible** en regard du champ à masquer. Cliquez sur **Enregistrer**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Si le champ que vous masquez dans Salesforce a déjà été synchronisé avec Marketo, vous devrez également le masquer dans Marketo, si vous ne souhaitez pas l’utiliser.

   C&#39;est tout ! Vous ne verrez plus ce champ dans Marketo une fois la synchronisation suivante terminée.

   >[!NOTE]
   >
   >**Articles connexes**
   >
   >    
   >    
   >    * [Masquer et afficher un champ](../../../../../product-docs/administration/field-management/hide-and-unhide-a-field.md)


