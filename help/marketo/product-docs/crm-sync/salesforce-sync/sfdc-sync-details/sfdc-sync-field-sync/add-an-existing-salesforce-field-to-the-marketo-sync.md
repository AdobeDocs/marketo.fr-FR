---
unique-page-id: 4719308
description: Ajouter un champ Salesforce existant à Marketo Sync - Marketo Docs - Documentation du produit
title: Ajouter un champ Salesforce existant à la synchronisation Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Ajouter un champ Salesforce existant à la synchronisation Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

En général, les nouveaux champs personnalisés de Salesforce sont automatiquement synchronisés sur Marketo. Dans le cas contraire, les champs peuvent ne pas être visibles par l’utilisateur Marketo Sync. Voici comment vous pouvez réparer ceci.

1. Cliquez sur votre nom, puis sélectionnez **Configuration**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Saisissez **profil** dans la barre de recherche de gauche et cliquez sur **Profils** sous **Gérer les utilisateurs**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Cliquez sur le profil de l’utilisateur de synchronisation.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Sous la section **Sécurité au niveau du champ**, cliquez sur **Vue** en regard de l’objet qui contient le champ.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Cliquez sur **Modifier**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Cochez la case **Visible** correspondant au champ que vous souhaitez ajouter à la synchronisation et cliquez sur **Enregistrer**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Doux ! Lors du prochain cycle de synchronisation, Marketo verra le champ et début la magie.

   >[!NOTE]
   >
   > Si le champ contient déjà des valeurs dans Salesforce, celles-ci ne sont synchronisées sur Marketo qu&#39;après la prochaine mise à jour de l&#39;enregistrement.
