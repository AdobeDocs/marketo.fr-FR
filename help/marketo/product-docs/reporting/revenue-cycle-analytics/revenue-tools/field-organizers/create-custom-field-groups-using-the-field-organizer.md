---
unique-page-id: 10094404
description: Création de groupes de champs personnalisés à l’aide de l’organisateur de champs - Documents Marketo - Documentation du produit
title: Créer des groupes de champs personnalisés à l’aide de l’organisateur de champs
exl-id: 0425a446-2c92-4a2a-85c4-e05c22118035
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 4%

---

# Créer des groupes de champs personnalisés à l’aide de l’organisateur de champs {#create-custom-field-groups-using-the-field-organizer}

Avant de pouvoir activer des groupes de champs personnalisés pour la création de rapports dans la zone Analyse des performances du modèle (leads) de l’Explorateur du cycle du chiffre d’affaires, vous devez catégoriser les champs standard ou personnalisés en groupes pour la création de rapports via l’Organisateur de champs dans Marketo Lead Management. Cela s’applique uniquement aux attributs de prospect et d’entreprise.
Lorsque vous sélectionnez un champ standard ou personnalisé dans la liste déroulante Champ de la boîte de dialogue Nouvelle organisation des champs , le système mappe le type de données de gestion des prospects Marketo associé au champ que vous souhaitez regrouper avec l’un des trois éditeurs disponibles dans l’organisation des champs : chaîne, entier ou date.

| Type de données de gestion des leads Marketo | Type De Données De L’Éditeur De L’Organisateur De Champs |
|---|---|
| Chaîne | Chaîne |
| E-mail | Chaîne |
| Nombre entier | Nombre entier |
| Texte | Chaîne |
| URL | Chaîne |
| Référence | Non pris en charge |
| Devise | Nombre entier |
| DateHeure | Date |
| Booléen | Non pris en charge |
| Téléphone | Chaîne |
| Date | Date |
| Flottante | Nombre entier |
| Calculé | Non pris en charge |

Les trois sections suivantes décrivent comment créer un groupe de champs personnalisé pour un type chaîne, entier ou date.

## Créer Un Groupe De Champs Personnalisé - Éditeur De Chaînes {#create-custom-field-group-string-editor}

1. Cliquez sur **[!UICONTROL Base de données de lead]**.

   ![](assets/one.png)

1. Cliquez sur **[!UICONTROL Nouveau]**, puis sélectionnez **[!UICONTROL Nouvel organisateur de champ]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Champ]** et sélectionnez un champ standard ou personnalisé avec un type de données qui correspond à l’éditeur de chaînes (voir le tableau dans la section précédente). [!UICONTROL &#x200B; Pays &#x200B;] est utilisé ici.

   ![](assets/three.png)

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/four.png)

   Le nouveau groupe personnalisé s’affiche dans l’arborescence de la base de données des prospects sous la forme Nom du champ > Groupe de noms de champ (exemple : Pays > Groupe de pays).

   ![](assets/4.5.png)

1. Cliquez sur l’icône en forme de crayon pour personnaliser le nom. Par exemple, vous pouvez renommer « Groupe de pays » en « Continent ». Saisissez le nouveau nom de votre choix et cliquez en dehors de la zone pour l’enregistrer automatiquement.

   ![](assets/five.png)

1. Par défaut, toutes les valeurs de données sont placées dans le sous-groupe « [!UICONTROL Autre] ». Pour catégoriser les valeurs de données, cliquez sur **[!UICONTROL Ajouter un groupe]** pour créer un sous-groupe et lui donner un nom.

   >[!NOTE]
   >
   >Vous pouvez ajouter jusqu’à dix sous-groupes pour catégoriser les valeurs des données. Chaque sous-groupe créé se voit attribuer un numéro d’identification.

   Dans cet exemple, des groupes ont été créés pour la plupart des continents.

   ![](assets/six.png)

   >[!NOTE]
   >
   >Pour supprimer un sous-groupe, cliquez simplement sur le X rouge en regard du nom du sous-groupe. Si le groupe contient des valeurs de données, celles-ci sont déplacées vers le groupe par défaut [!UICONTROL Autre].

1. Mettez en surbrillance une ou plusieurs valeurs de données dans la zone de travail, puis faites glisser et déposez la ou les valeurs de données dans le sous-groupe approprié.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Pour supprimer une valeur de données d’un sous-groupe, réaffectez-la au groupe par défaut Autre.

1. Utilisez l’option de filtre dans le coin supérieur gauche, directement au-dessus de la zone de travail, pour sélectionner et afficher les valeurs des données dans un ou plusieurs sous-groupes. Les valeurs de données basées sur votre sélection de filtre s’affichent dans la zone de travail.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Une fois les groupes définis, vous pouvez activer le groupe de champs personnalisés pour le reporting dans l’analyse des performances du modèle (prospects) via l’onglet Analyse du cycle de chiffre d’affaires dans la gestion des prospects Marketo.

## Créer Un Groupe De Champs Personnalisé - Éditeur D’Entiers {#create-custom-field-group-integer-editor}

1. Cliquez sur **[!UICONTROL Base de données de lead]**.

   ![](assets/one.png)

