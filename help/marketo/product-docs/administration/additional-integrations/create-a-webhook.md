---
unique-page-id: 2360360
description: Créez un webhook dans Admin pour appeler des services web tiers pour les SMS, les données de personne, etc.
title: Créer un  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
TQID: https://experienceleague.adobe.com/O4xw1wSvFeTJ2xqZn4Eo7JbrUBQQmKcl7mvLkduFXGc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 220
ht-degree: 0%

---

# Création d’un [!DNL Webhook] {#create-a-webhook}

Utilisez [!DNL Webhooks] pour tirer parti des services web tiers afin d’envoyer des SMS, de développer les données de personne, etc.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-webhook-1.png)

1. Cliquez sur **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Cliquez sur **[!UICONTROL Nouveau Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Nommez et configurez votre [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Cela inclut souvent la saisie de vos informations d’identification de service tierces en tant que paramètre d’URL ou dans le modèle POST.

   * **[!UICONTROL URL]** : saisissez l’URL que vous utilisez dans votre demande de service web. Pour insérer un jeton, tel que l’adresse e-mail de la personne (**`{{lead.Email Address}}`**), dans votre demande, cliquez sur **[!UICONTROL Insérer un jeton]**.

   * **[!UICONTROL Modèle]** : si vous souhaitez transmettre des informations dans le corps de la requête, saisissez via le modèle de payload. Modèles autorisés pour les types de requête suivants : POST, DELETE, PATCH ou PUT. Vous pouvez utiliser des formats de données tels que JSON ou XML. Pour insérer un jeton dans votre modèle, cliquez sur **[!UICONTROL Insérer un jeton]**.

   * **[!UICONTROL Encodage du jeton de demande]** : si les valeurs du jeton incluent des caractères spéciaux (par exemple une esperluette, «&amp; »), indiquez le format de votre demande (**JSON** ou **Formulaire/Url**).

   * **[!UICONTROL Type de réponse]** : sélectionnez le format de la réponse que vous recevez du service (**JSON** ou **XML**).

   * **[!UICONTROL Type de requête]** : sélectionnez la méthode HTTP à utiliser (DELETE, GET, PATCH, POST, PUT).

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>En savoir plus dans l’exploration approfondie de [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
