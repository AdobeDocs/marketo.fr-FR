---
description: Connexion des attributs d’activité de vente à Salesforce - Documents Marketo - Documentation du produit
title: Connexion des attributs d’activité de vente à Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 29%

---

# Connexion des attributs d’activité de vente à Salesforce {#logging-sales-activity-attributes-to-salesforce}

L’administrateur Salesforce peut ajouter manuellement des champs d’activité personnalisés à Salesforce.

1. Dans votre compte Salesforce, cliquez sur **Configuration**.

1. Recherchez &quot;Champs personnalisés de l’activité&quot; dans le champ de recherche rapide et cliquez dessus.

1. Cliquez sur **New**.

1. Sélectionnez Type de données correspondant au champ à ajouter en fonction du tableau ci-dessous et cliquez sur **Suivant**.

1. Saisissez le Nom du champ et le libellé correspondant au champ à ajouter.

Description de chaque colonne du tableau ci-dessous :

* **Libellé du champ** : nom de champ affiché dans l’interface utilisateur (ce nom peut être personnalisé pour améliorer la lisibilité de votre équipe)
* **Nom du champ** : nom technique du champ (assurez-vous que le nom du champ que vous saisissez correspond au nom du champ dans le tableau ci-dessous)
* **Nom de l’API** : nom technique du champ pour l’API (assurez-vous que le nom de l’API que vous saisissez correspond au nom de l’API dans le tableau ci-dessous)
* **Type de données** : type de champ
* **Taille** : taille du champ de texte

<table>
 <tr>
  <th>Intitulé de champ</th>
  <th>Nom de champ</th>
  <th>Nom de l'API</th>
  <th>Type de données</th>
  <th>Taille</th>
 </tr>
  <tr>
  <td>Résultats des appels</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result__c</td>
  <td>Texte</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Raisons de l’appel</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Texte</td>
  <td>50</td>
 </tr>
 <tr>
  <td>ID de présence locale de l’appel Marketo Sales</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Texte</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de l’enregistrement de l’appel Marketo Sales</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Campagne Marketo Sales</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Texte</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Étape de campagne Marketo Sales actuelle</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Texte</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de campagne Marketo Sales</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Pièce jointe d’e-mail Marketo Sales ouverte</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Case à cocher</td>
  <td></td>
 </tr>
 <tr>
  <td>E-mail Marketo Sales cliqué</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Case à cocher</td>
  <td></td>
 </tr>
 <tr>
  <td>A répondu à l’e-mail Marketo Sales</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>Case à cocher</td>
  <td></td>
 </tr>
 <tr>
  <td>Statut d’e-mail Marketo Sales</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Texte</td>
  <td></td>
 </tr>
 <tr>
  <td>Modèle d’e-mail Marketo Sales</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Texte</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL de modèle d’e-mail Marketo Sales</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>URL d’e-mail Marketo Sales</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>E-mail Marketo Sales consulté</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>Case à cocher</td>
  <td></td>
 </tr>
</table>
