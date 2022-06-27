---
unique-page-id: 2360360
description: Création d’un webhook - Documents Marketo - Documentation du produit
title: Création d’un webhook
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 25a574719eb6c064d33b6a1cebafe2668ed1330d
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 3%

---

# Création d’un webhook {#create-a-webhook}

Utilisez des webhooks pour tirer parti des services web tiers afin d’envoyer des messages texte, de développer les données de personne, etc.

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus d&#39;informations.

1. Accédez à **Administration** et cliquez sur **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Cliquez sur **Nouveau webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Nommez et configurez votre webhook.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Cela inclut souvent la saisie de vos informations d’identification de service tiers en tant que paramètre d’URL ou dans le modèle de POST.

   * **URL**: Saisissez l’URL que vous utilisez dans votre requête au service Web. Pour insérer un jeton, tel que l’adresse électronique de la personne (**`{{lead.Email Address}}`**), dans votre requête, cliquez sur **Insérer un jeton**.

   * **Modèle**: Si vous souhaitez transmettre des informations dans le corps du POST, saisissez le modèle. Utilisez n’importe quel format de données prenant en charge le POST HTTP, y compris XML, JSON ou SOAP. Pour insérer un jeton dans votre modèle, cliquez sur **Insérer un jeton**.

   * **Encodage du jeton de demande**: Si les valeurs de jeton incluent des caractères spéciaux (comme une esperluette, &#39;&amp;&#39;), indiquez le format de votre requête (**JSON** ou **Form/Url**).

   * **Type de réponse**: Sélectionnez le format de la réponse que vous recevez du service (**JSON** ou **XML**).

   * **Type de requête**: Sélectionnez la méthode HTTP à utiliser (DELETE, GET, PATCH, POST, PUT).

   Cliquez sur **Créer**.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>En savoir plus dans la section [webhooks](https://developers.marketo.com/documentation/webhooks/) plongée profonde.
