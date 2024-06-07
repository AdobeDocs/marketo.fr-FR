---
unique-page-id: 2949962
description: Activer/désactiver dynamiquement la visibilité d’un champ de formulaire - Documents Marketo - Documentation du produit
title: Activer/désactiver dynamiquement la visibilité d’un champ de formulaire
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 1%

---

# Activer/désactiver dynamiquement la visibilité d’un champ de formulaire {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Ajout d’une liste de pays à votre formulaire](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

L’une des fonctionnalités les plus intéressantes des formulaires Marketo est que vous pouvez masquer/afficher dynamiquement des champs de formulaire ou [fieldsets](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exemple**
>
>Dans cet exemple, masquons la variable **État** Champ sauf **Pays** est sélectionné comme &quot;États-Unis&quot;.

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities-8.png)

1. Sélectionnez votre formulaire et cliquez sur **Modifier le formulaire**.

   ![](assets/editform-1.png)

1. Sélectionnez le champ à masquer/afficher dynamiquement, puis cliquez sur le lien pour **Règles de visibilité**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Recherchez et sélectionnez le champ sur lequel vous souhaitez créer une condition.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Sélectionnez l’opérateur.

   >[!TIP]
   >
   >C&#39;est cool parce que vous pouvez choisir des allumettes floues comme &quot;commence par&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Sélectionnez la ou les valeurs à rechercher, puis cliquez en dehors de la liste déroulante.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Vous pouvez sélectionner plusieurs valeurs en cliquant dessus lorsque la liste déroulante est ouverte. Par exemple, vous pouvez sélectionner États-Unis et Canada.

   >[!NOTE]
   >
   >Nous avons auparavant converti le Pays en un type de champ de liste de sélection et [ajout de tous les pays en tant que valeurs](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Et c&#39;est tout ! Désormais, lorsque des personnes remplissent ce formulaire et sélectionnent Etats-Unis pour le pays, le champ Etat s’affiche de manière dynamique avec les choix spécifiés.

>[!IMPORTANT]
>
>Le comportement des champs de formulaire fonctionne parfaitement lorsque les valeurs de champ sont définies/mises à jour au moyen d’un script personnalisé utilisant [Fonctions d’API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"} dans Forms 2.0.
>
>Les champs conditionnels peuvent ne pas fonctionner comme prévu si les valeurs de champ sont modifiées par des scripts externes autres que l’API JavaScript Forms 2.0.
