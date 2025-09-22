---
unique-page-id: 2360297
description: Restreindre les connexions Marketo en fonction de l’adresse IP - Documents Marketo - Documentation du produit
title: Restreindre les connexions à Marketo en fonction de l’adresse IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 7%

---

# Restreindre les connexions à Marketo en fonction de l’adresse IP {#restrict-marketo-logins-based-on-ip}

Vous pouvez empêcher ou autoriser des utilisateurs à accéder à Marketo en fonction de leurs adresses IP. Voici comment faire.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!IMPORTANT]
>
>Les informations contenues dans cet article sont destinées aux utilisateurs qui se connectent directement à login.marketo.com et ne s’appliquent pas à ceux qui s’authentifient avec Adobe ID. Il n’est pas possible d’appliquer des restrictions IP sur les connexions d’authentification unique (SSO) pour le moment.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Cliquez sur **[!UICONTROL Paramètres de connexion]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Cliquez sur **[!UICONTROL Modifier les restrictions IP]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Choisissez si vous souhaitez **Autoriser** ou **Bloquer** des adresses spécifiques, saisissez la ou les adresses, puis cliquez sur **[!UICONTROL Enregistrer]**.

   >[!NOTE]
   >
   >**Définition**
   >
   >* **[!UICONTROL Adresses IP autorisées]** : l’ajout d’adresses IP autorisées est un processus d’inclusion. Elle inclut toutes les adresses IP spécifiées et exclut tout le reste.
   >* **[!UICONTROL Bloquer les adresses IP]** : empêche des adresses IP spécifiques d’accéder à Marketo.
   >* **[!UICONTROL Désactiver les restrictions IP]** : si vous cochez cette case, toutes les règles de restriction cesseront de fonctionner. Utilisez-le à des fins de test.

   >[!NOTE]
   >
   >Vous pouvez ajouter plusieurs restrictions, mais elles peuvent uniquement être AUTORISÉES POUR TOUT ou BLOQUÉES POUR TOUT. Vous ne pouvez pas mélanger et faire correspondre les valeurs autorisées et bloquées.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Bien joué, vos données marketing sont maintenant plus sûres qu&#39;elles ne l&#39;ont jamais été !
