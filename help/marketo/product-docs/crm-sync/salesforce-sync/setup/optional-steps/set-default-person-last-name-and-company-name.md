---
unique-page-id: 4719291
description: Découvrez comment définir le nom de famille de la personne et le nom de la société par défaut pour la synchronisation Salesforce. Utilisez les options d’administration et de synchronisation pour que les enregistrements partiels soient synchronisés avec les valeurs par défaut.
title: Définir le nom de famille et le nom de la société par défaut d’une personne
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/pq4XPfiwO1UemSmg3edhJgWWmvR-mx4Q3udff9xzWt0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 10%

---

# Définir le nom de famille et le nom de la société par défaut d’une personne {#set-default-person-last-name-and-company-name}

[!DNL Salesforce] nécessite (au minimum) le nom et le nom de la société pour ses leads et contacts. Les enregistrements incomplets ne seront pas synchronisés avec [!DNL Salesforce]. Si vous souhaitez synchroniser les enregistrements partiels, vous devez définir les valeurs par défaut que Marketo doit utiliser avec [!DNL Salesforce].

1. Accédez à **[!UICONTROL Admin]** et cliquez sur **[!DNL Salesforce]**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Cliquez sur **[!UICONTROL Modifier les options de synchronisation]**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Saisissez un **[!UICONTROL Nom de personne par défaut]** et un **[!UICONTROL Société par défaut]**, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage n’affecte une valeur par défaut que lorsque l’enregistrement est initialement synchronisé avec Salesforce et uniquement si l’un des champs obligatoires est vide.

Chaque fois qu&#39;une personne n&#39;a pas de nom ou de nom de société, Marketo ajoute la valeur par défaut lors de la synchronisation de l&#39;enregistrement.
