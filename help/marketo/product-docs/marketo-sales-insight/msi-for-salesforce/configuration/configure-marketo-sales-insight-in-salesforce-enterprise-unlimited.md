---
unique-page-id: 2360368
description: Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited - Documents Marketo - Documentation du produit
title: Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
source-git-commit: fbd8640d55a9a38936d060086f361b2281add47f
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 5%

---

# Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Voici les étapes à suivre pour configurer Marketo Sales Insight dans Salesforce Enterprise/Unlimited Editions. Commençons.

>[!PREREQUISITES]
>
>* [Installation du package Marketo Sales Insight dans l’AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
**Autorisations d’administrateur requises**

## Configuration de Sales Insight dans Marketo {#configure-sales-insight-in-marketo}

1. Ouvrez une nouvelle fenêtre de navigateur pour obtenir les informations d’identification Marketo Sales Insight de votre compte Marketo.

1. Dans la zone Admin, sélectionnez **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Cliquez sur **Modifier la configuration de l’API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Saisissez une clé secrète API de votre choix, puis cliquez sur **Enregistrer**. N’utilisez PAS d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   Votre clé secrète API est semblable à un mot de passe pour votre organisation et doit être sécurisée.

1. Cliquez sur **Afficher** dans le panneau Configuration de l’API REST pour renseigner les informations d’identification.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Une fenêtre contextuelle de confirmation s’affiche. Cliquez sur **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

## Configuration de Sales Insight dans Salesforce {#configure-sales-insight-in-salesforce}

1. Dans Salesforce, cliquez sur **Configuration**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Recherchez &quot;site distant&quot; et sélectionnez **Paramètres du site distant**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Cliquez sur **Nouveau site distant**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Saisissez le nom du site distant (il peut s’agir de &quot;MarketoSoapAPI&quot;). Saisissez l’URL du site distant, qui est votre URL d’hôte Marketo à partir du panneau Configuration de l’API Soap de Marketo. Cliquez sur **Enregistrer**. Vous avez maintenant créé des paramètres de site distant pour l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Cliquez à nouveau sur **Nouveau site distant**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Saisissez le nom du site distant (il peut s’agir de &quot;MarketoRestAPI&quot;). Saisissez l’URL du site distant, qui correspond à l’URL de votre API dans le panneau Configuration de l’API REST de Marketo. Cliquez sur **Enregistrer**. Vous avez maintenant créé des paramètres de site distant pour l’API REST.

## Configuration de Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Connectez-vous à votre instance Marketo et cliquez sur **Admin**.

   ![](assets/login-admin.png)

1. Cliquez sur **Sales Insight**.

   ![](assets/image2015-5-22-15-3a12-3a33.png)

1. Cliquez sur **Modifier la configuration de l’API**.

   ![](assets/image2015-5-22-15-3a15-3a0.png)

1. Saisissez une **clé secrète API** et cliquez sur **Enregistrer**.

   >[!CAUTION]
   N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2015-5-27-16-3a36-3a56.png)

   >[!TIP]
   Gardez cette fenêtre ouverte. Vous aurez besoin de ces informations plus tard dans Salesforce.

1. Revenez à Salesforce, cliquez sur **Configuration**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Recherchez &quot;site distant&quot; et cliquez sur **Paramètres du site distant** sous **Contrôles de sécurité**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Cliquez sur **Nouveau site distant**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Saisissez **Nom du site distant** et **URL du site distant**, puis cliquez sur **Enregistrer**.

   ![](assets/remote-site.png)

   >[!NOTE]
   Vous choisissez votre **nom du site distant** (MarketoAPI est utilisé ici). La **URL du site distant** se trouve dans le champ Hôte Marketo de la boîte de dialogue Modifier la configuration de l’API de l’étape 4.

## Personnalisation des mises en page {#customize-page-layouts}

1. Cliquez sur **Configuration**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Recherchez &quot;mise en page&quot; et sélectionnez **Mise en page** sous **Pistes**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Cliquez sur **Pages Visualforce** à gauche. Faites glisser **Section** vers la disposition sous la section Liens personnalisés .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Saisissez &quot;Marketo Sales Insight&quot; comme **Nom de la section**. Sélectionnez **1-Column** et cliquez sur **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Faites glisser **Lead** dans la nouvelle section.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   Le nom de cette zone change en fonction du type d’objet. Par exemple, si vous modifiez la mise en page des contacts, le message Contact est affiché.

