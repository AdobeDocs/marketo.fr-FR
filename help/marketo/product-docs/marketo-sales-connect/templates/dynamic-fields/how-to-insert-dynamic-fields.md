---
unique-page-id: 14352592
description: Comment insérer des champs dynamiques - Documents Marketo - Documentation du produit
title: Comment insérer des champs dynamiques
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# Comment insérer des champs dynamiques {#how-to-insert-dynamic-fields}

Nous vous permettons de personnaliser vos modèles d&#39;email avec des attributs prédéfinis tels que `{{first_name}}` ou `{{company}}`. Ces champs vous permettent d’envoyer un email à plusieurs contacts et de les renseigner automatiquement sans avoir à les entrer séparément pour chaque contact.

>[!TIP]
>
>Les champs &quot;first_name&quot; et &quot;company&quot; sont les seuls champs qui s’afficheront à la fois pour Sales Connect et Salesforce. Cela signifie que si un contact n’existe pas dans l’ [application web](https://toutapp.com/login), nous recherchons dans Salesforce si nous pouvons trouver un enregistrement de contact/piste avec une adresse électronique correspondante. Nous utilisons ensuite les informations de cet enregistrement pour remplir le champ.

## Insertion d’un champ dynamique dans un modèle {#insert-a-dynamic-field-into-a-template}

1. Dans **Modèles et campagnes**, recherchez le modèle à modifier, puis cliquez sur **Modifier le modèle**.

1. Cliquez sur **Tout champ dynamique**.

   >[!NOTE]
   >
   >Lors de l’envoi par courrier électronique de contacts existant dans Sales Connect, vous pouvez utiliser les champs dynamiques de base. Elles proviennent directement du contact.

Si vous envoyez un courrier électronique à des contacts qui se trouvent dans Salesforce, vous pouvez tirer parti des champs dynamiques Salesforce. Tous commencent par &quot;sfdc&quot;. Tant que vous avez une connexion à Salesforce, ces champs appellent directement le prospect/contact dans Salesforce pour renseigner les informations dans le modèle.

## Insertion de champs dynamiques dans un objet {#insert-dynamic-fields-in-a-subject-line}

Il vous suffit de les copier et de les coller manuellement dans le champ d’objet d’un email, en veillant à disposer du formatage approprié.
