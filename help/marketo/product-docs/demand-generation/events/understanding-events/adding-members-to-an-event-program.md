---
unique-page-id: 37355758
description: Ajout de membres à un programme d’événements - Documents Marketo - Documentation du produit
title: Ajout de membres à un programme d’événement
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Ajout de membres à un programme d’événement {#adding-members-to-an-event-program}

Cet article s’applique uniquement aux utilisateurs qui utilisent la limite d’événements ou les objectifs d’événement.

>[!CAUTION]
>
>L’importation d’une liste de personnes directement dans un programme d’événements empêche ces enregistrements d’être comptabilisés dans les inscriptions réelles dans le rapport Suivi des objectifs et dans le rapport Progression de la limite de l’événement . Suivez les instructions ci-dessous pour vous assurer que vos enregistrements sont comptabilisés.

1. Créez et [ajoutez des personnes à une liste statique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Créez une campagne dynamique ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Dans la liste dynamique de la campagne dynamique que vous avez créée à l’étape 2, recherchez et ajoutez le filtre **Membre de la liste** .

   ![](assets/three.png)

1. Recherchez et sélectionnez la liste que vous avez créée à l’étape 1.

   ![](assets/four.png)

1. Dans Flux, recherchez et ajoutez l’étape de flux **Modifier l’état du programme** .

   ![](assets/five.png)

1. Recherchez et sélectionnez votre programme d’événements.

   ![](assets/six.png)

1. Sélectionnez l’état de votre choix.

   ![](assets/seven.png)

1. Dans l’onglet Planning , cliquez sur **Exécuter une fois**.

   ![](assets/eight.png)

1. Sélectionnez **Run Now** et cliquez sur **Run**.

   ![](assets/nine.png)

1. Une fois la campagne dynamique exécutée, les membres sont ajoutés au programme et compteront dans les calculs Suivi des objectifs et Progression de la limite des événements .
