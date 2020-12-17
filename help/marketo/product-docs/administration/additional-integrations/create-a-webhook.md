---
unique-page-id: 2360360
description: Création d’un crochet Web - Documents marketing - Documentation du produit
title: Création d’un crochet Web
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Créer un crochet Web {#create-a-webhook}

Utilisez des hameçons Web pour tirer parti des services Web tiers pour envoyer des messages texte, développer les données personnelles, etc.

>[!NOTE]
>
>**Disponibilité**
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus de détails.

1. Accédez à **Admin **et cliquez sur **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Cliquez sur **New Webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Nommez et configurez votre webhook.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Cela inclut souvent la saisie de vos informations d’identification de service tiers en tant que paramètre d’URL ou dans le modèle de POST.

   * **URL** : Entrez l’URL que vous utilisez pour POST votre demande au service Web. Pour insérer un jeton, tel que l’adresse électronique de la personne (**`{{lead.Email Address}}`**), dans votre requête, cliquez sur **Insérer un jeton**.

   * **Modèle** : Si vous souhaitez transmettre des informations dans le corps du POST, entrez le modèle. Utilisez tout format de données prenant en charge le POST HTTP, y compris XML, JSON ou SOAP. Pour insérer un jeton dans votre modèle, cliquez sur **Insérer un jeton**.

   * **Encodage** du jeton de demande : Si les valeurs de jeton comportent des caractères spéciaux (par exemple une esperluette, &quot;&amp;&quot;), indiquez le format de votre requête (**** JSONou  **Form/Url**).

   * **Type** de réponse : Sélectionnez le format de la réponse que vous recevez du service (**** JSONou  **XML**).

   Cliquez sur Créer.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>**Plongée profonde**
>
>Pour en savoir plus, consultez les [webhooks](http://developers.marketo.com/documentation/webhooks/) plongée profonde.

