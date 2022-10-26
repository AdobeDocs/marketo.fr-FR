---
unique-page-id: 4719308
description: Ajout d’un champ Salesforce existant à la synchronisation Marketo - Documents Marketo - Documentation du produit
title: Ajout d’un champ Salesforce existant à la synchronisation Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 81bc90bcccc8073511c9f331471c0cda9f4147cb
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Ajout d’un champ Salesforce existant à la synchronisation Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

En règle générale, les nouveaux champs personnalisés de Salesforce sont automatiquement synchronisés avec Marketo. Dans le cas contraire, les champs peuvent ne pas être visibles par l’utilisateur de synchronisation Marketo. Voici comment vous pouvez réparer ceci.

1. Cliquez sur votre nom, puis sélectionnez **Configuration**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Entrée **profile** dans la barre de recherche de gauche, puis cliquez sur **Profils** under **Gestion des utilisateurs**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Cliquez sur le profil de l’utilisateur de synchronisation.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Sous , **Sécurité au niveau du champ** , cliquez sur **Affichage** en regard de l’objet qui contient le champ .

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Cliquez sur **Modifier**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Vérifiez les **Visible** pour le champ que vous souhaitez ajouter à la synchronisation, puis cliquez sur **Enregistrer**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Doux ! Lors du cycle de synchronisation suivant, Marketo voit le champ et démarre la magie.

   >[!NOTE]
   >
   > Si le champ contient déjà des valeurs dans Salesforce, celles-ci ne sont pas synchronisées avec Marketo avant la prochaine mise à jour de l’enregistrement.
