---
unique-page-id: 2360327
description: Affectation de partitions de personne avec des règles d’affectation - Documents Marketo - Documentation du produit
title: Affectation de partitions de personne avec des règles d’affectation
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
source-git-commit: 2d28d4b473815952231356691b1e9310c61a20f1
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 2%

---

# Affectation de partitions de personne avec des règles d’affectation {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!PREREQUISITES]
>
>[Création d’une partition de personne](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

Lors de l’utilisation de partitions de personne, configurez des règles d’affectation pour acheminer les personnes créées à partir de votre CRM vers leurs partitions respectives.

>[!NOTE]
>
>Seules les personnes créées dans Marketo à partir de votre CRM et via l’API SOAP auront des règles d’attribution qui leur seront appliquées.

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Cliquez sur **[!UICONTROL Espaces de travail et partitions]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. Sous , **[!UICONTROL Partitions de personne]** , cliquez sur **[!UICONTROL Règles d’affectation]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Cliquez sur **[!UICONTROL Ajouter un choix]** ajouter des conditions pour le routage des personnes dans des partitions individuelles.

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
