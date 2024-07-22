---
description: Désinstallation du module de personnalisation de l’éclair Salesforce - Documents Marketo - Documentation du produit
title: Désinstallation du module de personnalisation de l’éclair Salesforce
exl-id: 4af89222-22b1-4c08-8081-3dab89d1985b
feature: Sales Insight Actions
source-git-commit: 688120d2529339274c1650c7478480156810b0b4
workflow-type: tm+mt
source-wordcount: '1184'
ht-degree: 9%

---

# Désinstallation du module de personnalisation de l’éclair Salesforce {#uninstall-salesforce-lightning-customization-package}

Désinstallez le package Marketo Sales Connect de votre compte Salesforce une fois que vous avez commencé à utiliser le package MSI Actions.

## Suppression des champs de connexion aux ventes de la mise en page {#remove-sales-connect-fields-from-page-layout}

1. Dans Salesforce Lightning, cliquez sur l&#39;icône représentant un engrenage et sélectionnez **Setup**.

   ![](assets/uninstall-salesforce-lightning-customization-package-1.png)

1. Cliquez sur **Object Manager**.

   ![](assets/uninstall-salesforce-lightning-customization-package-2.png)

1. Faites défiler l’écran jusqu’à et sélectionnez **Lead**.

   ![](assets/uninstall-salesforce-lightning-customization-package-3.png)

1. Cliquez sur **Dispositions de page**.

   ![](assets/uninstall-salesforce-lightning-customization-package-4.png)

1. Cliquez sur **Mise en page de piste**.

   ![](assets/uninstall-salesforce-lightning-customization-package-5.png)

   >[!NOTE]
   >
   >La vue Modifier la mise en page n’a pas encore été mise à jour dans Salesforce Lightning.

1. Dans la console, sélectionnez **Champs**. Dans Recherche rapide, recherchez &quot;MSC&quot;. Tous les champs grisés ont été ajoutés à la mise en page. Vous devrez les supprimer.

   ![](assets/uninstall-salesforce-lightning-customization-package-6.png)

   >[!NOTE]
   >
   >Si aucun des champs n’est grisé, cela signifie que vous ne les avez pas ajoutés à la mise en page. Vous pouvez ignorer cette section.

1. Accédez à la section contenant vos champs personnalisés de Connect Sales.

   ![](assets/uninstall-salesforce-lightning-customization-package-7.png)

1. Il existe 10 types de champs du MSC qui peuvent être ajoutés à cette section. Supprimez tous les champs que vous avez ajoutés ou supprimez simplement la section entière.

1. Cliquez sur **Enregistrement rapide** lorsque vous avez terminé.

   ![](assets/uninstall-salesforce-lightning-customization-package-8.png)

## Suppression des boutons de connexion aux ventes des mises en page {#remove-sales-connect-buttons-from-page-layouts}

1. Dans la console (Étape 4 ci-dessus), sélectionnez **Boutons**. Recherchez &quot;MSC&quot;. Tous les boutons grisés ont été ajoutés à votre section de bouton personnalisée. Vous devrez les supprimer.

   ![](assets/uninstall-salesforce-lightning-customization-package-9.png)

   >[!NOTE]
   >
   >Si aucun des boutons n’est grisé, cela signifie que vous ne les avez pas ajoutés. Vous pouvez ignorer cette section.

1. Faites glisser les boutons MSC de la section Boutons personnalisés vers la console.

   ![](assets/uninstall-salesforce-lightning-customization-package-10.png)

1. Cliquez sur **Enregistrement rapide** lorsque vous avez terminé.

   ![](assets/uninstall-salesforce-lightning-customization-package-11.png)

## Suppression des champs de connexion aux ventes de la section Historique des activités {#remove-sales-connect-fields-from-activity-history-section}

1. Faites défiler la page jusqu’au bas de la page jusqu’à la section Liste associée à l’historique des activités , puis cliquez sur l’icône en forme de clé à molette.

   ![](assets/uninstall-salesforce-lightning-customization-package-12.png)

1. Sélectionnez les champs de connexion des ventes dans la zone Champs sélectionnés et cliquez sur la flèche Supprimer . Cliquez sur **OK** lorsque vous avez terminé.

   ![](assets/uninstall-salesforce-lightning-customization-package-13.png)

   >[!NOTE]
   >
   >L’abréviation MSE _est_ Sales Connect. C&#39;est juste le nom précédent, &quot;Marketo Sales Engage&quot;.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé avec la page Pistes.

## Suppression des boutons d’action en bloc Connect Sales du mode Liste des pistes {#remove-sales-connect-bulk-action-buttons-from-lead-list-view}

1. Dans Salesforce Lightning, cliquez sur l&#39;icône représentant un engrenage et sélectionnez **Setup**.

   ![](assets/uninstall-salesforce-lightning-customization-package-14.png)

1. Cliquez sur **Object Manager**.

   ![](assets/uninstall-salesforce-lightning-customization-package-15.png)

1. Faites défiler l’écran jusqu’à et sélectionnez **Lead**.

   ![](assets/uninstall-salesforce-lightning-customization-package-16.png)

