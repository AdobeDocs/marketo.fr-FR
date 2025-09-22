---
unique-page-id: 2360327
description: Affectation de partitions de personne avec des règles d’affectation - Documents Marketo - Documentation du produit
title: Affectation de partitions de personne avec des règles d’affectation
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 8%

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
>Seules les personnes créées dans Marketo à partir de votre CRM et via l’API SOAP se verront appliquer des règles d’affectation.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Cliquez sur **[!UICONTROL Workspaces et partitions]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. Sous l’onglet **[!UICONTROL Partitions de personne]**, cliquez sur **[!UICONTROL Règles d’affectation]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Cliquez sur **[!UICONTROL Ajouter un choix]** pour ajouter des conditions de routage des personnes dans des partitions de personne.

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. Sélectionnez le champ sur lequel la condition doit être créée.

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. Choisissez l’opérateur de choix et saisissez une valeur.

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. Sélectionnez la partition des personnes dans laquelle vous souhaitez que les personnes qui remplissent les conditions entrent.

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >Vous pouvez ajouter autant de choix que vous le souhaitez.

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

Et voilà ! Vous avez affecté des règles pour remplir vos partitions de personne avec des personnes !

>[!NOTE]
>
>Le choix par défaut sera appliqué si aucune des conditions précédentes n’est remplie.