1. Cliquez sur **[!UICONTROL Nouveau]**, puis sélectionnez **[!UICONTROL Nouvel organisateur de champ]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Champ]** et sélectionnez un champ standard ou personnalisé avec un type de données qui correspond à l’éditeur de chaînes (voir le tableau dans la section précédente). Le [!UICONTROL chiffre d’affaires annuel] est utilisé ici.

   ![](assets/nine.png)

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/9.5.png)

   Le nouveau groupe personnalisé s’affiche dans l’arborescence de la base de données des prospects sous la forme Nom du champ > Groupe de noms de champ (exemple : Chiffre d’affaires annuel > Groupe de chiffres d’affaires annuels).

   ![](assets/9.6.png)

1. Cliquez sur le nom de groupe personnalisé par défaut au-dessus de l’éditeur de nombres entiers pour personnaliser le nom. Par exemple, vous pouvez renommer « Groupe de revenus annuels » en « Revenus annuels par taille ». Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/eleven.png)

   L’éditeur d’entiers vous permet de créer plusieurs sous-groupes pour définir chaque sous-groupe par taille. Dans cet exemple, trois groupes seront créés pour les petites entreprises, les Medium et les entreprises.

1. Pour ajouter votre premier groupe, saisissez un nom dans le champ **[!UICONTROL Nom du groupe]** (exemple : Petit) et saisissez une valeur maximale dans le champ **[!UICONTROL Plage de groupes]** (exemple : 200000). Cliquez sur **[!UICONTROL Ajouter un groupe]**.

   ![](assets/twelve.png)

   Une entrée de groupe vide s’affiche sous le groupe que vous venez de saisir. L’exemple ci-dessous montre une entrée pour les petites entreprises, les entreprises Medium et les entreprises.

   >[!NOTE]
   >
   >Vous pouvez ajouter jusqu’à dix sous-groupes pour catégoriser les valeurs des données. Chaque entrée de plage de groupes s’appuie sur l’entrée précédente. Si vous laissez vide l&#39;entrée de la dernière plage de groupes pour le dernier sous-groupe personnalisé que vous créez, aucune valeur de données maximale n&#39;est définie.

1. Cliquez sur l’onglet Résumé pour enregistrer et vérifier vos paramètres.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Pour supprimer un sous-groupe, cliquez sur le X rouge en regard du nom du sous-groupe.

1. Vérifiez vos paramètres dans la page Résumé .

   ![](assets/13.5.png)

   >[!NOTE]
   >
   >Une fois les groupes définis, vous pouvez activer le groupe de champs personnalisés pour le reporting dans l’analyse des performances du modèle (prospects) via l’onglet Analyse du cycle de chiffre d’affaires dans la gestion des prospects Marketo.

## Créer un groupe de champs personnalisé - Éditeur de date {#create-custom-field-group-date-editor}

1. Cliquez sur **[!UICONTROL Base de données de lead]**.

   ![](assets/one.png)

1. Cliquez sur **[!UICONTROL Nouveau]**, puis sélectionnez **[!UICONTROL Nouvel organisateur de champ]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Champ]** et sélectionnez un champ standard ou personnalisé avec un type de données qui correspond à l’éditeur de chaînes (voir le tableau dans la section précédente). [!UICONTROL &#x200B; Date d’acquisition &#x200B;] est utilisé ici.

   ![](assets/fourteen.png)

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/14.5.png)

   Le nouveau groupe personnalisé s’affiche dans l’arborescence de la base de données de leads sous la forme Nom du champ > Groupe de noms de champ (exemple : Date d’acquisition > Groupe de dates d’acquisition).

   ![](assets/14.6.png)

1. Cliquez sur le nom de groupe personnalisé par défaut au-dessus de l’éditeur de dates pour personnaliser le nom. Par exemple, vous pouvez renommer « Groupe de dates d’acquisition » en « Catégories de dates d’acquisition ». Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/fifteen.png)

   L’éditeur de date vous permet de créer plusieurs sous-groupes et de définir chaque sous-groupe par date. Dans cet exemple, trois groupes seront créés : Leads du T1-15, Leads du T2-15 et Leads du T3-15.

1. Pour ajouter votre premier groupe, saisissez un nom dans le champ **[!UICONTROL Nom du groupe]** (exemple : Leads 1T15) et saisissez une date dans le champ de date qui représente la date à laquelle le prospect a été acquis le ou avant (exemple : 3/31/2015 pour le dernier jour du 1T15). Cliquez sur **[!UICONTROL Ajouter un groupe]**.

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >Vous pouvez ajouter jusqu’à dix sous-groupes pour catégoriser les valeurs des données. Chaque entrée [!UICONTROL Plage de groupes] s’appuie sur l’entrée précédente. Si vous laissez l&#39;entrée [!UICONTROL Plage de groupes] vide pour le dernier sous-groupe personnalisé que vous créez, aucune valeur de date de fin n&#39;est définie.

   L’exemple ci-dessous montre une entrée pour les prospects du 1er trimestre 2015 jusqu’au 3e trimestre.

   ![](assets/16.5.png)

   Et c&#39;est tout ! Bon travail.
