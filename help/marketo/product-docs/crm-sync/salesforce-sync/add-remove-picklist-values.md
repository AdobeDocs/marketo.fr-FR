---
unique-page-id: 4719312
description: Ajouter/supprimer des valeurs de liste d'achat - Documents Marketo - Documentation sur les produits
title: Ajouter/supprimer des valeurs de liste de sélection
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Ajouter/supprimer des valeurs de liste d&#39;achat {#add-remove-picklist-values}

Vous trouverez ci-dessous quelques informations sur l’ajout et la suppression de valeurs de liste de sélection dans Salesforce.

## Ajouter les valeurs de liste de sélection {#adding-picklist-values}

1. Si une valeur supplémentaire est ajoutée dans Salesforce à un type de champ de liste de sélection, vous recevrez une [notification](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) identifiant les formulaires concernés.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Accédez à l’éditeur de formulaire et [ajoutez la valeur supplémentaire ](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) à votre liste de suggestions.

## Supprimer les valeurs de liste d&#39;achat {#remove-picklist-values}

Lorsqu&#39;une valeur de liste de sélection est supprimée d&#39;un champ de Salesforce, vous devez la supprimer manuellement de tous les formulaires qui hébergent ce champ.

>[!NOTE]
>
>Si un champ de piste et un champ de contact dans Salesforce ont des valeurs différentes, les valeurs en commun seront disponibles pour utilisation dans Marketo.

Si un champ de piste et un champ de contact dans Salesforce ont des valeurs différentes :

1. Si vous Ajoutez une valeur supplémentaire dans la collecte de données régionale à une liste de sélection, une notification vous sera envoyée.
1. La notification vous indiquera où elle est utilisée. Vous pouvez désormais ajouter cette nouvelle valeur en tant qu’option sur le formulaire si vous le souhaitez.

Si une liste de sélection d&#39;une piste SFDC contient des valeurs différentes de celles d&#39;une liste de sélection pour un contact SFDC, les valeurs communes seront utilisées comme options de valeur par défaut dans le formulaire.

Si vous supprimez une valeur d’une liste de sélection, vous devrez la supprimer manuellement en tant qu’option de vos formulaires.
