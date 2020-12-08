---
unique-page-id: 14352592
description: Comment insérer des champs dynamiques - Documents marketing - Documentation du produit
title: Insertion de champs dynamiques
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# Insertion de champs dynamiques {#how-to-insert-dynamic-fields}

Nous vous permettons de personnaliser vos modèles de courrier électronique avec des attributs prédéfinis tels que `{{first_name}}` ou `{{company}}`. Ces champs vous permettent d’envoyer plusieurs contacts par courrier électronique et de les renseigner automatiquement sans avoir à les entrer séparément pour chaque contact.

>[!TIP]
>
>Les champs &quot;prénom&quot; et &quot;société&quot; sont les champs `only fields that will look to both Sales Connect and Salesforce.` Cela signifie que si un contact n&#39;existe pas dans l&#39;application [](http://toutapp.com/login)Web, nous recherchons dans Salesforce si nous pouvons trouver un enregistrement de contact/piste avec une adresse électronique correspondante. Nous utilisons ensuite les informations de ce dossier pour remplir le champ.

## Insérer un champ dynamique dans un modèle {#insert-a-dynamic-field-into-a-template}

1. Dans **Modèles et campagnes**, recherchez le modèle à modifier, puis cliquez sur **Modifier le modèle**.
1. Cliquez sur **Tout champ** dynamique.

   >[!NOTE]
   >
   >Lors de l&#39;envoi par courriel de contacts qui existent dans Sales Connect, vous pouvez utiliser les champs dynamiques de base. Ils vont tirer directement du contact.

Si vous envoyez un courriel à des contacts qui existent dans Salesforce, vous pouvez tirer parti des champs dynamiques Salesforce. Tous ces éléments commencent par &quot;sfdc&quot;. Tant que vous disposez d&#39;une connexion à Salesforce, ces champs appellent directement le responsable/contact de Salesforce pour renseigner les informations du modèle.

## Insérer des champs dynamiques dans une ligne d&#39;objet {#insert-dynamic-fields-in-a-subject-line}

Il vous suffit de les copier et de les coller manuellement dans le champ d&#39;objet d&#39;un courriel, en veillant à ce que vous disposiez de la mise en forme appropriée.
