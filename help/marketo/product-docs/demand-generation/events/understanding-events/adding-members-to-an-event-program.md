---
unique-page-id: 37355758
description: Ajouter des membres à un Programme de Événement - Docs marketing - Documentation du produit
title: Ajouter les membres à un Programme de Événement
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Ajouter les membres à un Programme de Événement {#adding-members-to-an-event-program}

Cet article ne s&#39;applique qu&#39;aux utilisateurs qui utilisent un cap de Événement ou des objectifs de Événement.

>[!CAUTION]
>
>L&#39;importation directe d&#39;une liste de personnes dans un Programme de Événement empêche ces enregistrements d&#39;être comptabilisés dans les inscriptions réelles dans le rapport Suivi des objectifs et le rapport Progression de la limite de Événement. Suivez les instructions ci-dessous pour vous assurer que vos enregistrements sont comptabilisés.

1. Créez et [ajoutez des personnes à une liste statique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Créez une campagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) intelligente.

1. Dans la Liste intelligente du Campaign dynamique que vous avez créée à l’étape 2, recherchez et ajoutez le filtre **Membre de Liste**.

   ![](assets/three.png)

1. Recherchez et sélectionnez la liste que vous avez créée à l’étape 1.

   ![](assets/four.png)

1. Dans le flux, recherchez et ajoutez l’étape de flux **Modifier l’état du Programme**.

   ![](assets/five.png)

1. Recherchez et sélectionnez votre Programme de Événement.

   ![](assets/six.png)

1. Sélectionnez l’état de votre choix.

   ![](assets/seven.png)

1. Dans l’onglet Planification, cliquez sur **Exécuter une fois**.

   ![](assets/eight.png)

1. Sélectionnez **Exécuter maintenant** et cliquez sur **Exécuter**.

   ![](assets/nine.png)

1. Une fois la campagne intelligente exécutée, les membres sont ajoutés au programme et compteront dans le suivi des objectifs et les calculs de progression des limites de Événement.
