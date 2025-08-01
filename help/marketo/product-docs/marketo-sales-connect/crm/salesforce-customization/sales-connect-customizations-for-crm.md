---
unique-page-id: 14745793
description: Personnalisations [!DNL Sales Connect] pour CRM - Documents Marketo - Documentation du produit
title: Personnalisations [!DNL Sales Connect] pour CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 2%

---

# Personnalisations [!DNL Sales Connect] pour CRM {#sales-connect-customizations-for-crm}

Les champs et boutons ci-dessous sont créés par l’API Metadata dans Salesforce CRM. Une fois les champs créés, les administrateurs doivent configurer les mises en page dans leur CRM pour les exposer. Instructions [vous pouvez trouver ici](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf).

## Installation des personnalisations dans [!DNL Salesforce] {#how-to-install-customizations-in-salesforce}

1. Dans [!DNL Sales Connect], cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/one.png)

1. Sous [!UICONTROL &#x200B; Paramètres d’administration &#x200B;], sélectionnez **[!UICONTROL Salesforce]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Personnalisations de Marketo Sales Engage]**.

   ![](assets/three.png)

1. Cliquez sur **[!UICONTROL Connexion à Salesforce]**.

   ![](assets/four.png)

1. Connectez-vous à [!DNL Salesforce].

   ![](assets/five.png)

## Mise à jour [!DNL Salesforce] personnalisation {#update-salesforce-customization}

Les mises à jour du package Personnalisation du [!DNL Salesforce] incluront des améliorations et des correctifs. Pour vérifier si des mises à jour sont disponibles ou pour en effectuer une, procédez comme suit.

>[!NOTE]
>
>**Autorisations d’administrateur requises.**

1. Dans l’[application web](https://www.toutapp.com), cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. Sous [!UICONTROL Paramètres d’administration], cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. La carte Personnalisation de l’[!DNL Sales Connect] s’affiche si des mises à jour sont disponibles. Cliquez sur **[!UICONTROL Mettre à jour les personnalisations]**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Cliquez sur **[!UICONTROL Mettre à niveau]**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Attendez que les mises à jour s’installent. Selon le nombre de numéros de version dont vous avez besoin, la durée de l’installation varie.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Une fois l’opération terminée, votre carte affichera « Vos personnalisations Sales Connect sont à jour ».

![](assets/sales-connect-customizations-for-crm-11.png)

## Champs d’activité personnalisés {#custom-activity-fields}

Marketo détectera la création des nouveaux champs, puis effectuera un renvoi unique des données, un remappage et une synchronisation continue des valeurs dans les **nouveaux** champs uniquement. Les anciens champs ne seront pas mis à jour.

<table><thead>
  <tr>
    <th>Nom du champ</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>ID de présence locale de l'appel MSE</td>
    <td>En tant qu'utilisateur, vous pouvez choisir l'option Présence locale lorsque vous passez des appels à partir du téléphone MSE. Les appels entrants affichent un numéro local pour le destinataire.</td>
  </tr>
  <tr>
    <td>URL d’enregistrement d’appel MSE</td>
    <td>Les appels peuvent être enregistrés et un lien vers l’enregistrement sera consigné ici.</td>
  </tr>
  <tr>
    <td>Campagne MSE</td>
    <td>Consigne le nom de la campagne MSE dont le contact/lead est membre.</td>
  </tr>
  <tr>
    <td>URL de MSE Campaign</td>
    <td>Consigne l’URL de la campagne créée dans MSE. Cliquez sur ce bouton pour ouvrir la campagne dans l’application web MSE.</td>
  </tr>
  <tr>
    <td>Étape actuelle de MSE Campaign</td>
    <td>Si un contact/prospect fait partie d’une campagne, ce champ consigne le nom de l’étape à laquelle le contact/prospect se trouve actuellement.</td>
  </tr>
  <tr>
    <td>Pièce jointe d’e-mail MSE vue</td>
    <td>Consigne les données lorsqu’un e-mail est envoyé avec une pièce jointe et que la pièce jointe est vue par le destinataire.</td>
  </tr>
  <tr>
    <td>E-mail MSE sur lequel l’utilisateur a cliqué</td>
    <td>Enregistre une coche lorsque le destinataire clique sur un lien dans un e-mail.</td>
  </tr>
  <tr>
    <td>Réponse à un e-mail de MSE</td>
    <td>Enregistre une coche lorsque le destinataire répond à un e-mail.</td>
  </tr>
  <tr>
    <td>Statut des e-mails MSE</td>
    <td>Indique si un email est envoyé/en cours/rebond (le suivi des emails rebonds dépend du canal de diffusion utilisé).</td>
  </tr>
  <tr>
    <td>Modèle d’e-mail MSE</td>
    <td>Consigne le nom du modèle MSE utilisé dans l’e-mail envoyé au prospect/contact.</td>
  </tr>
  <tr>
    <td>URL du modèle d'e-mail MSE</td>
    <td>Consigne l’URL vers le modèle qui a été créé dans MSE. Cliquez sur ce bouton pour ouvrir le modèle dans l’application web MSE.</td>
  </tr>
  <tr>
    <td>URL de l'e-mail MSE</td>
    <td>Cliquez sur cette URL pour ouvrir le centre de commandes dans MSE et afficher l’onglet Historique d’affichage des détails des personnes dans lequel vous pouvez voir l’e-mail envoyé.</td>
  </tr>
  <tr>
    <td>E-mail MSE vu</td>
    <td>Enregistre une coche lorsque le destinataire consulte un e-mail.</td>
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
    <td>Dernier engagement entrant de Marketing.</td>
  </tr>
  <tr>
    <td>MSE - Date du dernier engagement marketing</td>
    <td>Date et heure de l’engagement à partir du marketing.</td>
  </tr>
  <tr>
    <td>MSE - Description du dernier engagement marketing</td>
    <td>Description de l’engagement.</td>
  </tr>
  <tr>
    <td>MSE - Dernier engagement marketing Source</td>
    <td>Source de l’engagement marketing.</td>
  </tr>
  <tr>
    <td>MSE - Dernier type d’engagement marketing</td>
    <td>Type d’engagement.</td>
  </tr>
  <tr>
    <td>MSE - Dernière activité par ventes</td>
    <td>Dernière activité sortante effectuée par l'équipe commerciale.</td>
  </tr>
  <tr>
    <td>MSE - Dernière réponse</td>
    <td>Dernier e-mail de réponse à l’e-mail de vente.</td>
  </tr>
  <tr>
    <td>MSE - Campagne de vente actuelle</td>
    <td>Consigne le nom de la campagne MSE dont le prospect/contact est membre.</td>
  </tr>
  <tr>
    <td>MSE - Dernier engagement commercial</td>
    <td>Dernier engagement entrant des ventes.</td>
  </tr>
  <tr>
    <td>MSE - Opt-out</td>
    <td>Champ d’opt-out.</td>
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
    <td>Envoyer un e-mail au MSE</td>
    <td>Envoyez des e-mails commerciaux depuis Salesforce.</td>
  </tr>
  <tr>
    <td>Ajouter à MSE Campaign</td>
    <td>Ajoutez aux campagnes MSE à partir de Salesforce.</td>
  </tr>
  <tr>
    <td>Intégrer à MSE</td>
    <td>Intégrez le contact de Salesforce à MSE.</td>
  </tr>
  <tr>
    <td>Appel avec MSE</td>
    <td>Effectuez des appels commerciaux depuis Salesforce.</td>
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
    <td>Ajouter à MSE Campaign</td>
    <td>Ajoutez aux campagnes MSE à partir de Salesforce.</td>
  </tr>
  <tr>
    <td>Intégrer à MSE</td>
    <td>Intégrez le contact de Salesforce à MSE.</td>
  </tr>
</tbody>
</table>

## Guides de l’utilisateur {#user-guides}

[Rapports personnalisés MSE dans Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[MSE pour Salesforce Classic](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[MSE pour Salesforce Lightning](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
