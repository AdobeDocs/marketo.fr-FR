---
unique-page-id: 14352508
description: Création De Champs Dynamiques Personnalisés - Documents Marketo - Documentation Du Produit
title: Création de champs dynamiques personnalisés
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Création de champs dynamiques personnalisés {#create-custom-dynamic-fields}

Il existe deux façons de créer des champs dynamiques personnalisés.

## Enregistrement de champs personnalisés pour un ou plusieurs contacts {#saving-custom-fields-for-one-or-a-few-contacts}

1. Cliquez sur le nom d&#39;un contact dans la page [!UICONTROL Personnes].

1. Sélectionnez la liste déroulante en regard de [!UICONTROL Se désabonner] et sélectionnez **[!UICONTROL Modifier]**.

1. Faites défiler jusqu’au bas de la page d’édition. Vous pouvez ensuite créer un nom et une valeur pour votre champ.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

## Enregistrement de champs personnalisés pour de nombreux contacts {#saving-custom-fields-for-many-contacts}

1. Créez une feuille de calcul CSV avec vos champs personnalisés dans leur propre colonne.

1. Suivez le [processus de chargement CSV normal](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), en vous arrêtant sur l’écran de mappage des champs.

1. Au lieu de l’un des champs prédéfinis, choisissez **[!UICONTROL Ajouter un nouveau champ personnalisé]** dans la liste déroulante.

1. Saisissez le nom du champ souhaité, puis cliquez sur **[!UICONTROL OK]**.

1. Terminez de charger le fichier CSV. Vos contacts s’afficheront avec le champ personnalisé ajouté.

>[!NOTE]
>
>Après avoir créé votre champ personnalisé, il peut s’écouler environ 30 minutes avant que le champ n’apparaisse dans le menu déroulant du champ dynamique de votre éditeur de modèles.

## Utilisation de vos champs personnalisés dans un modèle {#how-to-use-your-custom-fields-in-a-template}

Une fois vos champs personnalisés stockés à l’aide des méthodes ci-dessus, vous pourrez les référencer dans vos modèles.

1. [Créez un modèle](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) puis cliquez sur le bouton **[!UICONTROL Champs dynamiques]** comme vous le feriez normalement.

1. Sélectionnez **[!UICONTROL Champs personnalisés]** dans la liste déroulante qui s’affiche.

1. Vos champs personnalisés préstockés s’affichent et vous pouvez en sélectionner un pour le remplir dans votre modèle.