1. Cliquez sur **Rechercher des mises en page**.

   ![](assets/uninstall-salesforce-lightning-customization-package-17.png)

1. Cliquez sur la flèche en regard de Mode Liste et sélectionnez **Modifier**.

   ![](assets/uninstall-salesforce-lightning-customization-package-18.png)

1. Sélectionnez **Ajouter à la campagne MSC**, **Email with MSC** et **Envoyer au MSC**, puis cliquez sur la flèche Supprimer . Cliquez ensuite sur **Enregistrer**.

   ![](assets/uninstall-salesforce-lightning-customization-package-19.png)

Vous ne devriez plus voir les boutons en mode Liste de pistes.

## Suppression de la configuration du MSC pour les contacts {#remove-msc-configuration-for-contacts}

1. Dans Salesforce Lightning, cliquez sur l&#39;icône représentant un engrenage et sélectionnez **Setup**.

1. Cliquez sur **Object Manager**.

1. Faites défiler l’écran jusqu’à et sélectionnez **Contact**.

1. Cliquez sur **Dispositions de page**.

1. Cliquez sur **Contact Layout**.

1. Répétez les étapes des trois sections.

## Suppression de la configuration du SMC pour les opportunités {#remove-msc-configuration-for-opportunity}

1. Dans Salesforce Lightning, cliquez sur l&#39;icône représentant un engrenage et sélectionnez **Setup**.

1. Cliquez sur **Object Manager**.

1. Faites défiler l’écran jusqu’à et sélectionnez **Opportunity**.

1. Cliquez sur **Dispositions de page**.

1. Cliquez sur **Disposition d’opportunité**.

La vue d’opportunité ne comporte qu’un seul bouton : &quot;Envoyer un email MSE&quot; et les champs suivants :

![](assets/uninstall-salesforce-lightning-customization-package-20.png)

## Suppression de la configuration MSC pour un compte {#remove-msc-configuration-for-account}

1. Dans Salesforce Lightning, cliquez sur l&#39;icône représentant un engrenage et sélectionnez **Setup**.

1. Cliquez sur **Object Manager**.

1. Faites défiler l’écran jusqu’à et sélectionnez **Compte**.

1. Cliquez sur **Dispositions de page**.

1. Cliquez sur **Disposition du compte**.

La vue Compte ne comporte qu’un seul bouton : &quot;Envoyer un email MSE&quot; et les champs suivants :

![](assets/uninstall-salesforce-lightning-customization-package-21.png)

## Supprimer la boîte d’envoi des ventes Marketo {#remove-marketo-sales-outbox}

1. Dans Salesforce, cliquez sur l’onglet **+** en haut de votre écran.

1. Cliquez Sur **Personnaliser Mes Onglets**.

1. Sélectionnez l’option Marketo Sales Outbox (Boîte d’envoi des ventes) à droite. Cliquez sur la flèche Supprimer, puis sur **Enregistrer**.

## Supprimer le module Sales Connect {#delete-sales-connect-package}

Une fois que vous avez supprimé tous les objets de votre compte Salesforce, procédez comme suit.

1. Dans Salesforce Lightning, cliquez sur l&#39;icône représentant un engrenage et sélectionnez **Setup**.

1. Dans la zone Recherche rapide, saisissez &quot;Classes Apex&quot;.

1. Cliquez sur **Supprimer** en regard de toutes les entrées &quot;MarketoSalesConnectionCustomization&quot; ou &quot;MarketoSalesEngageCustomization&quot; de votre liste.

Vous êtes tous prêts !

Voici la liste de tous les objets qui doivent être supprimés de votre instance Salesforce :

## Détails de la personnalisation de Sales Connect {#sales-connect-customization-details}

<table>
 <tr>
  <th>Champs d’activité personnalisés</th>
  <th>Description</th>
  <th>Type</th>
  <th>Type de données</th>
 </tr>
 <tr>
  <td>Identifiant de présence local de l’appel du MSC</td>
  <td>En tant qu’utilisateur, je peux choisir la Présence locale comme option lorsque je lance des appels depuis le MSC Phone. Les appels entrants affichent un numéro local pour le récepteur.</td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>URL d’enregistrement de l’appel du MSC</td>
  <td>Les appels peuvent être enregistrés et un lien pour l’enregistrement est consigné ici </td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>MSC Campaign</td>
  <td>Nom des journaux de la campagne du MSC sur laquelle se trouve le contact/la piste</td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>URL de la campagne MSC</td>
  <td>Consigne l’URL de la campagne qui a été créée dans MSC. Cliquer dessus ouvrira la campagne dans l’application web du MSC.</td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>Étape actuelle de la campagne MSC</td>
  <td>Si un contact/un prospect figure dans une campagne, ce champ consigne le nom de l’étape dans laquelle il se trouve actuellement.</td>
  <td>Activité</td>
  <td>Case à cocher</td>
 </tr>
 <tr>
  <td>Pièce jointe de courrier électronique du MSC affichée</td>
  <td>Consigne les données lorsqu’un email est envoyé avec une pièce jointe consultée par le destinataire</td>
  <td>Activité</td>
  <td>Case à cocher</td>
 </tr>
 <tr>
  <td>Courrier électronique du MSC cliqué</td>
  <td>Consigne une coche lorsque le destinataire clique sur un lien dans l’email</td>
  <td>Activité</td>
  <td>Case à cocher</td>
 </tr>
 <tr>
  <td>Message électronique du MSC répondu</td>
  <td>Consigne une coche lorsque le destinataire répond à l’email</td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>État des courriers électroniques du MSC</td>
  <td>Indique si un email est envoyé/en cours/rebond (le suivi des emails rebonds dépend du canal de diffusion utilisé).</td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>Modèle de courrier électronique MSC</td>
  <td>Nom des journaux du modèle MSC utilisé dans l’email envoyé au prospect/contact</td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>URL du modèle de courrier électronique du MSC</td>
  <td>Consigne l’URL du modèle qui a été créé dans MSC. Cliquer dessus ouvrira le modèle dans l’application web du MSC.</td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>URL de courriel du MSC</td>
  <td>Cliquez sur cette URL pour ouvrir le centre de commande dans MSC et extraire l’onglet Historique des détails des personnes où l’utilisateur peut voir l’email envoyé.</td>
  <td>Activité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>Courrier électronique du MSC consulté</td>
  <td>Consigne une coche lorsque le destinataire affiche un email</td>
  <td>Activité</td>
  <td>Case à cocher</td>
 </tr>
