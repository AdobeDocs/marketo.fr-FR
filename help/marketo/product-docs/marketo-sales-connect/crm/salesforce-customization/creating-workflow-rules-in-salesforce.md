---
unique-page-id: 14745823
description: Création de règles de workflow dans Salesforce - Documents Marketo - Documentation du produit
title: Création de règles de workflow dans Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---

# Création de règles de workflow dans Salesforce {#creating-workflow-rules-in-salesforce}

Lorsque vous utilisez Marketo Sales Insight (MSI) et Marketo Sales Connect (MSC) en parallèle, la fonctionnalité Meilleurs résultats MSI de [!DNL Salesforce] n’est pas mise à jour. Toutes les autres fonctionnalités MSI fonctionnent comme d&#39;habitude (affichage des moments intéressants dans l&#39;iFrame, envoi d&#39;e-mails, ajout aux campagnes, etc.). Cet article offre une solution pour que les meilleurs résultats fonctionnent à nouveau.

>[!NOTE]
>
>Cela n’affecte que les clients qui utilisent **à la fois** MSI et MSE, et qui souhaitent utiliser la fonctionnalité Meilleurs résultats dans MSI. Si vous n&#39;avez pas besoin/n&#39;utilisez pas les meilleurs paris, vous pouvez les ignorer.

## Prise en main {#getting-started}

La solution consiste à créer de nouvelles règles de workflow pour copier les valeurs des nouveaux champs MSI dans les anciens champs MSI. Vous devez créer quatre règles de workflow pour l’objet Contact et les mêmes quatre règles de workflow pour l’objet Lead dans votre propre instance [!DNL Salesforce]. Cela peut nécessiter que vous disposiez des droits d’administrateur CRM (selon votre rôle et la configuration dans le CRM).

Vous trouverez ci-dessous les noms recommandés des règles de workflow et leur description. Ils s’appliquent à l’objet [!UICONTROL Contact] et [!UICONTROL Lead] :

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td>Mettre à jour le champ de description du moment intéressant</td>
   <td><p>Copier à partir de : Desc Dernier engagement Marketo<br>Copier vers : Desc Dernier moment intéressant</p></td>
  </tr>
  <tr>
   <td>Mettre à jour le champ Type de moment intéressant</td>
   <td><p>Copier à partir de : dernier type d’engagement Marketo<br>Copier vers : dernier type de moment intéressant</p></td>
  </tr>
  <tr>
   <td>Mettre à jour le champ Source du moment intéressant</td>
   <td><p>Copier à partir de : dernier engagement Marketo Source<br>Copier vers : dernier moment intéressant Source</p></td>
  </tr>
  <tr>
   <td>Mettre à jour le champ Date du moment intéressant</td>
   <td><p>Copier à partir de : Date du dernier engagement dans Marketo<br>Copier vers : Date du dernier moment intéressant</p></td>
  </tr>
 </tbody>
</table>

## Instructions {#instructions}

1. Après avoir cliqué sur **[!UICONTROL Configuration]**, recherchez **Workflow** et sélectionnez **[!UICONTROL Règles de workflow]**.

   ![](assets/one-1.png)

1. Sélectionnez **[!UICONTROL Nouvelle règle]**.

   ![](assets/two-1.png)

1. Cliquez sur la liste déroulante [!UICONTROL Objet] et sélectionnez **[!UICONTROL Lead]**, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/three-1.png)

1. Saisissez « Mettre à jour le champ de description du moment intéressant » comme [!UICONTROL  Nom de la règle ]. Sélectionnez le bouton radio **[!UICONTROL créé, puis chaque fois qu’il est modifié]**. Dans le menu déroulant [!UICONTROL Critères de règle], sélectionnez **[!UICONTROL la formule est évaluée sur true]**. Recherchez et sélectionnez la fonction ISCHANGED. Ensuite, mettez en surbrillance la valeur de champ par défaut et cliquez sur **[!UICONTROL Insérer un champ]**.

   ![](assets/four-1.png)

1. Dans le pop-up « [!UICONTROL Insérer le champ] », choisissez **[!UICONTROL Dernière description de l’engagement Marketo]** et cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/five-1.png)

1. Cliquez sur **[!UICONTROL Enregistrer et suivant]**.

   ![](assets/6.png)

1. Dans la liste déroulante [!UICONTROL  Ajouter une action de workflow ], sélectionnez **[!UICONTROL Nouvelle mise à jour de champ]**.

   ![](assets/seven.png)

1. Dans le champ [!UICONTROL Nom], saisissez « Mettre à jour le champ de description du moment intéressant » ([!UICONTROL Nom unique] sera généré automatiquement). Dans la liste déroulante [!UICONTROL Champ à mettre à jour], choisissez **[!UICONTROL Dernière description du moment intéressant]**. Sélectionnez le bouton radio **[!UICONTROL Utiliser une formule pour définir une nouvelle valeur]** puis cliquez sur **[!UICONTROL Afficher l&#39;éditeur de formule]**.

   ![](assets/eight.png)

1. Cliquez sur le bouton **[!UICONTROL Insérer un champ]**.

   ![](assets/9a.png)

1. Sélectionnez **[!UICONTROL Dernière conception d’engagement Marketo]**, puis cliquez sur **[!UICONTROL Insérer]**. Sur la page suivante, cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/nine.png)

1. Cliquez sur **[!UICONTROL Terminé]**.

   ![](assets/twelve.png)

1. Cliquez sur **[!UICONTROL Activer]** pour activer la règle de workflow.

   ![](assets/thirteen.png)

   Après la dernière étape, vous pouvez choisir de cloner la règle de workflow pour les autres champs répertoriés dans la section [!UICONTROL Prise en main] : Desc, Type, Source, Date. Une fois les quatre règles de workflow de l’objet [!UICONTROL Contact] terminées, répétez la même opération pour l’objet [!UICONTROL Lead].
