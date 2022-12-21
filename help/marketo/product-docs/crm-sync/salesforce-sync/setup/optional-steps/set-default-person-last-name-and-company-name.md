---
unique-page-id: 4719291
description: Définition du nom de personne par défaut et du nom de société - Documents Marketo - Documentation du produit
title: Définition du nom de personne par défaut et du nom de société
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Définition du nom de personne par défaut et du nom de société {#set-default-person-last-name-and-company-name}

Salesforce requiert (au minimum) un nom de famille et un nom de société pour ses Leads et contacts. Les enregistrements incomplets ne seront pas synchronisés avec Salesforce. Si vous souhaitez synchroniser les enregistrements partiels, vous devez définir les valeurs par défaut que Marketo doit utiliser avec Salesforce.

1. Accédez à **Administration** et cliquez sur **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Cliquez sur **Modifier les options de synchronisation**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Saisissez un **Nom de la personne par défaut** et un **Société de personnes par défaut** puis cliquez sur **Enregistrer**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo attribue une valeur par défaut uniquement lorsque l’enregistrement est initialement synchronisé avec Salesforce et uniquement si l’un des champs obligatoires est vide.

Et c&#39;est ça ! Chaque fois qu’une personne manque un nom et/ou un nom de société, Marketo ajoute la valeur par défaut lors de la synchronisation de l’enregistrement.
