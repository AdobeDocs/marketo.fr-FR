---
unique-page-id: 4719312
description: Ajouter/Supprimer Des Valeurs De Liste De Sélection - Documents Marketo - Documentation Du Produit
title: Ajouter/supprimer des valeurs de la liste de sélection
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 3%

---

# Ajouter/supprimer des valeurs de la liste de sélection {#add-remove-picklist-values}

Voici quelques informations à connaître sur l’ajout et la suppression de valeurs de liste de sélection dans [!DNL Salesforce].

## Ajouter des valeurs de liste de sélection {#adding-picklist-values}

1. Si une valeur supplémentaire est ajoutée dans Salesforce à un type de champ de liste de sélection, vous recevrez une [notification](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"} identifiant les formulaires concernés.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Accédez à l’éditeur de formulaire et [ajoutez la valeur supplémentaire](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"} à votre liste de suggestions.

## Supprimer les valeurs de la liste de sélection {#remove-picklist-values}

Lorsqu’une valeur de liste de sélection est supprimée d’un champ dans [!DNL Salesforce], vous devez supprimer manuellement cette valeur de tous les formulaires hébergeant ce champ.

>[!NOTE]
>
>Si un champ de prospect et un champ de contact dans Salesforce ont des valeurs différentes, les valeurs en commun pourront être utilisées dans Marketo Engage.

Si un champ de prospect et un champ de contact dans [!DNL Salesforce] ont des valeurs différentes :

1. L’ajout d’une valeur supplémentaire dans SFDC à une liste de sélection génère une notification.
1. La notification vous indiquera où elle est utilisée. Vous pouvez maintenant ajouter cette nouvelle valeur en tant qu’option dans le formulaire si vous le souhaitez.

Si une liste de sélection d’un prospect SFDC comporte des valeurs différentes de celles d’une liste de sélection pour un contact SFDC, les valeurs communes seront utilisées comme options de valeur par défaut dans le formulaire.

Si vous supprimez une valeur d’une liste de sélection, vous devrez la supprimer manuellement en tant qu’option de vos formulaires.
