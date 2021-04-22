---
unique-page-id: 4719306
description: Masquer un champ Salesforce dans Marketo Sync - Marketo Docs - Documentation du produit
title: Masquer un champ Salesforce de la synchronisation Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Masquer un champ Salesforce de la synchronisation Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Tous les champs de Salesforce ne sont pas utiles pour le marketing. Vous pouvez optimiser les performances de synchronisation en incluant uniquement les champs dont vous avez besoin. Voici comment vous pouvez cacher un champ à Marketo.

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
   >Si le champ que vous masquez dans Salesforce a déjà été synchronisé avec Marketo, vous devrez également le masquer dans Marketo, si vous ne voulez pas l&#39;utiliser.

   C&#39;est tout ! Vous ne verrez plus ce champ dans Marketo une fois la synchronisation suivante terminée.

   >[!MORELIKETHIS]
   >
   >[Masquer et afficher un champ](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
