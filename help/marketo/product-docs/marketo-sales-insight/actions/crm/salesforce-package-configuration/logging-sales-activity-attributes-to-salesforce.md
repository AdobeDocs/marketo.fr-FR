---
description: Journalisation des attributs d’activité commerciale dans Salesforce - Documents Marketo - Documentation du produit
title: Journalisation des attributs des activités de vente dans Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 12%

---

# Consignation des attributs d’activité de vente à [!DNL Salesforce] {#logging-sales-activity-attributes-to-salesforce}

L’administrateur Salesforce peut ajouter manuellement des champs d’activité personnalisés aux [!DNL Salesforce].

1. Dans votre compte [!DNL Salesforce], cliquez sur **[!UICONTROL Configurer]**.

1. Recherchez « Champs personnalisés d’activité » dans le champ de recherche rapide et cliquez dessus.

1. Cliquez sur **[!UICONTROL Nouveau]**.

1. Sélectionnez le Type de données correspondant au champ que vous souhaitez ajouter en fonction du tableau ci-dessous et cliquez sur **[!UICONTROL Suivant]**.

1. Saisissez le Nom du champ et le libellé correspondant au champ que vous souhaitez ajouter.

Description de chaque colonne du tableau ci-dessous :

* **Libellé du champ** : nom du champ affiché dans l’interface utilisateur (ce nom peut être personnalisé pour améliorer la lisibilité par votre équipe).
* **Nom du champ** : nom technique du champ (assurez-vous que le nom du champ que vous saisissez correspond au nom du champ dans le tableau ci-dessous).
* **Nom de l’API** : nom technique du champ pour l’API (assurez-vous que le nom d’API saisi correspond au nom de l’API indiqué dans le tableau ci-dessous)
* **Type de données** : type de champ
* **Size** : taille du champ de texte

<table>
 <tr>
  <th>Intitulé de champ</th>
  <th>Nom du champ</th>
  <th>Nom de l'API</th>
  <th>Type de données</th>
  <th>Taille</th>
 </tr>
  <tr>
  <td>[!UICONTROL Call Outcomes]</td>
  <td>motosales_call_result</td>
  <td>mktosales_call_result__c</td>
  <td>Texte</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Call REASONS]</td>
  <td>motosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Texte</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Local Presence ID]</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Texte</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Recording URL]</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign]</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Texte</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign Current Step]</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Texte</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign URL]</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Attachment Viewed]</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Case à cocher</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Clicked]</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Case à cocher</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Reply]</td>
  <td>MSE_Answed</td>
  <td>MSE_Replied__c</td>
  <td>Case à cocher</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Status]</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Texte</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template]</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Texte</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template URL]</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email URL]</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Viewed]</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>Case à cocher</td>
  <td></td>
 </tr>
</table>
