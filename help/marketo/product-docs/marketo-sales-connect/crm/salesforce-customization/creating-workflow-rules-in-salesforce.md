---
unique-page-id: 14745823
description: Création de règles de processus dans Salesforce - Documents Marketo - Documentation du produit
title: Création de règles de processus dans Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Création de règles de processus dans Salesforce {#creating-workflow-rules-in-salesforce}

Lors de l’utilisation de Marketo Sales Insight (MSI) et Marketo Sales Connect (MSC) en parallèle, la fonctionnalité MSI Best Bets (Meilleurs jeux MSI) dans Salesforce ne sera pas mise à jour. Toutes les autres fonctionnalités MSI fonctionnent normalement (affichage de moments intéressants dans l’iFrame, envoi d’emails, ajout à des campagnes, etc.). Cet article propose une solution pour que les meilleurs paris fonctionnent à nouveau.

>[!NOTE]
>
>Cela concerne uniquement les clients qui utilisent **à la fois** MSI et MSE, et qui souhaitent utiliser la fonctionnalité Meilleurs paris dans MSI. Si vous n’avez pas besoin d’utiliser les meilleurs paris, vous pouvez ignorer.

## Prise en main {#getting-started}

La solution de contournement consiste à créer de nouvelles règles de workflow pour copier les valeurs des nouveaux champs MSE dans les anciens champs MSI. Vous devez créer quatre règles de workflow pour l’objet Contact et les mêmes quatre règles de workflow pour l’objet Lead dans votre propre instance Salesforce. Pour ce faire, vous devrez peut-être disposer des droits d’administrateur CRM (en fonction de votre rôle et de votre configuration dans le CRM).

Vous trouverez ci-dessous les noms recommandés des règles de workflow et leur description. Ils s’appliquent à l’objet Contact et Lead :

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Mettre à jour le champ Desc Moment intéressant</td> 
   <td><p>Copier de : Dernier engagement Marketo Desc<br>Copier vers : Dernier moment intéressant Desc</p></td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le champ Type de moment intéressant</td> 
   <td><p>Copier depuis : dernier type d’engagement Marketo<br>Copier vers : dernier type de moment intéressant</p></td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le champ Source de moment intéressant</td> 
   <td><p>Copier de : dernier Marketo Engagement Source<br>Copier vers : dernier moment intéressant Source</p></td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le champ Date du moment intéressant</td> 
   <td><p>Copier de : Date du dernier engagement Marketo<br>Copier vers : Date du dernier moment intéressant</p></td> 
  </tr> 
 </tbody> 
</table>

## Instructions {#instructions}

1. Après avoir cliqué sur **Setup**, recherchez **Workflow** et sélectionnez **Workflow Rules**.

   ![](assets/one-1.png)

1. Sélectionnez **Nouvelle règle**.

   ![](assets/two-1.png)

1. Cliquez sur la liste déroulante Objet et sélectionnez **Lead**, puis cliquez sur **Next**.

   ![](assets/three-1.png)

1. Saisissez &quot;Mettre à jour le champ Desc Moment intéressant&quot; comme nom de la règle. Sélectionnez le bouton radio **créé, et chaque fois qu’il est modifié**. Dans la liste déroulante Critères de règle , sélectionnez **formule = true**. Recherchez et sélectionnez la fonction ISCHANGED. Mettez ensuite la valeur de champ par défaut en surbrillance et cliquez sur **Insérer le champ**.

   ![](assets/four-1.png)

1. Dans la fenêtre contextuelle &quot;Insérer un champ&quot;, sélectionnez **Last Marketo Engagement Desc** et cliquez sur **Insérer**.

   ![](assets/five-1.png)

1. Cliquez sur **Enregistrer et suivant**.

   ![](assets/6.png)

1. Dans la liste déroulante Ajouter une action de workflow , sélectionnez **Nouvelle mise à jour de champ**.

   ![](assets/seven.png)

1. Dans le champ Nom , saisissez &quot;Mettre à jour le champ Desc du moment intéressant&quot; (le nom unique est généré automatiquement). Dans la liste déroulante Champ à mettre à jour , sélectionnez **Dernier moment intéressant Desc**. Sélectionnez le bouton radio **Utiliser une formule pour définir une nouvelle valeur** , puis cliquez sur **Afficher l’éditeur de formule**.

   ![](assets/eight.png)

1. Cliquez sur le bouton **Insérer un champ** .

   ![](assets/9a.png)

1. Sélectionnez **Last Marketo Engagement Desc**, puis cliquez sur **Insérer**. Sur la page suivante, cliquez sur **Enregistrer**.

   ![](assets/nine.png)

1. Cliquez sur **Terminé**.

   ![](assets/twelve.png)

1. Cliquez sur **Activer** pour activer la règle de workflow.

   ![](assets/thirteen.png)

   Après la dernière étape, vous pouvez choisir de cloner la règle de workflow pour les autres champs répertoriés dans la section Prise en main : Desc, Type, Source, Date. Une fois que vous avez terminé les quatre règles de workflow dans l’objet Contact, répétez la même chose pour l’objet Lead.
