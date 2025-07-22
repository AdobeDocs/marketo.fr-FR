---
unique-page-id: 11378814
description: '[!UICONTROL Listes de comptes] - Documents Marketo - Documentation du produit'
title: '[!UICONTROL Listes de comptes]'
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# [!UICONTROL Listes de comptes] {#account-lists}

Une liste de comptes est un ensemble de comptes nommés qui peuvent être ciblés ensemble. Les listes de comptes vous permettent de cibler des comptes nommés par secteur d’activité, emplacement ou taille de l’entreprise.

Outre les listes de comptes, vous pouvez également créer des listes de comptes dynamiques générées à partir des vues de compte CRM public. Une vue de compte CRM est un ensemble de règles qui agit comme un filtre lors de l’affichage des comptes. Par exemple, vous pouvez l’utiliser pour trouver les comptes où Industrie est Santé *et* Revenu est supérieur à 100 millions de dollars.

![](assets/one.png)

>[!NOTE]
>
>Les listes de comptes créées dans Marketo [!UICONTROL Gestion des comptes Target] sont automatiquement disponibles lors de la création de listes intelligentes et de campagnes web dans [Web Personalization](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Créer une liste de comptes {#create-a-new-account-list}

1. Cliquez sur le menu déroulant **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Créer une liste de comptes]**.

   ![](assets/1a.png)

1. Attribuez un nom à votre liste et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/three-0.png)

1. Après avoir créé votre liste de comptes, commencez à [y ajouter des comptes nommés](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md) !

   >[!NOTE]
   >
   >Marketo n’affiche des informations que pour les listes de comptes comportant 2 000 comptes nommés ou moins.

## Créer une liste de comptes dynamiques {#create-a-new-dynamic-account-list}

1. Cliquez sur la liste déroulante **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Créer une liste dynamique]**.

   ![](assets/1.png)

1. Dans la boîte de dialogue, sélectionnez une **Vue de compte CRM** dans la liste déroulante ou saisissez le nom pour la rechercher.

   ![](assets/image2017-7-18-9-48-23.png)

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Dans Salesforce, veillez à fournir des autorisations d’objet de vue Liste à l’utilisateur de synchronisation.

## Renommer une liste de comptes {#rename-an-account-list}

>[!NOTE]
>
>Ces étapes s’appliquent uniquement aux listes de comptes. Les listes de comptes _dynamiques_ utilisent le nom des vues de compte CRM associées.

1. Sélectionnez le compte à renommer, cliquez sur le menu déroulant **[!UICONTROL Actions de la liste des comptes]** et sélectionnez **[!UICONTROL Renommer la liste des comptes]**.

   ![](assets/three.png)

1. Saisissez le nouveau nom et cliquez sur **[!UICONTROL Renommer]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La vue Compte CRM se synchronise avec la liste des comptes dynamiques toutes les 8 heures. S’ils ne sont pas encore synchronisés, Marketo les synchronisera au cours du cycle suivant.

## Suppression d’une liste de comptes {#delete-an-account-list}

>[!NOTE]
>
>Ces étapes sont identiques pour les listes de comptes et les listes de comptes dynamiques.

1. Sélectionnez le compte à supprimer, cliquez sur le menu déroulant **[!UICONTROL Actions de liste de comptes]** et sélectionnez **[!UICONTROL Supprimer la liste de comptes]**.

   ![](assets/five.png)

1. Cliquez sur **[!UICONTROL Supprimer]**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Ajout d’un compte existant [!UICONTROL Compte nommé] à une liste de comptes](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Informations sur la liste des comptes](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
