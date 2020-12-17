---
unique-page-id: 4719308
description: Ajouter un champ Salesforce existant à la synchronisation du marché - Docs marketing - Documentation du produit
title: Ajouter un champ Salesforce existant à la synchronisation du marché
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Ajouter un champ Salesforce existant à la synchronisation du marché {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

En règle générale, les nouveaux champs personnalisés de Salesforce sont automatiquement synchronisés sur Marketo. Si ce n’est pas le cas, les champs peuvent ne pas être visibles par l’utilisateur de synchronisation du marketing. Voici comment vous pouvez réparer ceci.

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
   > Si le champ contient déjà des valeurs dans Salesforce, celles-ci ne sont pas synchronisées avec Marketo avant la prochaine mise à jour de l&#39;enregistrement.

