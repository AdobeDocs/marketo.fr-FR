---
unique-page-id: 2360327
description: Comment configurer des règles d’affectation pour acheminer les personnes de votre CRM vers les partitions de personne appropriées.
title: Attribution de partitions de personnes avec des règles d’attribution
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
TQID: 'https://experienceleague.adobe.com/7e7A0wXFiKVttSm7BXEJYtVBnSW6qAah1ygNqO4qdr0'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b4e49ca2-9149-5443-90e6-11978bb87c2f
    internal-label: Partitions
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 10%
---
# Attribution de partitions de personnes avec des règles d’attribution {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Autorisations d’administration requises**

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

Les règles d’affectation de vos partitions de personne ont été configurées.

>[!NOTE]
>
>Le choix par défaut sera appliqué si aucune des conditions précédentes n’est remplie.
