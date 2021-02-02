---
unique-page-id: 4719291
description: Définir le nom de la personne par défaut et le nom de la Société - Documents marketing - Documentation du produit
title: Définir le nom et le nom de la Société de la personne par défaut
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# Définir le nom de la personne par défaut et le nom de la Société {#set-default-person-last-name-and-company-name}

Salesforce requiert (minimum) le nom de famille et le nom de société pour ses Pistes et Contacts. Les enregistrements incomplets ne seront pas synchronisés avec Salesforce. Si vous souhaitez synchroniser des enregistrements partiels, vous devez définir les valeurs par défaut que Marketo doit utiliser avec Salesforce.

1. Accédez à **Admin** et cliquez sur **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Cliquez sur **Modifier les options de synchronisation**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Saisissez un **nom de personne par défaut** et une **société de personne par défaut**, puis cliquez sur **Enregistrer**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo affecte uniquement une valeur par défaut lorsque l&#39;enregistrement est initialement synchronisé avec Salesforce et uniquement si l&#39;un des champs obligatoires est vide.

Et c&#39;est ça ! Chaque fois qu’une personne manque un nom de famille et/ou de société, Marketo ajoute la valeur par défaut lors de la synchronisation de l’enregistrement.
