---
unique-page-id: 12615800
description: Importation de comptes nommés - Documents Marketo - Documentation du produit
title: Importer les comptes nommés
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Importer les comptes nommés {#import-named-accounts}

Vous disposez déjà d’un fichier CSV contenant de nombreux comptes cibles potentiels ? Importez-les directement dans TAM !

1. Cliquez sur la liste déroulante **New** et sélectionnez **Importer les comptes nommés**.

   ![](assets/inaone.png)

1. Une nouvelle fenêtre s’ouvre. Cliquez sur **Parcourir**, puis sélectionnez le fichier des comptes nommés à importer.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Dans votre fichier, fournissez [autant d&#39;informations](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) que possible. Vous pouvez uniquement ajouter des informations démographiques ; aucune analyse Marketo (c’est-à-dire Pipeline). Pour créer des comptes nommés basés sur des comptes CRM, il vous suffit d’exporter le nom du compte et l’identifiant CRM de votre CRM dans un fichier CSV, d’utiliser l’option Nom du compte et de mapper l’identifiant CRM au cours du processus d’importation. Pour lier correctement un compte CRM à un compte nommé, vous devez indiquer le nom exact du compte CRM.

1. Choisissez l’un des deux modes de déduplication : Nom du compte ou Nom de domaine. Dans cet exemple, nous choisirons Compte . Cliquez sur la liste déroulante **Modes** et sélectionnez **Par nom de compte**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Si vous choisissez **Par mode de domaine**, les champs de compte et de domaine nommés doivent être inclus.

1. Pour choisir la liste des comptes auxquels votre compte nommé sera ajouté, cliquez sur la liste déroulante **Liste des comptes** et effectuez votre sélection.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Vous pouvez également créer une nouvelle liste de comptes en saisissant simplement son nom dans la liste déroulante.

1. Pour envoyer une notification de l’importation, cliquez sur la liste déroulante **Envoyer une alerte à** et sélectionnez un utilisateur Marketo. Vous _ne pouvez pas_ saisir manuellement une adresse électronique.

   ![](assets/inafive-2.png)

1. Cliquez sur **Suivant**.

   ![](assets/inasix-2.png)

1. Faites correspondre chaque champ en double-cliquant sur la liste déroulante **Champ Marketo** et en sélectionnant le champ approprié. Cliquez sur **Suivant** une fois terminé.

   ![](assets/inaseven.png)

   Succès!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Vérifier l’état de l’importation&quot; affiche uniquement les trois derniers jours d’activité.

Scénarios de déduplication par nom de compte :

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importation d’un enregistrement avec le nom de compte nommé existant</strong></td> 
   <td><p>Nous mettrons à jour l’enregistrement existant</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importation d’un enregistrement avec un nouveau nom de compte nommé</strong></td> 
   <td>Nous allons créer un nouvel enregistrement</td> 
  </tr> 
 </tbody> 
</table>

Scénarios de déduplication par nom de domaine :

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importer un enregistrement avec un nouveau nom de compte et un nouveau nom de domaine</strong></td> 
   <td>Nous allons créer un nouveau compte nommé avec les informations fournies.</td> 
  </tr> 
  <tr> 
   <td><strong>Importer un enregistrement avec un nom de compte existant et un nom de domaine existant</strong></td> 
   <td>Nous mettrons à jour le compte nommé existant</td> 
  </tr> 
   <tr> 
   <td><strong>Importer un enregistrement avec un nouveau nom de compte et un nom de domaine existant</strong></td> 
   <td>Nous allons ajouter le nouveau nom de compte au compte nommé existant qui correspond au nom de domaine et mettre à jour d’autres informations (secteur, état, etc.).</td> 
  </tr> 
  <tr> 
   <td><strong>Importer un enregistrement avec le nom de compte nommé existant et le nouveau nom de domaine</strong></td> 
   <td>Nous allons ajouter le nouveau nom de domaine au compte nommé existant qui correspond au nom du compte et mettre à jour d’autres informations (secteur, état, etc.).</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Lorsque Marketo ajoute un compte nommé, nous mettons à jour une règle (en arrière-plan) qui nous permet d’identifier les personnes qui doivent faire partie du compte nommé. Exemple : si vous mettez à jour &quot;IBM&quot; vers &quot;IBM, Etats-Unis&quot;, les personnes qui portent l’un ou l’autre nom de société seront associées au compte nommé.

Si Marketo trouve des enregistrements que nous voyons comme des doublons, nous traiterons uniquement le premier.
