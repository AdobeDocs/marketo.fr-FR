---
unique-page-id: 2360297
description: Limitation des connexions Marketo en fonction de l’adresse IP - Documents Marketo - Documentation du produit
title: Limitation des connexions Marketo en fonction des adresses IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Limitation des connexions Marketo en fonction des adresses IP {#restrict-marketo-logins-based-on-ip}

Vous pouvez empêcher ou autoriser les utilisateurs d’accéder à Marketo en fonction de leurs adresses IP. Voici comment.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Les informations de cet article s’appliquent uniquement aux connexions directes sur login.marketo.com. Actuellement, il n’est pas possible d’appliquer des restrictions d’IP aux connexions par authentification unique (SSO).

1. Sous **Administration**, cliquez sur **Paramètres de connexion**.

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. Cliquez sur **Modification des restrictions IP**.

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. Choisissez si vous souhaitez **Autoriser** ou **Bloc** des adresses spécifiques, saisissez la ou les adresses, puis cliquez sur **Enregistrer**.

   >[!NOTE]
   >
   >**Définition**
   >
   >* **Adresses IP autorisées**: L’ajout d’adresses IP autorisées est inclusif. Elle inclura toutes les adresses IP spécifiées et exclura tout le reste.
   >* **Bloquer les adresses IP**: Empêche des adresses IP spécifiques d’accéder à Marketo.
   >* **Désactiver les restrictions d’IP**: Si vous cochez cette option, toutes les règles de restriction ne fonctionneront plus. Utilisez-le à des fins de test.


   >[!NOTE]
   >
   >Vous pouvez ajouter plusieurs restrictions, mais elles ne peuvent être TOUTES autorisées que ou TOUTES bloquées. Vous ne pouvez pas mélanger les éléments autorisés et bloqués.

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   Bien joué, vos données marketing sont désormais plus sûres que jamais !
