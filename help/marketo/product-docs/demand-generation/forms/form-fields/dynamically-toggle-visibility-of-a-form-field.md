---
unique-page-id: 2949962
description: Basculer dynamiquement la visibilité d’un champ de formulaire - Documents marketing - Documentation du produit
title: Basculer dynamiquement la visibilité d’un champ de formulaire
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---


# Basculer dynamiquement la visibilité d’un champ de formulaire {#dynamically-toggle-visibility-of-a-form-field}

>[!NOTE]
>
>**Conditions préalables**
>
>* [Ajouter une liste de pays à votre formulaire](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

>



L’une des fonctionnalités les plus intéressantes des formulaires Marketo est que vous pouvez masquer/afficher dynamiquement des champs ou des jeux de [champs](add-a-fieldset-to-a-form.md)de formulaire.

>[!NOTE]
>
>**Exemple**
>
>Dans cet exemple, masquons le champ **Etat** à moins que le **Pays** ne soit sélectionné comme &quot;Etats-Unis&quot;.

1. Accédez à **Marketing** **Activités**.

   ![](assets/login-marketing-activities-8.png)

1. Sélectionnez votre formulaire, puis cliquez sur **Modifier** le **formulaire**.

   ![](assets/editform-1.png)

1. Sélectionnez le champ à masquer/afficher dynamiquement et cliquez sur le lien correspondant aux **règles** de **visibilité**.

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
   >Auparavant, nous avons converti Pays en un type de champ de liste de prélèvement et [ajouté tous les pays en tant que valeurs](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Et c&#39;est tout ! Désormais, lorsque des personnes remplissent ce formulaire et sélectionnent Etats-Unis pour le pays, le champ Etat s’affiche de manière dynamique avec les choix spécifiés.

>[!NOTE]
>
>**Plongée profonde**
>
>Vous souhaitez en savoir plus sur [les formulaires](http://docs.marketo.com/display/docs/forms)?

