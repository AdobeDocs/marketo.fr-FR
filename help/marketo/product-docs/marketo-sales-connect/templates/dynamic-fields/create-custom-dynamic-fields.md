---
unique-page-id: 14352508
description: Création de champs dynamiques personnalisés - Documents Marketo - Documentation du produit
title: Créer des champs dynamiques personnalisés
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Créer des champs dynamiques personnalisés {#create-custom-dynamic-fields}

Il existe deux manières de créer des champs dynamiques personnalisés.

## Enregistrement de champs personnalisés pour un ou plusieurs contacts {#saving-custom-fields-for-one-or-a-few-contacts}

1. Cliquez sur le nom d&#39;un contact dans la page Personnes.

1. Sélectionnez la liste déroulante en regard de Désabonner et sélectionnez **Modifier**.

1. Faites défiler la page jusqu’au bas de la page de modification. Vous pouvez ensuite créer un nom et une valeur pour votre champ.

1. Cliquez sur **Enregistrer**.

## Enregistrement de champs personnalisés pour de nombreux contacts {#saving-custom-fields-for-many-contacts}

1. Créez une feuille de calcul CSV avec vos champs personnalisés dans leur propre colonne.

1. Suivez le [processus de chargement CSV normal](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), en s’arrêtant sur l’écran de mappage des champs.

1. Au lieu d’un des champs de paramètre prédéfini, sélectionnez **Ajouter un nouveau champ personnalisé** dans la liste déroulante.

1. Saisissez le nom de champ souhaité et cliquez sur **OK**.

1. Terminez le transfert de votre fichier CSV. Vos contacts recevront le champ personnalisé ajouté.

>[!NOTE]
>
>Une fois le champ personnalisé créé, il peut s’écouler 30 minutes avant qu’il ne s’affiche dans la liste déroulante des champs dynamiques de l’éditeur de modèles.

## Utilisation des champs personnalisés dans un modèle {#how-to-use-your-custom-fields-in-a-template}

Une fois vos champs personnalisés stockés à l’aide des méthodes ci-dessus, vous pouvez les référencer dans vos modèles.

1. [Créez un modèle](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) et cliquez sur le bouton **Champs dynamiques** comme vous le feriez normalement.

1. Sélectionnez **Champs personnalisés** dans la liste déroulante qui s’affiche.

1. Vos champs personnalisés préstockés s’affichent et vous pouvez en sélectionner un à remplir dans votre modèle.
