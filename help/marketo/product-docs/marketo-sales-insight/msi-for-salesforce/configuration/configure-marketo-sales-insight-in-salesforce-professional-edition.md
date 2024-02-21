---
unique-page-id: 3571743
description: Configuration de Marketo Sales Insight dans Salesforce Professional Edition - Documents Marketo - Documentation du produit
title: Configuration de Marketo Sales Insight dans Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 1ce807ce99e3551ffc29e59ed356423633dc2276
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 5%

---

# Configuration de Marketo Sales Insight dans Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Voici les étapes à suivre pour configurer Marketo Sales Insight dans Salesforce Professional Edition. Commençons.

>[!PREREQUISITES]
>
>* Installez Marketo dans votre Salesforce Professional Edition.
>
>* [Installation du package Marketo Sales Insight dans l’AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Configuration de Sales Insight dans Marketo {#configure-sales-insight-in-marketo}

1. Ouvrez une nouvelle fenêtre de navigateur pour obtenir les informations d’identification Marketo Sales Insight de votre compte Marketo.

1. Accédez au **Administration** zone et sélectionnez **Statistiques des ventes**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Cliquez sur **Modifier la configuration de l’API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Saisissez une clé secrète API de votre choix, puis cliquez sur **Enregistrer**. N’utilisez PAS d’esperluette (&amp;) dans votre clé secrète API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Votre clé secrète d’API est semblable à un mot de passe pour votre organisation et doit être sécurisée.

1. Cliquez sur **Affichage** dans le panneau Configuration de l’API REST pour renseigner les informations d’identification.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Vous verrez une fenêtre contextuelle de confirmation. Cliquez sur **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configuration de Sales Insight dans Salesforce {#configure-sales-insight-in-salesforce}

1. Dans Salesforce, cliquez sur **Configuration**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Recherchez &quot;site distant&quot; et sélectionnez **Paramètres du site distant**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Cliquez sur **Nouveau site distant**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Saisissez le nom du site distant (il peut s’agir de &quot;MarketoSoapAPI&quot;). Saisissez l’URL du site distant, qui est votre URL d’hôte Marketo à partir du panneau Configuration de l’API Soap de Marketo. Cliquez sur **Enregistrer**. Vous avez maintenant créé des paramètres de site distant pour l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Cliquez sur **Nouveau site distant** encore une fois.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Saisissez le nom du site distant (il peut s’agir de &quot;MarketoRestAPI&quot;). Saisissez l’URL du site distant, qui correspond à l’URL de votre API dans le panneau Configuration de l’API REST de Marketo. Cliquez sur **Enregistrer**. Vous avez maintenant créé des paramètres de site distant pour l’API REST.

## Accorder l’accès au profil des utilisateurs de Sales Insight aux objets Salesforce standard {#grant-sales-insight-users-profile-access}

En raison des améliorations apportées à la sécurité de Saleforce, les modules App Exchange ne peuvent plus accorder d’autorisation aux objets standard, et l’accès devra être accordé aux objets Salesforce appropriés à partir du profil de l’utilisateur Salesforce. Suivez les étapes ci-dessous pour accorder les autorisations nécessaires.

1. Cliquez sur **Configuration**.

1. Recherchez &quot;Profils&quot; dans Recherche rapide.

1. Cliquez sur **Modifier** en regard du profil que vos utilisateurs Salesforce utilisent.

1. Dans la section Autorisation d’objet standard , activez l’accès en lecture pour les objets suivants : prospect, contact, compte et opportunité.

1. Cliquez sur **Enregistrer**.

## Personnalisation des mises en page {#customize-page-layouts}

1. Cliquez sur **Configuration**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Recherchez &quot;mise en page&quot; et sélectionnez l’option **Disposition de page** under **Pistes**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Cliquez sur **Pages Visualforce** sur la gauche. Glisser **Section** à la disposition sous la section Liens personnalisés .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Saisissez &quot;Marketo Sales Insight&quot; comme **Nom de la section**. Sélectionner **1 colonne** et cliquez sur **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Glisser-déposer **prospect** dans la nouvelle section .

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Le nom de cette zone change en fonction du type d’objet. Par exemple, si vous modifiez la mise en page des contacts, le message Contact est affiché.

1. Double-cliquez sur le **prospect** que vous venez d&#39;ajouter.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modifier la hauteur en **450** pixels et cliquez sur **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Vérifier **Afficher les barres de défilement** si vous avez besoin d’accéder aux activités de défilement.

   >[!TIP]
   >
   >Nous recommandons une hauteur de 410 pixels pour les objets Comptes et opportunités .

1. Cliquez sur **Champs** sur la gauche. Recherchez ensuite le composant **Engagement** dans le **Marketo Sales Insight** disposition.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

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

1. Répétez cette procédure pour ajouter des sections de page Visualforce et des champs Sales Insight pour **Contact**, **Compte** et **Opportunité**.
1. Répétez les étapes 5 à 7 pour ajouter des sections de page Visualforce pour Contact, Compte et Opportunité. Répétez ensuite les étapes 8 à 10 pour ajouter des champs de statistiques sur les ventes pour **Contact**. Veillez à enregistrer après toute modification.

## Faire correspondre les champs de personne personnalisés {#map-custom-person-fields}

Les champs de personne Marketo doivent être mappés aux champs de contact Salesforce pour garantir le bon fonctionnement de la conversion. Voici comment.

1. Cliquez sur **Configuration**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Recherchez &quot;champs&quot; dans la barre de recherche, puis cliquez sur **Champs** under **Pistes**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Cliquez sur **Faire correspondre les champs de piste**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Cliquez sur le menu déroulant à droite pour **Engagement**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Sélectionner **Contact.Engagement** dans la liste.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

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

1. Cliquez sur **Enregistrer** lorsque vous avez fini.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Onglet Configuration des statistiques sur les ventes Marketo {#marketo-sales-insight-configuration-tab}

1. Dans Salesforce, cliquez sur l’icône **+** à la fin de la barre d’onglets, puis cliquez sur **Configuration de Marketo Sales Insight**.

1. Copiez les informations d’identification du panneau API Soap dans [Page d’administration de Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} et collez-les dans la section API Soap de la page de configuration Salesforce Sales Insight .

1. Copiez les informations d’identification du panneau API REST dans [Page d’administration de Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} et collez-les dans la section API REST de la page de configuration Salesforce Sales Insight .

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

Et c&#39;est tout ! Vous devriez être en mesure d’afficher les champs Marketo Sales Insight pour les Leads, les contacts, les comptes et les opportunités.

>[!NOTE]
>
>Si le test de diagnostic a échoué, vous devrez peut-être [ajouter des champs supplémentaires à la mise en page ;](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>Pour les comptes, Sales Insight inclura tous les emails, mais uniquement les derniers moments intéressants, l’activité web et les changements de score.

>[!MORELIKETHIS]
>
>* [Priorité, urgence, note relative et meilleurs paris](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Ajouter un onglet Marketo à Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Ajout de l’accès Sales Insight aux profils](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
