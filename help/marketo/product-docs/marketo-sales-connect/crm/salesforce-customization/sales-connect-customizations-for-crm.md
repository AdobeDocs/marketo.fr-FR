---
unique-page-id: 14745793
description: Personnalisations de Sales Connect pour le CRM - Documents Marketo - Documentation du produit
title: Personnalisations de la connexion aux ventes pour le CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: dbf058714f6c4e6003c5a64d1048ac8a47931a0f
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 2%

---

# Personnalisations de la connexion aux ventes pour le CRM {#sales-connect-customizations-for-crm}

Les champs et boutons ci-dessous sont créés par l’API de métadonnées dans le CRM Salesforce. Une fois les champs créés, les administrateurs doivent configurer les mises en page dans leur CRM pour les exposer. Les instructions [se trouvent ici](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf).

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

## Mise à jour de la personnalisation de Salesforce {#update-salesforce-customization}

Le module de personnalisation de Salesforce comprend des améliorations et des correctifs. Pour vérifier si des mises à jour sont disponibles ou pour effectuer une mise à jour, procédez comme suit.

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

<table><thead>
  <tr>
    <th>Nom du champ</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Identifiant de présence locale de l’appel MSE</td>
    <td>En tant qu’utilisateur, vous pouvez choisir l’option Présence locale lorsque vous effectuez des appels à partir du téléphone MSE. Les appels entrants affichent un numéro local pour le récepteur.</td>
  </tr>
  <tr>
    <td>URL d’enregistrement des appels MSE</td>
    <td>Les appels peuvent être enregistrés et un lien pour l’enregistrement sera consigné ici.</td>
  </tr>
  <tr>
    <td>Campagne MSE</td>
    <td>Nom des journaux de la campagne MSE dont le contact/prospect est membre.</td>
  </tr>
  <tr>
    <td>URL de campagne MSE</td>
    <td>Consigne l’URL de la campagne qui a été créée dans MSE. Cliquer dessus ouvre la campagne dans l’application web MSE.</td>
  </tr>
  <tr>
    <td>Étape actuelle de la campagne MSE</td>
    <td>Si un contact/prospect fait partie d’une campagne, ce champ consigne le nom de l’étape sur laquelle le prospect/contact est actuellement actif.</td>
  </tr>
  <tr>
    <td>Pièce jointe du courrier électronique MSE affichée</td>
    <td>Consigne les données lorsqu’un email est envoyé avec une pièce jointe et que la pièce jointe est visualisée par le destinataire.</td>
  </tr>
  <tr>
    <td>MSE Email Cliqué</td>
    <td>Consigne une coche lorsque le destinataire clique sur un lien dans un email.</td>
  </tr>
  <tr>
    <td>Message électronique MSE répondu</td>
    <td>Consigne une coche lorsque le destinataire répond à un email.</td>
  </tr>
  <tr>
    <td>Statut de l'email MSE</td>
    <td>Indique si un email est envoyé/en cours/rebond (le suivi des emails rebonds dépend du canal de diffusion utilisé).</td>
  </tr>
  <tr>
    <td>Modèle de courrier électronique MSE</td>
    <td>Nom du journal du modèle MSE utilisé dans l’e-mail envoyé au prospect/contact.</td>
  </tr>
  <tr>
    <td>URL du modèle de courrier électronique MSE</td>
    <td>Consigne l’URL du modèle qui a été créé dans MSE. Cliquer dessus ouvre le modèle dans l’application web MSE.</td>
  </tr>
  <tr>
    <td>URL de l’email MSE</td>
    <td>Cliquez sur cette URL pour ouvrir le Centre de commandes dans MSE et extraire l’onglet Historique de l’affichage des détails des personnes où vous pouvez voir l’email envoyé.</td>
  </tr>
  <tr>
    <td>MSE Email Viewed</td>
    <td>Consigne une coche lorsque le destinataire affiche un email.</td>
  </tr>
</tbody></table>

## Champs de journalisation de cumul {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>Nom du champ</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE - Dernier engagement marketing</td>
    <td>Dernier engagement entrant issu de Marketing.</td>
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
    <td>MSE - Dernier type d’engagement marketing</td>
    <td>Type d’engagement.</td>
  </tr>
  <tr>
    <td>MSE - Dernière activité par les ventes</td>
    <td>Dernière activité sortante réalisée par l'équipe de vente.</td>
  </tr>
  <tr>
    <td>MSE - Dernière réponse</td>
    <td>Dernière réponse par e-mail à l’e-mail de vente.</td>
  </tr>
  <tr>
    <td>MSE - Campagne de ventes en cours</td>
    <td>Nom des journaux de la campagne MSE dont le prospect/contact est membre.</td>
  </tr>
  <tr>
    <td>MSE - Dernier engagement commercial</td>
    <td>Dernier engagement entrant des ventes.</td>
  </tr>
  <tr>
    <td>MSE - Exclusion</td>
    <td>Champ d’exclusion.</td>
  </tr>
</tbody></table>

## Boutons {#buttons}

<table><thead>
  <tr>
    <th>Nom du bouton</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Envoyer un courrier électronique MSE</td>
    <td>Envoyez des e-mails de vente depuis Salesforce.</td>
  </tr>
  <tr>
    <td>Ajouter à la campagne MSE</td>
    <td>Ajoutez à des campagnes MSE à partir de Salesforce.</td>
  </tr>
  <tr>
    <td>Push to MSE</td>
    <td>Poussez le contact de Salesforce vers MSE.</td>
  </tr>
  <tr>
    <td>Appel avec MSE</td>
    <td>Lancer des appels de vente depuis Salesforce.</td>
  </tr>
</tbody>
</table>

## Boutons d’action en bloc {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>Nom du bouton</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ajouter à la campagne MSE</td>
    <td>Ajoutez à des campagnes MSE à partir de Salesforce.</td>
  </tr>
  <tr>
    <td>Push to MSE</td>
    <td>Poussez le contact de Salesforce vers MSE.</td>
  </tr>
</tbody>
</table>

## Guides de l’utilisateur {#user-guides}

[Rapports personnalisés MSE dans Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[MSE pour Salesforce Classic](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[MSE pour Salesforce Lightning](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
