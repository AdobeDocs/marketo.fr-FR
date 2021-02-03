---
unique-page-id: 2949962
description: Basculer dynamiquement la visibilité d’un champ de formulaire - Documents marketing - Documentation du produit
title: Basculer dynamiquement la visibilité d’un champ de formulaire
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Basculer dynamiquement la visibilité d’un champ de formulaire {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Ajouter une liste de pays à votre formulaire](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


L’une des fonctionnalités les plus intéressantes des formulaires Marketo est que vous pouvez masquer/afficher dynamiquement les champs de formulaire ou [les jeux de champs](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Exemple**
>
>Dans cet exemple, masquons le champ **Etat** à moins que **Pays** ne soit sélectionné comme &quot;Etats-Unis&quot;.

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities-8.png)

1. Sélectionnez votre formulaire et cliquez sur **Modifier le formulaire**.

   ![](assets/editform-1.png)

1. Sélectionnez le champ à masquer/afficher dynamiquement et cliquez sur le lien **Règles de visibilité**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Recherchez et sélectionnez le champ sur lequel vous souhaitez créer une condition.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Sélectionnez l’opérateur.

   >[!TIP]
   >
   >C&#39;est cool parce que vous pouvez choisir des allumettes floues comme &quot;débuts avec&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Sélectionnez la ou les valeurs à rechercher, puis cliquez en dehors de la liste déroulante.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Vous pouvez sélectionner plusieurs valeurs en cliquant dessus pendant que la liste déroulante est ouverte. Par exemple, vous pouvez sélectionner Etats-Unis et Canada.

   >[!NOTE]
   >
   >Auparavant, nous avons converti Pays en un type de champ de liste de prélèvement et [ajouté tous les pays en tant que valeurs](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Et c&#39;est tout ! Désormais, lorsque des personnes remplissent ce formulaire et sélectionnent Etats-Unis pour le pays, le champ Etat s’affiche de manière dynamique avec les choix spécifiés.
