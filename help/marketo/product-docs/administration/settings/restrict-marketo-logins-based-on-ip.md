---
unique-page-id: 2360297
description: Limitation des connexions Marketo en fonction de l’adresse IP - Documents Marketo - Documentation du produit
title: Limitation des connexions Marketo en fonction des adresses IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Limitation des connexions Marketo en fonction des adresses IP {#restrict-marketo-logins-based-on-ip}

Vous pouvez empêcher ou autoriser les utilisateurs d’accéder à Marketo en fonction de leurs adresses IP. Voici comment.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Les informations de cet article s’appliquent uniquement aux connexions directes sur login.marketo.com. Actuellement, il n’est pas possible d’appliquer des restrictions d’IP aux connexions par authentification unique (SSO).

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Cliquez sur **[!UICONTROL Paramètres de connexion]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Cliquez sur **[!UICONTROL Modification des restrictions IP]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Choisissez si vous souhaitez **Autoriser** ou **Bloc** des adresses spécifiques, saisissez la ou les adresses, puis cliquez sur **[!UICONTROL Enregistrer]**.

   >[!NOTE]
   >
   >**Définition**
   >
   >* **[!UICONTROL Adresses IP autorisées]**: L’ajout d’adresses IP autorisées est inclusif. Elle inclura toutes les adresses IP spécifiées et exclura tout le reste.
   >* **[!UICONTROL Bloquer les adresses IP]**: Empêche des adresses IP spécifiques d’accéder à Marketo.
   >* **[!UICONTROL Désactiver les restrictions d’IP]**: Si vous cochez cette option, toutes les règles de restriction ne fonctionneront plus. Utilisez-le à des fins de test.

   >[!NOTE]
   >
   >Vous pouvez ajouter plusieurs restrictions, mais elles ne peuvent être TOUTES autorisées que ou TOUTES bloquées. Vous ne pouvez pas mélanger les éléments autorisés et bloqués.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Bien joué, vos données marketing sont désormais plus sûres que jamais !
