---
unique-page-id: 4720232
description: Création d’une liste de comptes - Documents Marketo - Documentation du produit
title: Créer une liste de comptes
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 7%

---

# Créer une liste de comptes {#create-a-new-account-list}

Créez et téléchargez une liste de noms d’organisation et de domaine pour cibler ces comptes clés avec des campagnes personnalisées.

>[!NOTE]
>
>Cet article s’applique uniquement aux clients Web ABM hérités. Si vous avez acquis Web ABM après septembre 2016, suivez plutôt les étapes décrites dans [cet article](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) .

## Créer une liste de comptes {#create-a-new-account-list-1}

1. Accédez à **Listes de comptes**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Sélectionnez **Créer**.

   ![](assets/create-new-account-list-hand.jpg)

1. Sélectionnez **Parcourir** et téléchargez votre fichier CSV (assurez-vous que le fichier CSV répond aux critères). Ajoutez un **Nom** et une **Description**. Cliquez sur **Enregistrer**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**Quel est le format du fichier CSV ?**
   >
   >Assurez-vous que le fichier CSV du compte nommé répond aux exigences suivantes :
   >
   >* Enregistré au format CSV
   >* Ne dépasse pas 10 Mo
   >* Seulement 4 colonnes avec l’en-tête Colonne A : Nom, Colonne B : Domaine, Colonne C : Pays, Colonne D : Etat américain.
   >* Le fichier téléchargé peut prendre jusqu’à deux jours ouvrables pour être validé.
   >* Vous recevrez un e-mail de notification de validation ou un avis d’état du fichier dans la page des comptes nommés.
   >* Le nombre total d&#39;enregistrements/lignes cumulés pour toutes vos listes téléchargées commence à 10K, avec le plus grand package totalisant 100K.

   >[!NOTE]
   >
   >**Exemple de fichier CSV**
   >
   >* Ligne 1 Colonne A Valeur = Organisation
   >* Ligne 1 Valeur de colonne B = Domaine
   >* Ligne 1 Valeur de colonne C = Pays
   >* Ligne 1 colonne D valeur = Etat des États-Unis
   >* L’une des valeurs de colonne est obligatoire. Cependant, le fait de fournir des noms d’organisation et de domaine améliore les taux de correspondance de la liste de comptes.
   >* Pays et Etat sont des valeurs facultatives.
   >
   >   * Pour le nom du pays, utilisez le nom du pays complet ou le code d’abréviation. Par exemple, États-Unis ou États-Unis.
   >   * Pour un état des États-Unis, utilisez le code d’abréviation de 2 lettres, c’est-à-dire CA. Seuls les États américains sont reconnus.
   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Modifier une liste de comptes {#edit-an-account-list}

Sur la page **Listes de comptes**, cliquez sur l’icône **Modifier** de la liste.

![](assets/create-new-account-list-edit.jpg)

Sélectionnez **Parcourir** et téléchargez votre nouveau fichier CSV. Ce fichier remplacera le fichier d’origine. Cliquez sur **Enregistrer**. Le nouveau fichier téléchargé restera dans l’état en attente jusqu’à ce qu’il soit approuvé par l’assistance Marketo. Dans l’état en attente, le fichier d’origine restera actif.

![](assets/set-account-list-edit-hands.jpg)

Le fichier CSV remplace le fichier existant. La liste existante reste active jusqu’à ce que le traitement du nouveau fichier soit terminé.

## Suppression d’une liste de comptes nommés {#delete-a-named-account-list}

1. Sur la page **Listes de comptes**, cliquez sur l’icône Supprimer de la liste que vous souhaitez supprimer.

   ![](assets/create-new-account-list-delete.jpg)

1. Un message s’affiche pour confirmer la suppression de la liste. Cliquez sur **OK**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Créer un segment à l’aide d’une liste de comptes](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