1. Double-cliquez sur le bloc **Lead** que vous venez d’ajouter.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Editez la hauteur à **450** pixels et cliquez sur **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   Nous recommandons une hauteur de 410 pixels pour les objets Comptes et opportunités .

1. Cliquez sur **Champs** à gauche. Recherchez ensuite le libellé **Engagement** et faites-le glisser dans la disposition **Marketo Sales Insight**.

   ![](assets/image2015-5-22-16-3a32-3a46.png)

1. Répétez également l’étape ci-dessus pour ces champs.

   <table> 
    <tbody> 
     <tr> 
      <td colspan="1">Engagement</td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valeur d'évaluation relative</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valeur d'urgence</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Date dernier moment significatif</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Description dernier moment significatif</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Source dernier moment significatif</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Type dernier moment significatif</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Répétez cette procédure pour ajouter des sections de page Visualforce et des champs de statistiques sur les ventes pour **Contact**, **Compte** et **Opportunité**.

1. Répétez les étapes 5 à 7 pour ajouter des sections de page Visualforce pour Contact, Compte et Opportunité. Répétez ensuite les étapes 8 à 10 pour ajouter les champs de statistiques sur les ventes pour **Contact**. Veillez à enregistrer après toute modification.

## Faire correspondre les champs de personne personnalisés {#map-custom-person-fields}

Les champs de personne Marketo doivent être mappés aux champs de contact Salesforce pour garantir le bon fonctionnement de la conversion. Voici comment.

1. Cliquez sur **Configuration**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Recherchez &quot;fields&quot; dans la barre de recherche et cliquez sur **Champs** sous **Pistes**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Cliquez sur **Faire correspondre les champs de piste**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Cliquez sur la liste déroulante à droite de **Engagement**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Sélectionnez **Contact.Engagement** dans la liste.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Répétez et mappez également ces champs.

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Champ personnalisé de personne Marketo</th> 
      <th colspan="1" rowspan="1">Champ personnalisé Contact Salesforce</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Engagement</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valeur d'évaluation relative</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Valeur de score relative</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valeur d'urgence</p></td> 
      <td colspan="1" rowspan="1"><p>Valeur Contact.Urgency</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Date dernier moment significatif</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last intéressant Moment Date</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Description dernier moment significatif</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last intéressant Moment Desc</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Source dernier moment significatif</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last intéressant Moment Source</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Type dernier moment significatif</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last intéressant Moment Type</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

## Configuration de Marketo Sales Insight {#marketo-sales-insight-config}

1. Cliquez sur **+**, puis sélectionnez **Marketo Sales Insight Config**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Cochez **Activer l’API Marketo**. Renseignez ensuite les [informations de configuration de l’API dans Marketo Admin](#set-up-marketo-sales-insight). Cliquez sur **Enregistrer les modifications** lorsque vous avez terminé.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   Si le test de diagnostic a échoué, vous devrez peut-être [ajouter d’autres champs à la mise en page](https://nation.marketo.com/docs/DOC-1115).

Et voilà ! Vous devriez être en mesure d’afficher les champs Marketo Sales Insight pour les Leads, les contacts, les comptes et les opportunités.

![](assets/twenty-six.png)

>[!NOTE]
Pour les comptes, Sales Insight inclura tous les emails, mais uniquement les derniers moments intéressants, l’activité web et les changements de score.

## Accès Sales Insight de Marketo {#access-marketo-sales-insight}

1. Dans Salesforce, cliquez sur **+** à la fin de la barre d’onglets et cliquez sur **Marketo Sales Insight Config**.

1. Cochez la case **Activer l’API Marketo** .

1. Copiez les informations d’identification à partir du panneau API Soap de la page d’administration des statistiques sur les ventes de Marketo et collez-les dans la section API Soap de la page de configuration des statistiques sur les ventes de Salesforce.

1. Copiez les informations d’identification du panneau API REST dans la page d’administration des statistiques sur les ventes de Marketo et collez-les dans la section API REST de la page de configuration des statistiques sur les ventes de Salesforce.

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
* [Priorité, urgence, note relative et meilleurs paris](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
* [Ajout de l’onglet Statistiques sur les ventes Marketo et de boutons à Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)
* [Configuration de Sales Insight pour votre équipe](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)

