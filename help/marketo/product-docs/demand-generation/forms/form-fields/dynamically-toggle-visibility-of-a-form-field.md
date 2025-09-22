---
unique-page-id: 2949962
description: Basculement dynamique de la visibilité d’un champ de formulaire - Documents Marketo - Documentation du produit
title: Activer/désactiver dynamiquement la visibilité d’un champ de formulaire
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 8%

---

# Activer/désactiver dynamiquement la visibilité d’un champ de formulaire {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Ajouter une liste de sélection de pays à votre formulaire](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Une fonctionnalité vraiment intéressante des formulaires Marketo est que vous pouvez masquer/afficher dynamiquement des champs de formulaire ou des [ensembles de champs](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exemple**
>
>Dans cet exemple, masquons le champ **État** sauf si **Pays** est sélectionné comme « États-Unis ».

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/login-marketing-activities-8.png)

1. Sélectionnez votre formulaire et cliquez sur **[!UICONTROL Modifier le formulaire]**.

   ![](assets/editform-1.png)

1. Sélectionnez le champ à masquer/afficher dynamiquement et cliquez sur le lien correspondant à **[!UICONTROL Règles de visibilité]**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Recherchez et sélectionnez le champ autour duquel vous souhaitez créer une condition.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Sélectionnez l’opérateur.

   >[!TIP]
   >
   >C&#39;est cool parce que vous pouvez choisir des matchs flous comme « [!UICONTROL commence par]. »

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Sélectionnez la ou les valeurs à rechercher, puis cliquez en dehors de la liste déroulante.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Vous pouvez sélectionner plusieurs valeurs en cliquant dessus lorsque la liste déroulante est ouverte. Par exemple, vous pouvez sélectionner États-Unis et Canada.

   >[!NOTE]
   >
   >Nous avons précédemment converti le Pays en type de champ de liste de sélection et [avons ajouté tous les pays en tant que valeurs](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Et c&#39;est tout ! Désormais, lorsque les personnes remplissent ce formulaire et sélectionnent États-Unis pour le pays, le champ État s’affiche de manière dynamique avec les choix spécifiés.

>[!IMPORTANT]
>
>Le comportement des champs de formulaire fonctionne de manière transparente lorsque les valeurs de champ sont définies/mises à jour par le biais d’un script personnalisé à l’aide de [ fonctions API ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"} dans Forms 2.0.
>
>Les champs conditionnels peuvent ne pas fonctionner comme prévu si les valeurs de champ sont modifiées par des scripts externes autres que l’API JavaScript Forms 2.0.
