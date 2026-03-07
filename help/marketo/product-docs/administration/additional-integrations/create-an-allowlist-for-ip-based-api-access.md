---
unique-page-id: 10098433
description: Restreindre l’accès à l’API à des adresses IP ou plages spécifiques via les restrictions IP des services Web d’administration.
title: Créer une liste autorisée pour l’accès à l’API basé sur l’adresse IP
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 11%

---

# Créer une liste autorisée pour l’accès à l’API basé sur l’adresse IP {#create-an-allowlist-for-ip-based-api-access}

Parfois, vous souhaitez accorder l’accès à l’API uniquement à une adresse IP spécifique ou à une plage d’adresses. Pour ce faire, vous devez d’abord activer les restrictions, puis spécifier les adresses IP qui sont autorisées à utiliser les API.

>[!NOTE]
>
>**Autorisations d’administration requises**

>[!NOTE]
>
>Cette fonctionnalité fonctionne indépendamment des restrictions de connexion basées sur l’adresse IP [Marketo Engage](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} qui sont remplacées par le contrôle d’accès basé sur l’adresse IP [Admin Console](https://helpx.adobe.com/fr/enterprise/using/ip-based-access.html){target="_blank"}. Il continuera à fonctionner en l’état après la migration d’Adobe IMS.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-1.png)

1. Cliquez sur **[!UICONTROL Services web]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-2.png)

1. Dans la zone **[!UICONTROL Restrictions IP]**, cliquez sur **[!UICONTROL Modifier],** ou cliquez sur **[!UICONTROL Modifier les restrictions IP]** dans le coin supérieur gauche.

   ![](assets/create-an-allowlist-for-ip-based-api-access-3.png)

1. Cochez la case **[!UICONTROL Activer les restrictions IP]** et saisissez les adresses IP à Placer sur la liste autorisée.

   ![](assets/create-an-allowlist-for-ip-based-api-access-4.png)

   >[!NOTE]
   >
   >Vous pouvez saisir une seule adresse IP ou une plage d’adresses IP, ou utiliser un caractère générique.

1. Cliquez sur **[!UICONTROL Ajouter]** pour ouvrir des champs supplémentaires et saisir d’autres adresses IP.

   ![](assets/create-an-allowlist-for-ip-based-api-access-5.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/create-an-allowlist-for-ip-based-api-access-6.png)
