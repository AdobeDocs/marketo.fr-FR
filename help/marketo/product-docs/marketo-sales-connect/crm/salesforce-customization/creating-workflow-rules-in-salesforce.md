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
>Cela affecte uniquement les clients qui utilisent **both** MSI et MSE, et qui souhaitent utiliser la fonctionnalité Meilleurs paris de MSI. Si vous n’avez pas besoin d’utiliser les meilleurs paris, vous pouvez ignorer.

## Premiers pas {#getting-started}

La solution de contournement consiste à créer de nouvelles règles de workflow pour copier les valeurs des nouveaux champs MSE dans les anciens champs MSI. Vous devez créer quatre règles de workflow pour l’objet Contact et les mêmes quatre règles de workflow pour l’objet Lead dans votre propre instance Salesforce. Pour ce faire, vous devrez peut-être disposer des droits d’administrateur CRM (en fonction de votre rôle et de votre configuration dans le CRM).

Vous trouverez ci-dessous les noms recommandés des règles de workflow et la description de chacune d’elles. Ils s’appliquent à l’objet Contact et Lead :

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Mettre à jour le champ Desc Moment intéressant</td> 
   <td><p>Copier depuis : Dernier engagement Marketo Desc<br>Copier vers : Dernier moment intéressant Desc</p></td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le champ Type de moment intéressant</td> 
   <td><p>Copier depuis : Dernier type d’engagement Marketo<br>Copier vers : Dernier type de moment intéressant</p></td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le champ source du moment intéressant</td> 
   <td><p>Copier depuis : Dernière source d’engagement Marketo<br>Copier vers : Dernière source intéressante</p></td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le champ Date du moment intéressant</td> 
   <td><p>Copier depuis : Date de la dernière interaction Marketo<br>Copier vers : Date du dernier moment intéressant</p></td> 
  </tr> 
 </tbody> 
</table>

## Instructions {#instructions}

1. Après avoir cliqué sur **Configuration**, recherchez **Workflow** et sélectionnez **Règles de workflow**.

   ![](assets/one-1.png)

1. Sélectionner **Nouvelle règle**.

   ![](assets/two-1.png)

1. Cliquez sur la liste déroulante Objet et sélectionnez **prospect**, puis cliquez sur **Suivant**.

   ![](assets/three-1.png)

1. Saisissez &quot;Mettre à jour le champ Desc Moment intéressant&quot; comme nom de la règle. Sélectionner le bouton radio **créé et modifié à chaque fois**. Dans la liste déroulante Critères de règle , sélectionnez **la formule renvoie true (vrai)**. Recherchez et sélectionnez la fonction ISCHANGED. Mettez ensuite la valeur de champ par défaut en surbrillance et cliquez sur **Champ d’insertion**.

   ![](assets/four-1.png)

1. Dans la fenêtre contextuelle &quot;Insérer un champ&quot;, choisissez **Dernier engagement Marketo Desc** et cliquez sur **Insérer**.

   ![](assets/five-1.png)

1. Cliquez sur **Enregistrer et suivant**.

   ![](assets/6.png)

1. Dans la liste déroulante Ajouter une action de processus , sélectionnez **Nouvelle mise à jour des champs**.

   ![](assets/seven.png)

1. Dans le champ Nom , saisissez &quot;Mettre à jour le champ Desc du moment intéressant&quot; (le nom unique est généré automatiquement). Dans la liste déroulante Champ à mettre à jour , choisissez **Dernier moment intéressant Desc**. Sélectionnez la **Utiliser une formule pour définir une nouvelle valeur** bouton radio, puis cliquez sur **Afficher l’éditeur de formules**.

   ![](assets/eight.png)

1. Cliquez sur le bouton **Champ d’insertion** bouton .

   ![](assets/9a.png)

1. Sélectionner **Dernier engagement Marketo Desc**, puis cliquez sur **Insérer**. Sur la page suivante, cliquez sur **Enregistrer**.

   ![](assets/nine.png)

1. Cliquez sur **Terminé**.

   ![](assets/twelve.png)

1. Cliquez sur **Activer** pour activer la règle de workflow.

   ![](assets/thirteen.png)

   Après la dernière étape, vous pouvez choisir de cloner la règle de workflow pour les autres champs répertoriés dans la section Prise en main : Desc, Type, Source, Date. Une fois que vous avez terminé les quatre règles de workflow dans l’objet Contact, répétez la même chose pour l’objet Lead.
