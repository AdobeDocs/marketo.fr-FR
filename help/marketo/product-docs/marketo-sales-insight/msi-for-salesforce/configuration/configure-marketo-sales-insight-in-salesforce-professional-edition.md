---
unique-page-id: 3571743
description: Configuration de Marketo Sales Insight dans Salesforce Professional Edition - Marketo Docs - Documentation sur les produits
title: Configuration de Marketo Sales Insight dans Salesforce Professional Edition
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---


# Configuration de Marketo Sales Insight dans Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Vous trouverez ci-dessous les étapes à suivre pour configurer Marketo Sales Insight dans Salesforce Professional Edition. Commençons.

>[!PREREQUISITES]
>
>* Installez Marketo dans votre Salesforce Professional Edition.
   >
   >
* [Installation du package Marketing Cloud Sales Insight dans l’AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Configurer Sales Insight dans Marketo {#configure-sales-insight-in-marketo}

1. Ouvrez une nouvelle fenêtre de navigateur pour obtenir les informations d’identification de Marketing Cloud Sales Insight à partir de votre compte Marketo.
1. Accédez à la zone Admin et sélectionnez **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Cliquez sur **Modifier la configuration de l&#39;API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Saisissez une clé secrète d’API de votre choix et cliquez sur **Enregistrer**. N’utilisez PAS d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Votre clé secrète d&#39;API est un mot de passe pour votre entreprise et doit être sécurisée.

1. Cliquez sur **Vue** dans le panneau Configuration de l’API REST pour renseigner les informations d’identification.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Une fenêtre contextuelle de confirmation s’affiche. Cliquez sur **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configurer Sales Insight dans Salesforce {#configure-sales-insight-in-salesforce}

1. Dans Salesforce, cliquez sur **Configuration**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Recherchez &quot;site distant&quot; et sélectionnez **Paramètres du site distant**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Cliquez sur **Nouveau site distant**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Saisissez le nom du site distant (il peut s’agir de &quot;MarketoSoapAPI&quot;). Saisissez l’URL du site distant, qui correspond à l’URL de l’hôte de marketing depuis le panneau Configuration de l’API Soap de Marketo. Cliquez sur **Enregistrer**. Vous avez maintenant créé des paramètres de site distant pour l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Cliquez à nouveau sur **Nouveau site distant**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Saisissez le nom du site distant (il peut s’agir de &quot;MarketoRestAPI&quot;). Saisissez l’URL du site distant, qui correspond à l’URL de votre API depuis le panneau de configuration de l’API REST de Marketo. Cliquez sur **Enregistrer**. Vous avez maintenant créé des paramètres de site distant pour l’API REST.

## Configurer le rapport commercial {#set-up-marketo-sales-insight}

1. Connectez-vous à votre instance Marketo et cliquez sur **Admin**.

   ![](assets/login-admin-1.png)

1. Cliquez sur **Sales Insight**.

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. Cliquez sur **Modifier la configuration de l&#39;API**.

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. Saisissez une **clé secrète API** et cliquez sur **Enregistrer**.

   >[!CAUTION]
   >
   >N’utilisez pas d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >Garde cette fenêtre ouverte. Vous aurez besoin de cette information plus tard dans Salesforce.

1. Revenez à Salesforce, cliquez sur **Configuration**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Recherchez &quot;site distant&quot; et cliquez sur **Paramètres du site distant** sous **Contrôles de sécurité**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Cliquez sur **Nouveau site distant**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Saisissez **Nom du site distant** et **URL du site distant**, puis cliquez sur **Enregistrer**.

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >Vous choisissez votre **nom du site distant** (MarketoAPI est utilisé ici). L&#39;**URL du site distant** se trouve dans le champ Hôte de marketing de la boîte de dialogue Modifier la configuration de l&#39;API de l&#39;étape 4.

## Personnaliser les mises en page {#customize-page-layouts}

1. Cliquez sur **Configuration**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Recherchez &quot;mise en page&quot; et sélectionnez **Mise en page** sous **Pistes**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Cliquez sur **Visualforce Pages** sur la gauche. Faites glisser **Section** vers la mise en page sous la section Liens personnalisés.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Saisissez &quot;Marketo Sales Insight&quot; comme **Nom de la section**. Sélectionnez **1-Column** et cliquez sur **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Faites glisser **Piste** dans la nouvelle section.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Le nom de cette zone change en fonction du type d’objet. Par exemple, si vous modifiez la mise en page des contacts, il indique Contact.

1. Doublon-cliquez sur le bloc **Piste** que vous venez d&#39;ajouter.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modifiez la hauteur en **450** pixels et cliquez sur **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >Nous vous recommandons une hauteur de 410 pixels pour les objets Comptes et Opportunités.

1. Cliquez sur **Champs** à gauche. Recherchez ensuite le libellé **Engagement** et faites-le glisser dans la mise en page **Marketing Sales Insight**.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Répétez également l’étape ci-dessus pour ces champs.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Engagement</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valeur de score relative</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valeur d’urgence</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Date du dernier moment intéressant</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Dernier moment intéressant Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Dernière source intéressante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Dernier type de moment intéressant</p></td> 
  </tr> 
 </tbody> 
</table>

1. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Répétez ce processus pour ajouter des sections de page Visualforce et des champs Sales Insight pour **Contact**, **Compte** et **Opportunité**.
1. Répétez les étapes 5 à 7 pour ajouter des sections de page Visualforce pour Contact, Compte et Opportunité. Ensuite, répétez les étapes 8 à 10 pour ajouter les champs Sales Insight pour **Contact**. Veillez à enregistrer après toute modification.

## Mettre en correspondance les champs de personne personnalisée {#map-custom-person-fields}

Les champs de personne à personne doivent être mappés aux champs de contact Salesforce pour s’assurer que la conversion fonctionne correctement. Voici comment.

1. Cliquez sur **Configuration**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Recherchez &quot;champs&quot; dans la barre de recherche et cliquez sur **Champs** sous **Pistes**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Cliquez sur **Faire correspondre les champs de piste**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Cliquez sur la liste déroulante à droite pour **Engagement**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Sélectionnez **Contact.Engagement** dans la liste.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Répétez et mappez également ces champs.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Champ personnalisé Personne du marketing</th> 
   <th colspan="1" rowspan="1">Champ personnalisé Contact Salesforce</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Engagement</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valeur de score relative</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Valeur de note relative</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valeur d’urgence</p></td> 
   <td colspan="1" rowspan="1"><p>Valeur Contact.Urgence</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Date du dernier moment intéressant</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Dernière date intéressante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Dernier moment intéressant Desc</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Dernier moment intéressant Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Dernière source intéressante</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Dernière source de moment intéressante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Dernier type de moment intéressant</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Dernier type de moment intéressant</p></td> 
  </tr> 
 </tbody> 
</table>

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Config des statistiques commerciales de marketing {#marketo-sales-insight-config}

1. Cliquez sur **+**, puis sélectionnez **Config des statistiques commerciales du marketing**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Cochez **Activer l’API de marketing**. Renseignez ensuite les informations de configuration de l’API [dans l’élément Administration de marketing](#set-up-marketo-sales-insight). Cliquez sur **Enregistrer les modifications** lorsque vous avez terminé.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Si le test de diagnostic a échoué, vous devrez peut-être [ajouter d&#39;autres champs à votre mise en page](https://nation.marketo.com/docs/DOC-1115).

Et c&#39;est tout ! Vous devriez être en mesure d&#39;afficher les champs de statistiques de ventes de Marketo pour les pistes, contacts, comptes et opportunités.

![](assets/twenty-six-1.png)

>[!NOTE]
>
>Pour les comptes, Sales Insight inclura tous les e-mails, mais uniquement les derniers moments intéressants, l&#39;activité Web et les changements de notes.

## Accéder à Marketing Sales Insight {#access-marketo-sales-insight}

1. Dans Salesforce, cliquez sur le **+** à la fin de la barre d’onglets et cliquez sur **Config des statistiques commerciales du marketing**.

1. Cochez la case **Activer l’API de marketing**.

1. Copiez les informations d’identification du panneau API Soap de la page d’administration de Sales Insight de Marketo et collez-les dans la section API Soap de la page de configuration de Sales Insight de Salesforce.

1. Copiez les informations d’identification du panneau API REST de la page d’administration de Sales Insight de Marketo et collez-les dans la section API REST de la page de configuration de Sales Insight de Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

>[!MORELIKETHIS]
>
>* [Priorité, urgence, note relative et meilleurs résultats](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Ajouter l&#39;onglet et les boutons d&#39;aperçu commercial du marketing à Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)
>* [Configuration de Sales Insight pour votre équipe](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)

