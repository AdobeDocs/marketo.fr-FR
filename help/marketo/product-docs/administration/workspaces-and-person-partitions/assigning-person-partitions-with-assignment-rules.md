---
unique-page-id: 2360327
description: Affectation de partitions de personne avec des règles d’affectation - Documents Marketo - Documentation du produit
title: Affectation de partitions de personne avec des règles d’affectation
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# Affectation de partitions de personne avec des règles d’affectation {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>[Créer une partition de personne](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

Lors de l’utilisation de partitions de personne, configurez des règles d’affectation pour acheminer les personnes créées à partir de votre CRM vers leurs partitions respectives.

>[!NOTE]
>
>Seules les personnes créées dans Marketo à partir de votre CRM et via l’API SOAP auront des règles d’attribution qui leur seront appliquées.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Cliquez sur **[!UICONTROL Espaces de travail et partitions]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. Sous l’onglet **[!UICONTROL Partitions de personne]**, cliquez sur **[!UICONTROL Règles d’affectation]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Cliquez sur **[!UICONTROL Ajouter un choix]** pour ajouter des conditions de routage des personnes dans des partitions de personne.

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. Sélectionnez le champ sur lequel la condition doit être créée.

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. Choisissez l&#39;opérateur de choix et saisissez une valeur.

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. Sélectionnez la partition du peuple dans laquelle vous souhaitez que les personnes qui répondent aux conditions soient incluses.

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >Vous pouvez ajouter autant de choix que vous le souhaitez.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

Et voilà ! Vous avez défini des règles pour remplir vos partitions avec des personnes !

>[!NOTE]
>
>Le choix par défaut est appliqué si aucune des conditions précédentes n’est remplie.
