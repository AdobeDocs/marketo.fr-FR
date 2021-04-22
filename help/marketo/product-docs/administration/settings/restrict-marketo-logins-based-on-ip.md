---
unique-page-id: 2360297
description: Restreindre les connexions Marketo en fonction de l'adresse IP - Docs Marketo - Documentation du produit
title: Restreindre les connexions Marketo en fonction de l'adresse IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Restreindre les connexions Marketo en fonction de l&#39;adresse IP {#restrict-marketo-logins-based-on-ip}

Vous pouvez restreindre ou autoriser les utilisateurs à accéder à Marketo en fonction de leurs adresses IP. Voici comment.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Les informations de cet article s’appliquent uniquement aux connexions directes sur login.marketo.com. Il n’est pas possible pour le moment d’imposer des restrictions d’IP sur les connexions SSO (Single Sign-On).

1. Sous **Admin**, cliquez sur **Paramètres de connexion**.

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. Cliquez sur **Modifier les restrictions IP**.

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. Indiquez si vous souhaitez **Autoriser** ou **Bloquer** les adresses spécifiques, entrez la ou les adresses, puis cliquez sur **Enregistrer**.

   >[!NOTE]
   >
   >**Définition**
   >
   >* **Adresses** IP autorisées : Ajouter les adresses IP autorisées est inclusif. Elle inclura toutes les adresses IP spécifiées et exclura tout le reste.
   >* **Bloquer les adresses** IP : Empêche certaines adresses IP d’accéder à Marketo.
   >* **Désactiver les restrictions** d&#39;adresse IP : Si vous cochez cette case, toutes les règles de restriction ne fonctionneront plus. Utilisez-le à des fins de test.


   >[!NOTE]
   >
   >Vous pouvez ajouter plusieurs restrictions, mais elles peuvent uniquement être TOUTES autorisées ou TOUTES bloquées. Vous ne pouvez pas mélanger et faire correspondre autorisé et bloqué.

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   Bien joué, vos données marketing sont désormais plus sûres que jamais !
