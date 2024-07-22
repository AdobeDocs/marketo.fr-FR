---
unique-page-id: 4719312
description: Ajout/suppression de valeurs de liste de sélection - Documents Marketo - Documentation du produit
title: Ajout/suppression de valeurs de liste de sélection
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# Ajout/suppression de valeurs de liste de sélection {#add-remove-picklist-values}

Voici quelques éléments à savoir sur l’ajout et la suppression de valeurs de liste de sélection dans Salesforce.

## Ajout de valeurs de liste de sélection {#adding-picklist-values}

1. Si une valeur supplémentaire est ajoutée dans Salesforce à un type de champ de liste de sélection, vous recevrez une [notification](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"} identifiant les formulaires qui seront affectés.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Accédez à l’éditeur de formulaire et [ajoutez la valeur supplémentaire](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"} à votre liste de suggestions.

## Supprimer les valeurs de liste de sélection {#remove-picklist-values}

Lorsqu’une valeur de liste de sélection est supprimée d’un champ dans Salesforce, vous devez supprimer manuellement cette valeur de tous les formulaires hébergeant ce champ.

>[!NOTE]
>
>Si un champ de piste et un champ de contact dans Salesforce ont des valeurs différentes, les valeurs communes pourront être utilisées en Marketo Engage.

Si un champ de piste et un champ de contact dans Salesforce ont des valeurs différentes :

1. L’ajout d’une valeur supplémentaire dans SFDC à une liste de sélection recevra une notification.
1. La notification vous indique où elle est utilisée. Vous pouvez maintenant ajouter cette nouvelle valeur comme option sur le formulaire si vous le souhaitez.

Si une liste de sélection d’un prospect SFDC a des valeurs différentes d’une liste de sélection pour un contact SFDC, les valeurs communes seront utilisées comme options de valeur par défaut dans le formulaire.

Si vous supprimez une valeur d’une liste de sélection, vous devrez la supprimer manuellement en tant qu’option de vos formulaires.
