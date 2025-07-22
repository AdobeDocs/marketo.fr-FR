---
unique-page-id: 4720232
description: Création d’une liste de comptes - Documents Marketo - Documentation du produit
title: Créer une liste de comptes
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 8%

---

# Créer une liste de comptes {#create-a-new-account-list}

Créez et chargez une liste de noms d’organisation et de domaine pour cibler ces comptes clés avec des campagnes personnalisées.

>[!NOTE]
>
>Cet article s’applique uniquement aux anciens clients de la gestion des actifs numériques Web. Si vous avez acquis Web ABM après septembre 2016, suivez plutôt les étapes décrites dans [cet article](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList).

## Créer une liste de comptes {#create-a-new-account-list-1}

1. Accédez à **[!UICONTROL Listes de comptes]**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Sélectionnez **[!UICONTROL Créer]**.

   ![](assets/create-new-account-list-hand.jpg)

1. Sélectionnez **[!UICONTROL Parcourir]** et chargez votre fichier CSV (assurez-vous que le fichier CSV répond aux critères). Ajoutez un **[!UICONTROL Nom de la liste]** et **[!UICONTROL Description]**. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**Quel est le format du fichier CSV ?**
   >
   >Assurez-vous que le fichier CSV du compte nommé répond aux exigences suivantes :
   >
   >* Enregistré au format CSV
   >* Ne dépasse pas 10 Mo
   >* Seulement 4 colonnes avec l&#39;en-tête Colonne A : Nom, Colonne B : Domaine, Colonne C : Pays, Colonne D : Etat US.
   >* Le fichier téléchargé peut prendre jusqu’à deux jours ouvrables pour être validé.
   >* Vous recevrez un e-mail de notification de validation ou un avis d’état du fichier dans la page des comptes nommés.
   >* Le nombre total d’enregistrements/de lignes accumulés pour toutes vos listes chargées commence à 10 000, le package le plus volumineux atteignant 100 000.

   >[!NOTE]
   >
   >**Exemple du fichier CSV**
   >
   >* Ligne 1 Colonne A valeur = Organisation
   >* Ligne 1 Valeur de colonne B = Domaine
   >* Ligne 1 Colonne C value = Pays
   >* Ligne 1 Colonne D value = US State
   >* L’une des valeurs de colonne est obligatoire. Cependant, le fait de fournir à la fois des noms d’organisation et de domaine améliore les taux de correspondance de la liste des comptes.
   >* Le pays et l’état sont des valeurs facultatives.
   >
   >   * Pour le nom de pays, utilisez le nom de pays complet ou le code abréviation. Par exemple, États-Unis ou États-Unis.
   >   * Pour un État américain, utilisez le code abréviation à 2 lettres, c’est-à-dire CA. Seuls les États américains sont reconnus.
   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Modification d’une liste de comptes {#edit-an-account-list}

Sur la page **Listes de comptes**, cliquez sur l’icône **Modifier** dans la liste.

![](assets/create-new-account-list-edit.jpg)

Sélectionnez **[!UICONTROL Parcourir...]** et chargez votre nouveau fichier CSV. Ce fichier remplacera le fichier d’origine. Cliquez sur **[!UICONTROL Enregistrer]**. Le nouveau fichier chargé reste en attente jusqu’à ce qu’il soit approuvé par le support Marketo, tandis que le fichier d’origine reste actif tant qu’il est en attente.

![](assets/set-account-list-edit-hands.jpg)

Le fichier CSV remplacera le fichier existant. La liste existante reste active jusqu’à ce que le traitement du nouveau fichier soit terminé.

## Supprimer une liste de comptes nommés {#delete-a-named-account-list}

1. Sur la page **[!UICONTROL Listes de comptes]**, cliquez sur l’icône Supprimer de la liste à supprimer.

   ![](assets/create-new-account-list-delete.jpg)

1. Un message s’affiche pour confirmer la suppression de la liste. Cliquez sur **[!UICONTROL OK]**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Créer un segment à l’aide d’une liste de comptes](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
