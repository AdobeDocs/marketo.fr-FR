---
unique-page-id: 2360297
description: Limiter les connexions marketing en fonction de l'adresse IP - Docs marketing - Documentation du produit
title: Limiter les connexions marketing en fonction de l'adresse IP
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Limiter les connexions marketing en fonction de l&#39;adresse IP {#restrict-marketo-logins-based-on-ip}

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
   >* **Bloquer les adresses** IP : Empêche les adresses IP spécifiques d’accéder à Marketo.
   >* **Désactiver les restrictions** d&#39;adresse IP : Si vous cochez cette case, toutes les règles de restriction ne fonctionneront plus. Utilisez-le à des fins de test.


   >[!NOTE]
   >
   >Vous pouvez ajouter plusieurs restrictions, mais elles peuvent uniquement être TOUTES autorisées ou TOUTES bloquées. Vous ne pouvez pas mélanger et faire correspondre autorisé et bloqué.

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   Bien joué, vos données marketing sont désormais plus sûres que jamais !
