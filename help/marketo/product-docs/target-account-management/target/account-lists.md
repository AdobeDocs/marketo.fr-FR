---
unique-page-id: 11378814
description: Listes de comptes - Documents Marketo - Documentation du produit
title: Listes de comptes
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Listes de comptes {#account-lists}

Une liste de comptes est un ensemble de comptes nommés qui peuvent être ciblés ensemble. Les listes de comptes vous permettent de cibler des comptes nommés par secteur, emplacement ou taille de l’entreprise.

Outre les listes de comptes, vous pouvez créer des listes de comptes dynamiques générées à partir des vues de compte CRM publiques. Une vue de compte CRM est un ensemble de règles qui agit comme un filtre lors de l’affichage de comptes. Vous pouvez, par exemple, l’utiliser pour rechercher des comptes pour lesquels le secteur industriel est le secteur des soins de santé *et où le chiffre d’affaires est supérieur à 100 millions de dollars.*

![](assets/one.png)

>[!NOTE]
>
>Les listes de compte créées dans la gestion de compte Marketo Target sont automatiquement disponibles lors de la création de listes dynamiques et de campagnes web dans [Personalization web](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Créer une liste de comptes {#create-a-new-account-list}

1. Cliquez sur la liste déroulante **New** et sélectionnez **Create New Account List**.

   ![](assets/1a.png)

1. Donnez un nom à votre liste et cliquez sur **Créer**.

   ![](assets/three-0.png)

1. Après avoir créé votre liste de comptes, commencez à [y ajouter des comptes nommés](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo affiche uniquement les informations des listes de comptes avec 2 000 comptes nommés ou moins.

## Création d’une liste de comptes dynamiques {#create-a-new-dynamic-account-list}

1. Cliquez sur la liste déroulante **New** et sélectionnez **Create New Dynamic List**.

   ![](assets/1.png)

1. Dans la boîte de dialogue, sélectionnez une **vue de compte CRM** dans la liste déroulante ou saisissez le nom pour la rechercher.

   ![](assets/image2017-7-18-9-48-23.png)

1. Cliquez sur **Créer**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Dans Salesforce, veillez à accorder les autorisations List View Object à l’utilisateur de synchronisation.

## Renommer une liste de comptes {#rename-an-account-list}

>[!NOTE]
>
>Ces étapes s&#39;appliquent uniquement aux listes de comptes. Les listes de comptes _dynamiques_ utilisent le nom de leurs vues de compte CRM associées.

1. Sélectionnez le compte à renommer, cliquez sur la liste déroulante **Actions de liste de comptes** et sélectionnez **Renommer la liste de comptes**.

   ![](assets/three.png)

1. Saisissez le nouveau nom et cliquez sur **Renommer**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La vue Compte CRM se synchronise avec la liste des comptes dynamiques toutes les 8 heures. S’ils ne sont pas encore synchronisés, Marketo les synchronise au cours du cycle suivant.

## Suppression d’une liste de comptes {#delete-an-account-list}

>[!NOTE]
>
>Ces étapes sont les mêmes pour les listes de comptes et les listes de comptes dynamiques.

1. Sélectionnez le compte à supprimer, cliquez sur la liste déroulante **Actions de liste de comptes** et sélectionnez **Supprimer la liste de comptes**.

   ![](assets/five.png)

1. Cliquez sur **Supprimer**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Ajouter un compte nommé existant à une liste de comptes](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [ Statistiques sur la liste de comptes ](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
