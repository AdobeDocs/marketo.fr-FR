---
description: La description va ici.
title: Gestion des listes de sélection
hide: true
hidefromtoc: true
feature: Field Management
source-git-commit: 3c9facaed46a72c12a8a604aa9d22b47e28183cb
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Gestion des listes de sélection {#picklist-management}

La gestion des listes de sélection vous permet de définir un ensemble fixe de valeurs pour un champ afin de simplifier la gestion des données et des workflows dans Marketo Engage. Seuls les champs non textuels non mappés à un champ CRM avec une liste de sélection définie peuvent être gérés dans Marketo. Si un champ est mappé à un champ CRM qui possède une liste de sélection définie, les valeurs de ce champ doivent être définies dans le CRM.

Vous pouvez voir le statut d’une liste de sélection sur sa page Gestion des champs . Un champ peut avoir l’un des statuts de liste de sélection suivants :

* **Géré** : un utilisateur a défini l’ensemble des valeurs qui peuvent être suggérées automatiquement pour ce champ. Seules les valeurs définies dans la gestion des champs sont suggérées automatiquement. Si une liste de sélection gérée est supprimée, le statut de la liste de sélection revient à la valeur initiale du champ, soit Non géré soit Prédéfini.

* **Non géré** : les valeurs possibles pour ce champ ne sont pas définies. Les valeurs sont suggérées automatiquement en fonction de celles qui existent dans ces champs de la base de données.

* **Prédéfini** : le champ comporte une liste définie par le système de valeurs suggérées à l’utilisateur.

* **CRM** : le champ contient une valeur définie par le système CRM, Salesforce.com ou Microsoft Dynamics, synchronisée avec l’instance.

  ![](assets/picklist-management-1.png)

## Gérer la liste de sélection {#manage-picklist}

Pour modifier les valeurs d’un champ, accédez à **Admin** > **Gestion des champs** et sélectionnez le champ de votre choix.

Cliquez sur le menu déroulant _Actions de champ_ et sélectionnez **Gérer la liste de sélection**.

![](assets/picklist-management-2.png)

Dans la boîte de dialogue _Gérer la liste de sélection_ vous pouvez ajouter, modifier ou supprimer des valeurs. Vous pouvez également supprimer la liste de sélection gérée pour rétablir le statut d’origine du champ dans la liste de sélection, _Non géré_ ou _Prédéfini_.

![](assets/picklist-management-3.png)

Chaque entrée de la liste de sélection possède une valeur d’affichage et une valeur envoyée. La valeur d’affichage est celle qui est suggérée à l’utilisateur lors de la création de listes intelligentes, de campagnes intelligentes ou de formulaires, tandis que la valeur envoyée est celle qui est stockée. Par exemple, votre cas d’utilisation Code de territoire peut suggérer le nom complet d’un territoire (par exemple, Alberta), tout en stockant le code à deux lettres (AB).

## Suggérer automatiquement {#autosuggest}

### Basculer entre les listes de sélection gérées et non gérées {#switching}

La plupart des abonnements Marketo Engage contiennent des données antérieures à l’introduction des listes de sélection gérées. Pour utiliser des valeurs dans des listes dynamiques ou des étapes de flux à partir de cette liste de sélection de version non gérée (par exemple, à partir du jeu complet de valeurs qui existe sur les enregistrements dans votre base de données), activez le paramètre Liste de sélection gérée dans votre liste dynamique ou votre vue Campagne. Lorsque cette option est activée, seules les valeurs de la liste de sélection gérée s’affichent. Lorsqu’elle est désactivée, la liste de sélection non gérée est utilisée et les valeurs sont suggérées automatiquement en fonction des valeurs existantes dans la base de données.

### Listes De Sélection De Formulaires (Sélectionner Des Champs De Type) {#form-picklists}

Comme pour les listes de sélection prédéfinies et gérées par CRM, les valeurs des listes de sélection gérées se propagent dans Forms lors de l’utilisation du type de champ Sélectionner . Pour un champ avec une liste de sélection gérée, sélectionnez ce champ et définissez le Type de champ sur _Sélectionner_.

![](assets/picklist-management-4.png)

L’ensemble des valeurs de liste de sélection gérée définies pour ce champ s’affiche.

![](assets/picklist-management-5.png)
