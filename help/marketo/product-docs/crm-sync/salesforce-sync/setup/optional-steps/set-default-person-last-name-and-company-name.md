---
unique-page-id: 4719291
description: Définition du nom de personne par défaut et du nom de société - Documents Marketo - Documentation du produit
title: Définition du nom de personne par défaut et du nom de société
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Définition du nom de personne par défaut et du nom de société {#set-default-person-last-name-and-company-name}

Salesforce requiert (au minimum) un nom de famille et un nom de société pour ses Leads et contacts. Les enregistrements incomplets ne seront pas synchronisés avec Salesforce. Si vous souhaitez synchroniser les enregistrements partiels, vous devez définir les valeurs par défaut que Marketo doit utiliser avec Salesforce.

1. Accédez à **[!UICONTROL Administration]** et cliquez sur **[!DNL Salesforce]**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Cliquez sur **[!UICONTROL Modifier les options de synchronisation]**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Saisissez un **[!UICONTROL Nom de la personne par défaut]** et un **[!UICONTROL Société de personnes par défaut]**, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage affecte uniquement une valeur par défaut lorsque l’enregistrement est initialement synchronisé avec Salesforce et uniquement si l’un des champs obligatoires est vide.

Et c&#39;est ça ! Chaque fois qu’une personne manque un nom et/ou un nom de société, Marketo ajoute la valeur par défaut lors de la synchronisation de l’enregistrement.
