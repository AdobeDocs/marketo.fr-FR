---
unique-page-id: 2360360
description: Création d’une  [!DNL Webhook]  - Documents Marketo - Documentation du produit
title: Créer un [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 23a7b8cb1cd07c0194c08d30218602a52d03df5b
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 1%

---

# Créer un [!DNL Webhook] {#create-a-webhook}

Utilisez [!DNL Webhooks] pour tirer parti des services web tiers pour envoyer des messages texte, développer les données de personne, etc.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-webhook-1.png)

1. Cliquez sur **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Cliquez sur **[!UICONTROL New Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Nommez et configurez votre [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Cela inclut souvent la saisie de vos informations d’identification de service tiers en tant que paramètre d’URL ou dans le modèle de POST.

   * **[!UICONTROL URL]** : saisissez l’URL que vous utilisez dans votre requête au service Web. Pour insérer un jeton, tel que l’adresse électronique de la personne (**`{{lead.Email Address}}`**), dans votre requête, cliquez sur **[!UICONTROL Insérer un jeton]**.

   * **[!UICONTROL Modèle]** : si vous souhaitez transmettre des informations dans le corps de la requête, saisissez via le modèle de payload. Modèles autorisés pour les types de requête suivants : POST, DELETE, PATCH ou PUT. Vous pouvez utiliser des formats de données tels que JSON ou XML. Pour insérer un jeton dans votre modèle, cliquez sur **[!UICONTROL Insérer un jeton]**.

   * **[!UICONTROL Encodage du jeton de demande]** : si les valeurs du jeton incluent des caractères spéciaux (tels qu’une esperluette, &#39;&amp;&#39;), indiquez le format de votre requête (**JSON** ou **Form/Url**).

   * **[!UICONTROL Type de réponse]** : sélectionnez le format de la réponse que vous recevez du service (**JSON** ou **XML**).

   * **[!UICONTROL Type de requête]** : sélectionnez la méthode HTTP à utiliser (DELETE, GET, PATCH, POST, PUT).

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Pour en savoir plus, consultez la plongée profonde [[!DNL Webhooks]](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
