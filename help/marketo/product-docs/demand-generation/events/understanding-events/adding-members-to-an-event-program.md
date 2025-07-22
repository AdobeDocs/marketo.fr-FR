---
unique-page-id: 37355758
description: Ajout de membres à un programme d’événement - Documents Marketo - Documentation du produit
title: Ajout de membres à un programme d’événement
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Ajout de membres à un programme d’événement {#adding-members-to-an-event-program}

Cet article s’applique uniquement aux utilisateurs qui utilisent la limitation d’événement ou les objectifs d’événement.

>[!CAUTION]
>
>L&#39;importation d&#39;une liste de personnes directement dans un programme d&#39;événement empêchera le comptage de ces enregistrements dans les enregistrements réels dans le rapport de suivi des objectifs et dans le rapport Progression de la limite d&#39;événement. Suivez les instructions ci-dessous pour vous assurer que vos enregistrements sont comptabilisés.

1. Créer et [ajouter des personnes à une liste statique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Créer une campagne intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Dans la liste dynamique de la campagne dynamique créée à l’étape 2, recherchez et ajoutez le filtre **[!UICONTROL Membre de la liste]**.

   ![](assets/three.png)

1. Recherchez et sélectionnez la liste que vous avez créée à l’étape 1.

   ![](assets/four.png)

1. Dans le flux, recherchez et ajoutez l’étape de flux **[!UICONTROL Modifier le statut du programme]**.

   ![](assets/five.png)

1. Recherchez et sélectionnez votre programme d’événement.

   ![](assets/six.png)

1. Choisissez le statut souhaité.

   ![](assets/seven.png)

1. Dans l’onglet [!UICONTROL Planifier], cliquez sur **[!UICONTROL Exécuter une fois]**.

   ![](assets/eight.png)

1. Sélectionnez **[!UICONTROL Exécuter maintenant]** et cliquez sur **[!UICONTROL Exécuter]**.

   ![](assets/nine.png)

1. Une fois la campagne intelligente exécutée, les membres sont ajoutés au programme et sont comptabilisés dans les calculs Suivi des objectifs et Progression de la limite d’événement .
