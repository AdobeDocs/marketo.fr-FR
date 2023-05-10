---
unique-page-id: 2360360
description: Création d’un webhook - Documents Marketo - Documentation du produit
title: Création d’un webhook
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: a498dcc5dc95bd7f732481d30db021485cf052c0
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 5%

---

# Création d’un webhook {#create-a-webhook}

Utilisez des webhooks pour tirer parti des services web tiers afin d’envoyer des messages texte, de développer les données de personne, etc.

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus d&#39;informations.

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/create-a-webhook-1.png)

1. Cliquez sur **Webhooks**.

   ![](assets/create-a-webhook-2.png)

1. Cliquez sur **Nouveau webhook**.

   ![](assets/create-a-webhook-3.png)

1. Nommez et configurez votre webhook.

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Cela inclut souvent la saisie de vos informations d’identification de service tiers en tant que paramètre d’URL ou dans le modèle de POST.

   * **URL**: Saisissez l’URL que vous utilisez dans votre requête au service Web. Pour insérer un jeton, tel que l’adresse électronique de la personne (**`{{lead.Email Address}}`**), dans votre requête, cliquez sur **Insérer un jeton**.

   * **Modèle**: Si vous souhaitez transmettre des informations dans le corps de la requête, saisissez depuis le modèle de payload. Modèles autorisés pour les types de requête suivants : POST, DELETE, PATCH ou PUT. Vous pouvez utiliser des formats de données tels que JSON ou XML. Pour insérer un jeton dans votre modèle, cliquez sur **Insérer un jeton**.

   * **Encodage du jeton de demande**: Si les valeurs de jeton incluent des caractères spéciaux (comme une esperluette, &#39;&amp;&#39;), indiquez le format de votre requête (**JSON** ou **Form/Url**).

   * **Type de réponse**: Sélectionnez le format de la réponse que vous recevez du service (**JSON** ou **XML**).

   * **Type de requête**: Sélectionnez la méthode HTTP à utiliser (DELETE, GET, PATCH, POST, PUT).

1. Cliquez sur **Créer**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>En savoir plus dans la section [webhooks](https://developers.marketo.com/documentation/webhooks/) plongée profonde.
