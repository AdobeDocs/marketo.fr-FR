---
unique-page-id: 4719308
description: Ajout d’un champ Salesforce existant à la synchronisation Marketo - Documents Marketo - Documentation du produit
title: Ajout d’un champ Salesforce existant à la synchronisation Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
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

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Saisissez **profile** dans la barre de recherche de gauche, puis cliquez sur **Profils** sous **Gérer les utilisateurs**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Cliquez sur le profil de l’utilisateur de synchronisation.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Dans la section **Sécurité au niveau du champ** , cliquez sur **Afficher** en regard de l’objet qui contient le champ .

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Cliquez sur **Modifier**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Cochez la case **Visible** correspondant au champ que vous souhaitez ajouter à la synchronisation, puis cliquez sur **Enregistrer**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Doux ! Lors du cycle de synchronisation suivant, Marketo voit le champ et démarre la magie.

   >[!NOTE]
   >
   > Si le champ contient déjà des valeurs dans Salesforce, celles-ci ne sont pas synchronisées avec Marketo avant la prochaine mise à jour de l’enregistrement.