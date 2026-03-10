---
unique-page-id: 4719291
description: Découvrez comment définir le nom de famille de la personne et le nom de la société par défaut pour la synchronisation Salesforce. Utilisez les options d’administration et de synchronisation pour que les enregistrements partiels soient synchronisés avec les valeurs par défaut.
title: Définir le nom de famille et le nom de la société par défaut d’une personne
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '153'
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

Et c&#39;est ça ! Chaque fois qu’une personne n’a pas de nom et/ou de nom de société, Marketo ajoute la valeur par défaut lors de la synchronisation de l’enregistrement.
