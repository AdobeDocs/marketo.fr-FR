---
unique-page-id: 12615800
description: Importer des comptes nommés - Documents marketing - Documentation du produit
title: Importer des comptes nommés
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---


# Importer des comptes nommés {#import-named-accounts}

Avez-vous déjà un fichier CSV rempli de comptes de cible potentiels ? Importez-les directement dans ABM !

1. Cliquez sur la liste déroulante **New** et sélectionnez **Importer des comptes nommés**.

   ![](assets/inaone.png)

1. Une nouvelle fenêtre s&#39;ouvre. Cliquez sur **Parcourir**, puis sélectionnez le fichier des comptes nommés à importer.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Dans votre fichier, fournissez [autant d&#39;informations](/help/marketo/product-docs/account-based-marketing/target/named-accounts/named-account-overview.md#named-account-attributes) que possible. Vous pouvez uniquement ajouter des informations de fimographie ; rien que Marketo calcule (c.-à-d. Pipeline). Pour créer des comptes nommés basés sur des comptes CRM, il vous suffit d’exporter le nom du compte et l’identifiant de gestion de la relation client de votre gestion de la relation client dans un fichier CSV, d’utiliser l’option Nom du compte et de mapper l’identifiant de gestion de la relation client au cours du processus d’importation. Pour lier correctement un compte CRM à un compte nommé, vous devez indiquer le nom exact du compte CRM.

1. Choisissez entre deux modes de déduplication : Nom du compte ou nom de domaine. Dans cet exemple, nous allons choisir Compte. Cliquez sur la liste déroulante **Modes** et sélectionnez **Par nom de compte**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Si vous choisissez **Par mode de domaine**, les champs de compte et de domaine nommés doivent être inclus.

1. Pour choisir à quelle liste de compte votre compte nommé est ajouté, cliquez sur la liste déroulante **Liste de compte** et faites votre sélection.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Vous pouvez également créer une toute nouvelle Liste de compte en saisissant simplement son nom dans la liste déroulante.

1. Pour envoyer une notification de l’importation, cliquez sur la liste déroulante **Envoyer l’alerte à** et sélectionnez un utilisateur Marketing. Vous _ne pouvez pas_ saisir manuellement une adresse électronique.

   ![](assets/inafive-2.png)

1. Cliquez sur **Suivant**.

   ![](assets/inasix-2.png)

1. Faites correspondre chaque champ en cliquant sur le doublon dans la liste déroulante **Champ marketing** et en sélectionnant le champ approprié. Cliquez sur **Suivant** lorsque vous avez terminé.

   ![](assets/inaseven.png)

   Succès !

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Vérifier l’état de l’importation&quot; affiche uniquement les trois derniers jours d’activité.

Scénarios lorsque vous dédupliquez par nom de compte :

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importation d’un enregistrement avec un nom de compte nommé existant</strong></td> 
   <td><p>Nous mettrons à jour l'enregistrement existant</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importation d’un enregistrement avec un nouveau nom de compte nommé</strong></td> 
   <td>Nous créerons un nouvel enregistrement</td> 
  </tr> 
 </tbody> 
</table>

Scénarios lorsque vous dédupliquez par nom de domaine :

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importation d’un enregistrement avec un nouveau nom de compte et un nouveau nom de domaine</strong></td> 
   <td>Nous créerons un nouveau compte nommé avec les informations fournies.</td> 
  </tr> 
  <tr> 
   <td><strong>Importation d’un enregistrement avec un nom de compte existant et un nom de domaine existant</strong></td> 
   <td>Nous mettrons à jour le compte nommé existant</td> 
  </tr> 
   <tr> 
   <td><strong>Importation d’un enregistrement avec un nouveau nom de compte et un nom de domaine existant</strong></td> 
   <td>Nous allons ajouter le nouveau nom de compte au compte nommé existant qui correspond au nom de domaine et mettre à jour d'autres informations (industrie, état, etc.)</td> 
  </tr> 
  <tr> 
   <td><strong>Importation d’un enregistrement avec le nom de compte nommé existant et le nouveau nom de domaine</strong></td> 
   <td>Nous allons ajouter le nouveau nom de domaine au compte nommé existant qui correspond au nom du compte et mettre à jour d'autres informations (industrie, état, etc.)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Lorsque Marketo ajoute un compte nommé, nous mettons à jour une règle (en arrière-plan) qui nous permet d’identifier les personnes qui doivent faire partie du compte nommé. Exemple : si vous mettez à jour &quot;IBM&quot; vers &quot;IBM, USA&quot;, les personnes portant l’un ou l’autre nom de société seront associées au compte nommé.

Si Marketo trouve des enregistrements que nous considérons comme des duplicata, nous ne traiterons que le premier.