</table>

<table>
 <tr>
  <th>Champ de journalisation de cumul du MSC</th>
  <th>Description</th>
  <th>Type</th>
  <th>Type de données</th>
 </tr>
 <tr>
  <td>MSC - Dernier engagement marketing</td>
  <td>Dernier engagement entrant provenant de Marketing</td>
  <td>
  <p>Compte
  <p>Contact
  <p>Prospect
  <p>Opportunité</td>
  <td>Données et heure</td>
 </tr>
 <tr>
  <td>MSC - Date de dernier engagement marketing</td>
  <td>Horodatage de l’engagement à partir de Marketing</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
  <td>Données et heure</td>
 </tr>
 <tr>
  <td>MSC - Dernier engagement marketing Desc</td>
  <td>Description de l’engagement</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>MSC - Dernier Source d’engagement marketing</td>
  <td>Source de l’engagement marketing</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>MSC - Dernier type d’engagement marketing</td>
  <td>Type d’engagement (ex : activité web)</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>MSC - Dernière activité par les ventes</td>
  <td>Dernière activité sortante réalisée par l'équipe commerciale</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
  <td>Données et heure</td>
 </tr>
 <tr>
  <td>MSC - Dernière réponse</td>
  <td>Dernière réponse par e-mail à l’e-mail de vente</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
  <td>Données et heure</td>
 </tr>
 <tr>
  <td>MSC - Campagne de ventes en cours</td>
  <td>Nom des journaux de la campagne du MSC sur laquelle se trouve le contact/la piste</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
  <td>Texte</td>
 </tr>
 <tr>
  <td>MSC - Dernier engagement commercial</td>
  <td>Dernier engagement entrant provenant des ventes</td>
  <td>
  <p>Compte
  <p>Contact
  <p>Prospect
  <p>Opportunité</td>
  <td>Données et heure</td>
 </tr>
 <tr>
  <td>MSC - Exclusion</td>
  <td>Champ d’exclusion</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
  <td>Case à cocher</td>
 </tr>
</table>

<table>
 <tr>
  <th>Boutons du MSC</th>
  <th>Description</th>
  <th>Type</th>
 </tr>
 <tr>
  <td>Envoi d’un courrier électronique MSC</td>
  <td>Envoi d’emails de vente par Salesforce</td>
  <td>
  <p>Compte 
  <p>Contact 
  <p>Prospect 
  <p>Opportunité</td>
 </tr>
 <tr>
  <td>Ajouter à la campagne MSC</td>
  <td>Ajouter aux campagnes du MSC depuis Salesforce</td>
  <td>
  <p>Contact
  <p>Lead</td>
 </tr>
 <tr>
  <td>Poussez au MSC</td>
  <td>Envoyer le contact de Salesforce au MSC</td>
  <td>
  <p>Contact
  <p>Lead</td>
 </tr>
 <tr>
  <td>Appel avec le MSC</td>
  <td>Lancer des appels de vente depuis Salesforce</td>
  <td>
  <p>Contact
  <p>Lead</td>
 </tr>
</table>

<table>
 <tr>
  <th>Boutons d’action en bloc du MSC</th>
  <th>Description</th>
  <th>Type</th>
 </tr>
 <tr>
  <td>Ajouter à la campagne MSC</td>
  <td>Ajouter aux campagnes du MSC depuis Salesforce</td>
  <td>
  <p>Contact
  <p>Lead</td>
 </tr>
 <tr>
  <td>Poussez au MSC</td>
  <td>Envoyer le contact de Salesforce au MSC</td>
  <td>
  <p>Contact
  <p>Lead</td>
 </tr>
 <tr>
  <td>Email avec le MSC</td>
  <td>Courriel du MSC de Salesforce</td>
  <td>
  <p>Contact
  <p>Lead</td>
 </tr>
</table>
