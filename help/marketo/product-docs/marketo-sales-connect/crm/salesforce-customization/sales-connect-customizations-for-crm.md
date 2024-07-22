---
unique-page-id: 14745793
description: Personnalisations de Sales Connect pour le CRM - Documents Marketo - Documentation du produit
title: Personnalisations de la connexion aux ventes pour le CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Personnalisations de la connexion aux ventes pour le CRM {#sales-connect-customizations-for-crm}

Les champs et boutons ci-dessous sont créés par l’API de métadonnées dans Salesforce CRM. Une fois les champs créés, les administrateurs doivent configurer les mises en page dans leur CRM pour les exposer. Les instructions se trouvent [ici](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Cela a un impact sur les clients ToutApp et Sales Connect.

## Comment installer des personnalisations dans Salesforce {#how-to-install-customizations-in-salesforce}

1. Dans Sales Connect, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/one.png)

1. Sous Paramètres d’administration, sélectionnez **Salesforce**.

   ![](assets/two.png)

1. Cliquez sur **Personnalisations Marketo Sales Connect**.

   ![](assets/three.png)

1. Cliquez sur **Se connecter à Salesforce**.

   ![](assets/four.png)

1. Connectez-vous à Salesforce.

   ![](assets/five.png)

## Mise à jour de la personnalisation Salesforce {#update-salesforce-customization}

Les mises à jour du package de personnalisation Salesforce comprennent des améliorations et des correctifs. Pour vérifier si des mises à jour sont disponibles ou pour effectuer une mise à jour, procédez comme suit.

>[!NOTE]
>
>**Autorisations d’administrateur requises.**

1. Dans l’ [application web](https://www.toutapp.com), cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. Sous Paramètres d’administration, cliquez sur **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. La carte de personnalisation de Sales Connect s’affiche si des mises à jour sont disponibles. Cliquez sur **Mettre à jour les personnalisations**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Cliquez sur **Upgrade**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Attendez l’installation des mises à jour. Selon le nombre de numéros de version dont vous avez besoin, l’heure d’installation varie.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Une fois que vous avez terminé, votre carte affiche &quot;Vos personnalisations de votre connexion commerciale sont à jour&quot;.

![](assets/sales-connect-customizations-for-crm-11.png)

## Champs d’activité personnalisés {#custom-activity-fields}

Marketo détectera la création des nouveaux champs, puis effectuera un renvoi unique des données, un re-mappage et une synchronisation continue des valeurs dans les champs **new** uniquement. Les anciens champs ne seront pas mis à jour.

| **Nom du champ** | **Description** |
|---|---|
| Identifiant de présence locale de l’appel MSE | En tant qu’utilisateur, vous pouvez choisir l’option Présence locale lorsque vous effectuez des appels à partir du téléphone MSE. Les appels entrants affichent un numéro local pour le récepteur. |
| URL d’enregistrement des appels MSE | Les appels peuvent être enregistrés et un lien pour l’enregistrement sera consigné ici. |
| Campagne MSE | Nom des journaux de la campagne MSE dont le contact/prospect est membre. |
| URL de campagne MSE | Consigne l’URL de la campagne qui a été créée dans MSE. Cliquer dessus ouvre la campagne dans l’application web MSE. |
| Étape actuelle de la campagne MSE | Si un contact/prospect fait partie d’une campagne, ce champ consigne le nom de l’étape sur laquelle le prospect/contact est actuellement actif. |
| Pièce jointe du courrier électronique MSE affichée | Consigne les données lorsqu’un email est envoyé avec une pièce jointe et que la pièce jointe est visualisée par le destinataire. |
| MSE Email Cliqué | Consigne une coche lorsque le destinataire clique sur un lien dans un email. |
| Message électronique MSE répondu | Consigne une coche lorsque le destinataire répond à un email. |
| Statut de l&#39;email MSE | Indique si un email est envoyé/en cours/rebond (le suivi des emails rebonds dépend du canal de diffusion utilisé). |
| Modèle de courrier électronique MSE | Nom du journal du modèle MSE utilisé dans l’e-mail envoyé au prospect/contact. |
| URL du modèle de courrier électronique MSE | Consigne l’URL du modèle qui a été créé dans MSE. Cliquer dessus ouvre le modèle dans l’application web MSE. |
| URL de l’email MSE | Cliquez sur cette URL pour ouvrir le Centre de commandes dans MSE et extraire l’onglet Historique de l’affichage des détails des personnes où vous pouvez voir l’email envoyé. |
| MSE Email Viewed | Consigne une coche lorsque le destinataire affiche un email. |

## Champs de journalisation de cumul {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Nom de champ</strong></td> 
   <td><strong>Description</strong></td> 
  </tr> 
  <tr> 
   <td>MSE - Dernier engagement marketing</td> 
   <td>Dernier engagement entrant issu de Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Date de dernier engagement marketing</td> 
   <td>Horodatage de l’engagement de Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Dernier engagement marketing Desc</td> 
   <td>Description de l’engagement.</td> 
  </tr> 
  <tr> 
   <td>MSE - Dernier Source d’engagement marketing</td> 
   <td>Source de l’engagement marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Dernier type d’engagement marketing</td> 
   <td colspan="1">Type d’engagement.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Dernière activité par les ventes<br></td> 
   <td colspan="1">Dernière activité sortante réalisée par l'équipe de vente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Dernière réponse</td> 
   <td colspan="1">Dernière réponse par e-mail à l’e-mail de vente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campagne de ventes en cours</td> 
   <td colspan="1">Nom des journaux de la campagne MSE dont le prospect/contact est membre.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Dernier engagement commercial</td> 
   <td colspan="1">Dernier engagement entrant des ventes. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Exclusion</td> 
   <td colspan="1">Champ d’exclusion.</td> 
  </tr> 
 </tbody> 
</table>

## Boutons {#buttons}

| **Nom du bouton** | **Description** |
|---|---|
| Envoyer un courrier électronique MSE | Envoyez des e-mails de vente depuis Salesforce. |
| Ajouter à la campagne MSE | Ajoutez à des campagnes MSE à partir de Salesforce. |
| Push to MSE | Envoyez le contact de Salesforce à MSE. |
| Appel avec MSE | Effectuez des appels de vente depuis Salesforce. |

## Boutons d’action en bloc {#bulk-action-buttons}

| **Nom du bouton** | **Description** |
|---|---|
| Ajouter à la campagne MSE | Ajoutez à des campagnes MSE à partir de Salesforce. |
| Push to MSE | Envoyez le contact de Salesforce à MSE. |

## Guides de l’utilisateur {#user-guides}

[Rapports personnalisés MSE dans Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE pour Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE pour Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
