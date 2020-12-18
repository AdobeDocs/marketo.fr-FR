---
unique-page-id: 14745793
description: Personnalisations de Sales Connect pour CRM - Documents marketing - Documentation sur les produits
title: Personnalisations de Sales Connect pour CRM
translation-type: tm+mt
source-git-commit: 07ae1b3f3ee3e9d7f35373eea039d336bd786f97
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---


# Personnalisations de Sales Connect pour CRM {#sales-connect-customizations-for-crm}

Les champs et les boutons ci-dessous sont créés par l’API de métadonnées dans Salesforce CRM. Une fois les champs créés, les administrateurs doivent configurer les mises en page dans leur gestion de la relation client pour les exposer. Vous trouverez les instructions [ici](http://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf).

>[!NOTE]
>
>Cela a un impact sur les clients de ToutApp et de Sales Connect.

## Comment installer des personnalisations dans Salesforce {#how-to-install-customizations-in-salesforce}

1. Dans Sales Connect, cliquez sur l&#39;icône représentant un engrenage et sélectionnez **Paramètres**.

   ![](assets/one.png)

1. Sous Paramètres d’administration, sélectionnez **Salesforce**.

   ![](assets/two.png)

1. Cliquez sur **Personnalisations de Marketing Connect**.

   ![](assets/three.png)

1. Cliquez sur **Se connecter à Salesforce**.

   ![](assets/four.png)

1. Connectez-vous à Salesforce.

   ![](assets/five.png)

## Champs d&#39;Activité personnalisés {#custom-activity-fields}

Marketo détecte la création des nouveaux champs, puis effectue un renvoi unique des données, un remappage et une synchronisation continue des valeurs dans les champs **new** uniquement. Les anciens champs ne seront pas mis à jour.

| **Nom du champ** | **Description** |
|---|---|
| ID de présence locale de l’appel MSE | En tant qu’utilisateur, vous pouvez choisir l’option Présence locale lorsque vous effectuez des appels à partir du téléphone MSE. Les appels entrants affichent un numéro local pour le destinataire. |
| URL d’enregistrement d’appel MSE | Les appels peuvent être enregistrés et un lien pour l&#39;enregistrement sera enregistré ici. |
| MSE Campaign | Consigne le nom de la campagne MSE dont le contact/prospect est membre. |
| URL Campaign MSE | Consigne l’URL de la campagne créée dans MSE. Cliquez sur cette option pour ouvrir la campagne dans l’application Web MSE. |
| Étape actuelle de MSE Campaign | Si un contact/prospect fait partie d&#39;une campagne, ce champ consigne le nom de l&#39;étape sur laquelle se trouve actuellement le prospect/contact. |
| Pièce jointe au courrier électronique MSE affichée | Consigne les données lorsqu’un courrier électronique est envoyé avec une pièce jointe et que la pièce jointe est consultée par le destinataire. |
| Courriel MSE cliqué | Enregistre une coche lorsque le destinataire clique sur un lien dans un courrier électronique. |
| Message électronique MSE répondu | Enregistre une coche lorsque le destinataire répond à un courrier électronique. |
| État du courrier électronique MSE | Indique si un courrier électronique est envoyé/en cours/rebondi (le suivi des messages rebondis dépend du canal de diffusion utilisé). |
| Modèle de courrier électronique MSE | Consigne le nom du modèle MSE utilisé dans le courrier électronique envoyé au prospect/contact. |
| URL du modèle de courrier électronique MSE | Consigne l’URL dans le modèle créé dans MSE. Cliquez sur cette option pour ouvrir le modèle dans l’application Web MSE. |
| URL de courriel MSE | Cliquez sur cette URL pour ouvrir le Centre de commandes dans MSE et afficher l&#39;onglet Historique des Vues des détails sur les personnes dans lequel vous pouvez voir le courrier électronique envoyé. |
| Courriel MSE consulté | Enregistre une coche lorsque le destinataire vue un courriel. |

## Champs de journalisation cumulée {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Nom du champ</strong></td> 
   <td><strong>Description</strong></td> 
  </tr> 
  <tr> 
   <td>MSE - Dernier engagement marketing</td> 
   <td>Dernier engagement entrant de Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Dernière date d’engagement marketing</td> 
   <td>Horodatage de l’engagement de Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Dernier engagement marketing Desc</td> 
   <td>Description de l’engagement.</td> 
  </tr> 
  <tr> 
   <td>MSE - Dernière source d’engagement marketing</td> 
   <td>Source de l’engagement Marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Dernier type d’engagement marketing</td> 
   <td colspan="1">Type d’engagement.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Dernière Activité par vente<br></td> 
   <td colspan="1">Dernière activité sortante réalisée par l'équipe des ventes.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Dernière réponse</td> 
   <td colspan="1">Dernière réponse par courrier électronique à l'adresse électronique de vente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campaign de vente en cours</td> 
   <td colspan="1">Consigne le nom de la campagne MSE dont le responsable/contact est membre.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Dernier engagement commercial</td> 
   <td colspan="1">Dernier engagement entrant des ventes. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Opt-out</td> 
   <td colspan="1">Champ d’exclusion.</td> 
  </tr> 
 </tbody> 
</table>

## Boutons {#buttons}

| **Nom du bouton** | **Description** |
|---|---|
| Envoyer un courrier électronique MSE | Envoyer des e-mails de vente de Salesforce. |
| Ajouter à MSE Campaign | Ajoutez aux campagnes MSE de Salesforce. |
| Pousser vers MSE | Poussez le contact de Salesforce vers MSE. |
| Appel avec MSE | Effectuez des appels de vente à partir de Salesforce. |

## Boutons d&#39;action en bloc {#bulk-action-buttons}

| **Nom du bouton** | **Description** |
|---|---|
| Ajouter à MSE Campaign | Ajoutez aux campagnes MSE de Salesforce. |
| Pousser vers MSE | Poussez le contact de Salesforce vers MSE. |

## Guides de l&#39;utilisateur {#user-guides}

[Rapports personnalisés MSE dans Salesforce](http://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE pour Salesforce](http://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE for Salesforce Lightning](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)

## Vidéos connexes {#related-videos}

**Comment installer des personnalisations dans Salesforce**
`<iframe width="630" height="470" src="//play.vidyard.com/YEPWYBfFEa4nKCo2F6bKKc.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>` ** Avantages de l&#39;utilisation de personnalisations dans Salesforce** 
`<iframe width="630" height="470" src="//play.vidyard.com/4PzSDb6o8Qg8WbvBsq8wJD.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`