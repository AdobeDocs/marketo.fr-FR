---
unique-page-id: 37355569
description: Champs personnalisés des membres du programme - Documents marketing - Documentation du produit
title: Champs personnalisés des membres de programme
translation-type: tm+mt
source-git-commit: 2d03d93e120c8b3ce359c6aca44730cfa7c16bf9
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Champs personnalisés des membres de programme {#program-member-custom-fields}

Les champs personnalisés Membres du programme vous permettent de collecter des données spécifiques au programme pour chaque membre. Ils peuvent être utilisés dans : Formulaires marketing, filtres et déclencheurs de Listes dynamiques et actions de flux Smart Campaign. Les données peuvent être consultées dans l’onglet Membres du programme.

>[!NOTE]
>
>Pour le moment, les champs personnalisés Membres du programme n&#39;ont pas d&#39;intégration avec les champs Membres Campaign de Salesforce.

## Créer un champ personnalisé de membre de Programme {#create-a-program-member-custom-field}

1. Dans Marketo, cliquez sur **Admin**.

   ![](assets/one.png)

1. Cliquez sur **Gestion des champs**.

   ![](assets/two.png)

1. Cliquez sur **Nouveau champ personnalisé**.

   ![](assets/three.png)

1. Cliquez sur la liste déroulante Objet et sélectionnez l’objet de votre choix.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Les champs personnalisés Personne et Membre de Programme ne peuvent pas partager le même nom.

1. Renseignez les champs restants et cliquez sur **Créer**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Les types pris en charge pour les champs personnalisés Membres du Programme sont les suivants : booléen, date, datetime, float, integer, string, URL. [En savoir plus sur les types](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md) de champ.

## Descriptions des objets {#object-descriptions}

| Objet | Description |
|---|---|
| Société | Nom de la société associée à la personne. |
| Opportunité | Une occasion peut être associée à une personne ou à un compte en tant que vente future potentielle. Ils entrent généralement dans Marketo via une gestion de la relation client ou via une API. |
| Personne | Personne de votre base de données Marketo avec laquelle vous vous adressez par le biais de campagnes marketing. |
| Membre du programme | Personne qui est également membre d&#39;un programme |

## Déclencheurs et Filtres {#triggers-and-filters}

Vous pouvez exploiter ces données spécifiques à un programme dans les listes dynamiques par l&#39;intermédiaire de [triggers](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md) et/ou [filtres](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md).

![](assets/six.png)

## Informations à connaître {#things-to-know}

* Les champs personnalisés Membres du programme sont disponibles uniquement dans les ressources locales. Ils ne sont pas pris en charge dans Design Studio car il n’existe aucun moyen de le lier à un programme spécifique.
* Vous ne pouvez pas cloner ou déplacer un formulaire (ou un landing page avec un formulaire) qui contient des champs personnalisés Membre de Programme vers Design Studio.
* L&#39;objet Membre du Programme peut comporter jusqu&#39;à 20 champs personnalisés. Ces champs sont accessibles à tout programme.
* Lorsque vous supprimez un membre d&#39;un programme, si le champ personnalisé Membre du Programme contient des données, celles-ci sont supprimées de ce champ.
* Pour vue des données, cliquez sur l’onglet Membres du programme et créez une vue personnalisée qui inclut ledit ou ces champs.
* L’importation et l’exportation via [liste](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) et [API](https://developers.marketo.com/) sont prises en charge.
* Lorsque vous fusionnez deux personnes, les données de champ personnalisé Membre du Programme de l’expérience gagnante sont utilisées. Mais si le gagnant n’en a pas, la valeur du perdant sera utilisée.

>[!MORELIKETHIS]
>
>[Créer un champ personnalisé dans Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
