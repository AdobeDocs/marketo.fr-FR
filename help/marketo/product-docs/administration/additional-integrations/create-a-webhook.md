---
unique-page-id: 2360360
description: Créez un [!DNL Webhook] - Documents Marketo - Documentation du produit
title: Créez un [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 6%

---

# Créez un [!DNL Webhook] {#create-a-webhook}

Utilisation [!DNL Webhooks] pour tirer parti des services web tiers pour envoyer des messages texte, développer les données de personne, etc.

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus d&#39;informations.

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/create-a-webhook-1.png)

1. Cliquez sur **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Cliquez sur **[!UICONTROL Nouveau webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Nommez et configurez vos [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Cela inclut souvent la saisie de vos informations d’identification de service tiers en tant que paramètre d’URL ou dans le modèle de POST.

   * **[!UICONTROL URL]**: Saisissez l’URL que vous utilisez dans votre requête au service Web. Pour insérer un jeton, tel que l’adresse électronique de la personne (**`{{lead.Email Address}}`**), dans votre requête, cliquez sur **[!UICONTROL Insérer un jeton]**.

   * **[!UICONTROL Modèle]**: Si vous souhaitez transmettre des informations dans le corps de la requête, saisissez depuis le modèle de payload. Modèles autorisés pour les types de requête suivants : POST, DELETE, PATCH ou PUT. Vous pouvez utiliser des formats de données tels que JSON ou XML. Pour insérer un jeton dans votre modèle, cliquez sur **[!UICONTROL Insérer un jeton]**.

   * **[!UICONTROL Encodage du jeton de demande]**: Si les valeurs de jeton incluent des caractères spéciaux (comme une esperluette, &#39;&amp;&#39;), indiquez le format de votre requête (**JSON** ou **Form/Url**).

   * **[!UICONTROL Type de réponse]**: Sélectionnez le format de la réponse que vous recevez du service (**JSON** ou **XML**).

   * **[!UICONTROL Type de requête]**: Sélectionnez la méthode HTTP à utiliser (DELETE, GET, PATCH, POST, PUT).

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>En savoir plus dans la section [[!DNL Webhooks]](https://developers.marketo.com/documentation/webhooks/){target="_blank"} plongée profonde.
