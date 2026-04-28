---
unique-page-id: 10098433
description: Restreindre l’accès à l’API à des adresses IP ou plages spécifiques via les restrictions IP des services Web d’administration.
title: Créer une liste autorisée pour l’accès à l’API basé sur l’adresse IP
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 12%

---

# Créer une liste autorisée pour l’accès à l’API basé sur l’adresse IP {#create-an-allowlist-for-ip-based-api-access}

Parfois, vous souhaitez accorder l’accès à l’API uniquement à une adresse IP spécifique ou à une plage d’adresses. Pour ce faire, vous devez d’abord activer les restrictions, puis spécifier les adresses IP qui sont autorisées à utiliser les API.

>[!NOTE]
>
>**Autorisations d’administration requises**

>[!CAUTION]
>
>L&#39;activation de cette fonctionnalité vous empêche d&#39;accéder au serveur MCP [Marketo](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mcp-server){target="_blank"} pour le moment. Ce problème devrait être résolu dans une prochaine version.

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
