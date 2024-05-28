---
unique-page-id: 37356893
description: Présentation des fonctionnalités MSI - Documents Marketo - Documentation du produit
title: Présentation des fonctionnalités MSI
exl-id: e6cd988c-afba-44e3-b240-68258236f344
feature: Marketo Sales Insights
source-git-commit: bda95da160c5a27a0a460d26c102e6166c1ddea0
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 11%

---

# Présentation des fonctionnalités MSI {#msi-feature-overview}

MSI propose les fonctionnalités suivantes dans Salesforce Lightning et Classic.

>[!NOTE]
>
>Pour afficher toutes les données disponibles, veillez à ce que le zoom de votre navigateur ne dépasse pas 125 % sous Windows et 150 % sous Mac OS.

## Panneau Visualforce {#visualforce-panel}

Le panneau MSI Visualforce comprend les fonctionnalités suivantes :

* Onglets

   * [Tableau de bord des statistiques](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * Moments significatifs
   * Activité Web
   * E-mail
   * Évaluation

* Actions

   * Ajouter à la campagne Marketo
   * Envoyer l&#39;e-mail Marketo
   * Ajouter/Supprimer de la liste de contrôle

* Etoiles et flammes

## Disposition de piste {#lead-layout}

Pages Visualforce :

* Piste : comprend l’option permettant de cliquer sur l’hyperactivité &quot;Atteindre la liste complète&quot;. Vous serez alors dirigé vers un nouvel onglet de Salesforce dans lequel le panneau MSI sera visible en page entière.
* Liste complète des pistes - N’inclut pas l’option &quot;Aller à la liste complète&quot;
* Lead Mobile - Visible dans l’application mobile Salesforce
* Pont Contact de piste : affiche le panneau MSI du contact que vous avez ajouté dans le champ ID de contact MSI.

Champs :

* Dernier moment significatif
* Date dernier moment significatif
* Description dernier moment significatif
* Source dernier moment significatif
* Type dernier moment significatif
* Dernière activité Marketo par les équipes de ventes
* Dernier engagement Marketo par les équipes de ventes
* Évaluation relative
* Valeur d&#39;évaluation relative
* Urgence
* Valeur d&#39;urgence
* Afficher dans Marketo : cliquez sur ce champ pour ouvrir une vue non modifiable de la piste dans Marketo. Inclut : Infos sur les pistes, Informations sur la société, Infos sur les pistes de la SFDC, Champs personnalisés de la SFDC, Journal d’activité
* Identifiant de contact MSI : ajoutez un contact Salesforce à ce champ et incluez le panneau &quot;Pont contact de piste&quot; dans la mise en page de piste pour afficher le panneau MSI du contact.

## Contact Layout {#contact-layout}

Pages Visualforce :

* Contact - Inclut l’option permettant de cliquer sur l’hyper &quot;Aller à la liste complète&quot;. Vous serez alors envoyé vers un nouvel onglet de Salesforce, où le panneau MSI sera visible en page entière.
* Contact Liste complète - N’inclut pas l’option &quot;Aller à la liste complète&quot;
* Contact Mobile - Visible dans l’application mobile Salesforce
* La fonction Ajouter à la page de contact Marketo Campaign - Ajouter à Marketo Campaign est disponible dans ce panneau.

Champs :

* Dernier moment significatif
* Date dernier moment significatif
* Description dernier moment significatif
* Source dernier moment significatif
* Type dernier moment significatif
* Dernière activité Marketo par les équipes de ventes
* Évaluation relative
* Valeur d&#39;évaluation relative
* Urgence
* Valeur d&#39;urgence
* Afficher dans Marketo : cliquez sur ce champ pour ouvrir une vue non modifiable de la piste dans Marketo. Inclut : Infos sur les pistes, Informations sur la société, Infos sur les pistes de la SFDC, Champs personnalisés de la SFDC, Journal d’activité
* Mkto Lead Score
* Sales Insight - Ouvre la page de liste complète des contacts

## Disposition du compte {#account-layout}

Pages Visualforce :

* Compte - Inclut l’option permettant de cliquer sur l’hyperactivité &quot;Atteindre la liste complète&quot;. Vous serez alors dirigé vers un nouvel onglet de Salesforce dans lequel le panneau MSI sera visible en page entière.
* Liste complète du compte - N’inclut pas l’option &quot;Aller à la liste complète&quot;
* Compte mobile - Visible dans l’application mobile Salesforce

Champs :

* Sales Insight - Ouvre la page de liste complète des contacts

Actions :

* Ajouter à la campagne Marketo
* Envoyer l&#39;e-mail Marketo
* Ajouter/Supprimer de la liste de contrôle

Les fonctionnalités suivantes sont disponibles : **non disponible** sur la page Disposition du compte :

* Etoiles et flammes

## Disposition des opportunités {#opportunity-layout}

Pages Visualforce :

* Opportunité - Inclut l’option permettant de cliquer sur l’hyperactivité &quot;Atteindre la liste complète&quot;. Vous serez alors dirigé vers un nouvel onglet de Salesforce dans lequel le panneau MSI sera visible dans une mise en page complète.
* Liste complète des opportunités - N’inclut pas l’option &quot;Aller à la liste complète&quot;
* Opportunity Mobile - Visible dans l’application mobile Salesforce

Champs :

* Sales Insight - Ouvre la page de liste complète des contacts
* Analyse des opportunités Marketo - Ouvre l’analyseur d’influence des opportunités dans Marketo

Actions :

* Ajouter à la campagne Marketo
* Envoyer l&#39;e-mail Marketo
* Ajouter/Supprimer de la liste de contrôle

Les fonctionnalités suivantes sont disponibles : **non disponible** sur la page Disposition d’opportunité :

* Etoiles et flammes

## Mode Liste de pistes et de contacts (actions en bloc) {#lead-and-contact-list-view-bulk-actions}

Éclair Salesforce : ajoutez les boutons d’action groupée Ajouter à la liste de contrôle, Ajouter à Marketo Campaign et Envoyer un courrier électronique Marketo en mode Liste de pistes et de contacts.

Salesforce Classic : boutons d’action en bloc Ajouter à la liste de contrôle, Ajouter à Marketo Campaign et Envoyer un courrier électronique Marketo en mode Liste de pistes et de contacts.

## Onglet Marketo {#marketo-tab}

* Meilleurs paris

   * Inclut la possibilité de créer et de modifier des vues. Possibilité de masquer les meilleures options selon la configuration de l’option &quot;Masquage par défaut&quot; sur la page de configuration de Marketo
   * Colonnes : nom, compte, dernier moment intéressant, en-tête d’état, engagement (étoiles et flammes), masquer

* Ma liste de surveillance

   * Possibilité de créer et de modifier des vues
   * Colonnes : nom, compte, dernier moment intéressant, en-tête d’état, engagement (étoiles et flammes), suppression

* Activité Web

   * Inclut la possibilité de créer et de modifier des vues, ainsi que la fonctionnalité de filtre de période.
   * Colonne : Page vue, Nom, Compte, Dernière visite

* Activité Web anonyme

   * Inclut la possibilité de créer et de modifier des vues, ainsi que la fonctionnalité de filtre de période.
   * Colonnes - Page vue, Société, Dernière visite, Recherche (ouvre la page LinkedIn de l’entreprise)

* Mes e-mails

   * Possibilité de créer et de modifier des vues
   * Colonnes - Nom, Compte, Objet, Date, Ouvrir, Clic

* Flux de piste : inclut la possibilité de s’abonner à des moments intéressants. Le flux RSS sur la page Configuration doit être activé pour utiliser cette fonctionnalité.

   * Responsable/contact ayant vécu ce moment intéressant
   * Type de moment intéressant (web, email ou jalon) et description
   * Nom de compte
   * Heure à laquelle ce moment intéressant s&#39;est produit
   * Option d’abonnement pour recevoir une notification par email pour ce type d’événement
   * Icône Haute priorité pour afficher la meilleure mise pour cette personne

## Onglet Configuration des statistiques sur les ventes Marketo {#marketo-sales-insight-configuration-tab}

* Paramètres opérationnels : comprend les informations d’identification de l’API Soap &amp; Rest requises pour configurer MSI dans SFDC
* Configuration de MSI : inclut la configuration de l’onglet Marketo et du panneau MSI VisitorForce.
* Réinitialiser Marketo Sales Insight : permet d’effacer toutes les configurations.

>[!MORELIKETHIS]
>
>[Onglet Configuration de l’aperçu des ventes Marketo dans Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## Rapports sur les performances de Sales Insight {#sales-insight-performance-reports}

Afficher les performances des emails envoyés par le biais de Salesforce, Microsoft Dynamics ou d’un module externe Gmail ou Outlook

## MSI pour Mobile {#msi-for-mobile}

Les fonctionnalités MSI sont prises en charge dans l’application mobile Salesforce.

## Prise en charge linguistique {#language-support}

Marketo Sales Insight est stocké par langue. Ainsi, si vous souhaitez qu’il fonctionne pour plusieurs langues, vous devez saisir les informations d’identification séparément pour chaque langue.

>[!NOTE]
>
>* Un contact/prospect doit se trouver dans la partition par défaut pour être ajouté à la liste de contrôle.
>
>* Le package MSI Salesforce ne prend pas en charge la vue personnalisée avec les champs dépendants.
