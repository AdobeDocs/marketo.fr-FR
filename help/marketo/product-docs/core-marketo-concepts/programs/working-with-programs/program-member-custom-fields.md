---
unique-page-id: 37355569
description: Champs personnalisés des membres du programme - Documents Marketo - Documentation du produit
title: Champs personnalisés des membres du programme
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
source-git-commit: 10f7bf5b8b3fd91e98550ab281e5ddda87b1c30b
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 1%

---

# Champs personnalisés des membres du programme {#program-member-custom-fields}

Les champs personnalisés Membres du programme vous permettent de collecter des données spécifiques au programme pour chaque membre. Ils peuvent être utilisés dans : Formulaires Marketo, filtres et déclencheurs de liste dynamique et actions de flux de campagne dynamique. Les données sont visibles dans l’onglet Membres du programme.

## Créer un champ personnalisé de membre de programme {#create-a-program-member-custom-field}

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/one.png)

1. Cliquez sur **Gestion des champs**.

   ![](assets/two.png)

1. Cliquez sur **Nouveau champ personnalisé**.

   ![](assets/three.png)

1. Cliquez sur la liste déroulante Objet et sélectionnez l’objet de votre choix.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Les champs personnalisés Personne et Membre du programme ne peuvent pas partager le même nom.

1. Renseignez les champs restants et cliquez sur **Créer**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Les types pris en charge pour les champs personnalisés des membres du programme sont les suivants : booléen, date, datetime, float, entier, chaîne, URL. [En savoir plus sur les types de champ](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target=&quot;_blank&quot;}.

## Descriptions des objets {#object-descriptions}

| Objet | Description |
|---|---|
| Société | Nom de la société associée à la personne. |
| Opportunité | Une opportunité peut être associée à une personne ou à un compte en tant que vente future potentielle. Ils accèdent généralement à Marketo par le biais d’un CRM ou d’une API. |
| Individu | Personne de la base de données Marketo avec laquelle vous interagissez par le biais de campagnes marketing. |
| Membre du programme | Personne qui est également membre d’un programme |

## Déclencheurs et filtres {#triggers-and-filters}

Vous pouvez exploiter ces données spécifiques au programme dans des listes dynamiques via [triggers](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target=&quot;_blank&quot;} et/ou [filtres](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target=&quot;_blank&quot;}.

![](assets/six.png)

## Informations à connaître {#things-to-know}

* Les champs personnalisés Membres du programme sont disponibles uniquement dans les ressources locales. Ils ne sont pas pris en charge dans Design Studio, car il n’existe aucun moyen de le lier à un programme spécifique.
* Vous ne pouvez pas cloner/déplacer un formulaire (ou une landing page avec un formulaire) contenant des champs personnalisés de membre de programme vers Design Studio.
* [Vous pouvez synchroniser](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target=&quot;_blank&quot;} : champ personnalisé du membre de programme avec champs personnalisés du membre de campagne.
* L’objet membre du programme peut comporter jusqu’à 20 champs personnalisés. Ces champs sont disponibles pour tous les programmes.
* Lorsque vous supprimez un membre d’un programme, si le champ personnalisé Membre du programme contient des données, celles-ci sont supprimées de ce champ.
* Pour afficher les données, cliquez sur l’onglet Membres du programme et créez une vue personnalisée qui inclut ces champs.
* Import et export via [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target=&quot;_blank&quot;} et [API](https://developers.marketo.com/){target=&quot;_blank&quot;} sont pris en charge. Les exportations ne fonctionnent que sur les listes de membres de programme, et non sur les listes statiques.
* Lorsque vous fusionnez deux personnes, les données de champ personnalisé Membre du programme du gagnant sont utilisées. Mais si le gagnant n’en a pas, la valeur du perdant sera utilisée.
* Le type de modification n’est pas autorisé dans les champs Informations sur les membres du programme.
* La contrainte Liste dynamique &quot;contient&quot; n’est pas prise en charge pour les champs personnalisés Membres du programme.

>[!MORELIKETHIS]
>
>* [Création d’un champ personnalisé dans Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target=&quot;_blank&quot;}
>
>* [Synchronisation des champs personnalisés des membres du programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target=&quot;_blank&quot;}

