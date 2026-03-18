---
unique-page-id: 14352592
description: Découvrez comment insérer des champs dynamiques dans les modèles Sales Connect. Ajoutez le prénom, la société et d’autres champs de fusion dans l’éditeur de modèles.
title: Comment insérer des champs dynamiques
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 4%

---

# Comment insérer des champs dynamiques {#how-to-insert-dynamic-fields}

Nous vous permettons de personnaliser vos modèles d’e-mail avec des attributs prédéfinis tels que `{{first_name}}` ou `{{company}}`. Ces champs vous permettent d’envoyer plusieurs e-mails à des contacts et de remplir automatiquement ces champs sans avoir à les saisir séparément pour chaque contact.

>[!TIP]
>
>Les champs « first_name » et « company » sont les seuls champs qui s’appliqueront à [!DNL Sales Connect] et [!DNL Salesforce]. Cela signifie que si un contact n’existe pas dans l’[application web](https://toutapp.com/login), nous recherchons dans [!DNL Salesforce] si nous pouvons trouver un enregistrement contact/prospect avec une adresse e-mail correspondante. Nous utilisons ensuite les informations de cet enregistrement pour remplir le champ.

## Insertion d’un champ dynamique dans un modèle {#insert-a-dynamic-field-into-a-template}

1. Dans **[!UICONTROL Modèles et campagnes]**, recherchez le modèle à modifier, puis cliquez sur **[!UICONTROL Modifier le modèle]**.

1. Cliquez sur **[!UICONTROL Tout les champs dynamiques]**.

   >[!NOTE]
   >
   >Lors de l’envoi d’e-mails à des contacts qui existent dans [!DNL Sales Connect], vous pouvez utiliser les champs dynamiques de base. Ceux-ci tireront directement du contact.

Si vous envoyez un e-mail à des contacts qui existent dans [!DNL Salesforce], vous pouvez tirer parti des champs dynamiques [!DNL Salesforce]. Tout commence par « sfdc ». Tant que vous disposez d’une connexion à [!DNL Salesforce], ces champs appellent directement le prospect/contact dans [!DNL Salesforce] pour renseigner les informations dans le modèle.

## Insertion de champs dynamiques dans une ligne d&#39;objet {#insert-dynamic-fields-in-a-subject-line}

Il vous suffit de les copier et de les coller manuellement dans le champ Objet d’un e-mail, en veillant à disposer de la mise en forme appropriée.
