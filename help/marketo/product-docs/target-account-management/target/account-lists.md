---
unique-page-id: 11378814
description: Listes de comptes - Documents Marketo - Documentation du produit
title: Listes de comptes
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 1%

---

# Listes de comptes {#account-lists}

Une liste de comptes est un ensemble de comptes nommés qui peuvent être ciblés ensemble. Les listes de comptes vous permettent de cibler des comptes nommés par secteur, emplacement ou taille de l’entreprise.

Outre les listes de comptes, vous pouvez créer des listes de comptes dynamiques générées à partir des vues de compte CRM publiques. Une vue de compte CRM est un ensemble de règles qui agit comme un filtre lors de l’affichage de comptes. Par exemple, vous pouvez l’utiliser pour rechercher des comptes où le secteur est celui des soins de santé. *et* Les recettes sont supérieures à 100 millions de dollars.

![](assets/one.png)

>[!NOTE]
>
>Les listes de compte créées dans la gestion de compte Marketo Target sont automatiquement disponibles lors de la création de listes intelligentes et de campagnes web dans [Personnalisation web](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Créer une liste de comptes {#create-a-new-account-list}

1. Cliquez sur le bouton **Nouveau** et sélectionnez **Créer une liste de comptes**.

   ![](assets/1a.png)

1. Attribuez un nom à votre liste et cliquez sur **Créer**.

   ![](assets/three-0.png)

1. Après avoir créé votre liste de comptes, commencez à [l’ajout de comptes nommés](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo affiche uniquement les informations des listes de comptes avec 2 000 comptes nommés ou moins.

## Création d’une liste de comptes dynamiques {#create-a-new-dynamic-account-list}

1. Cliquez sur le bouton **Nouveau** et sélectionnez **Créer une liste dynamique**.

   ![](assets/1.png)

1. Dans la boîte de dialogue, sélectionnez une **Vue du compte CRM** dans la liste déroulante ou saisissez le nom pour le rechercher.

   ![](assets/image2017-7-18-9-48-23.png)

1. Cliquez sur **Créer**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Dans Salesforce, veillez à accorder les autorisations List View Object à l’utilisateur de synchronisation.

## Renommer une liste de comptes {#rename-an-account-list}

>[!NOTE]
>
>Ces étapes s&#39;appliquent uniquement aux listes de comptes. _Dynamique_ Les listes de comptes utilisent le nom de leurs vues de compte CRM associées.

1. Sélectionnez le compte à renommer, puis cliquez sur le bouton **Actions de liste de comptes** et sélectionnez **Renommer la liste des comptes**.

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

1. Sélectionnez le compte à supprimer, puis cliquez sur le bouton **Actions de liste de comptes** et sélectionnez **Supprimer la liste de comptes**.

   ![](assets/five.png)

1. Cliquez sur **Supprimer**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Ajout d’un compte nommé existant à une liste de comptes](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Informations sur la liste de comptes](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)

