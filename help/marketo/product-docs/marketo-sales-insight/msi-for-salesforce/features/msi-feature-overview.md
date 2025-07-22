---
unique-page-id: 37356893
description: Présentation des fonctionnalités MSI - Documentation de Marketo - Documentation du produit
title: Présentation des fonctionnalités MSI
exl-id: e6cd988c-afba-44e3-b240-68258236f344
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 12%

---

# Présentation des fonctionnalités MSI {#msi-feature-overview}

MSI offre les fonctionnalités suivantes dans [!DNL Salesforce] Lightning et Classic.

>[!NOTE]
>
>Pour afficher toutes les données disponibles, assurez-vous que le zoom de votre navigateur est défini sur une valeur maximale de 125 % sous Windows et de 150 % sous Mac OS.

## Panneau Visualforce {#visualforce-panel}

Le panneau Visualforce de MSI comprend les fonctionnalités suivantes :

* Onglets

   * [Tableau de bord des informations](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * Moments significatifs
   * Activité Web
   * E-mail
   * Score

* Actions

   * Ajouter à la campagne Marketo
   * Envoyer l&#39;e-mail Marketo
   * Ajouter/Supprimer de la liste de surveillance

* Étoiles et flammes

## Mise en page du lead {#lead-layout}

Pages Visualforce :

* Lead - Inclut l&#39;option de cliquer sur hyper « Aller à la liste complète », vous serez envoyé à un nouvel onglet dans Salesforce où le panneau MSI sera visible dans une mise en page complète
* Liste complète des leads - N’inclut pas l’option « Accéder à la liste complète »
* Lead mobile - Visible dans l’application mobile Salesforce
* Bridge du contact du lead - Affiche le panneau MSI du contact que vous avez ajouté dans le champ ID du contact MSI.

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
* Afficher dans Marketo - Cliquez sur ce champ pour afficher une vue non modifiable du prospect dans Marketo. Inclut : informations sur le lead, informations sur la société, informations sur le lead SFDC, champs personnalisés SFDC, journal d’activité.
* ID de contact MSI - Ajoutez un contact Salesforce à ce champ et incluez le panneau « Bridge du contact du lead » dans la mise en page du lead pour afficher le panneau MSI du contact

## Mise en page du contact {#contact-layout}

Pages Visualforce :

* Contact - Inclut l&#39;option de cliquer sur hyper « Aller à la liste complète », vous serez envoyé à un nouvel onglet dans Salesforce où le panneau MSI sera visible dans une mise en page complète
* Contacter la liste complète - N’inclut pas l’option « Accéder à la liste complète »
* Contact Mobile : visible dans l’application mobile Salesforce
* Ajouter à la page de contact de Marketo Campaign - La fonctionnalité Ajouter à Marketo Campaign est disponible dans ce panneau

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
* Afficher dans Marketo - Cliquez sur ce champ pour afficher une vue non modifiable du prospect dans Marketo. Inclut : informations sur le lead, informations sur la société, informations sur le lead SFDC, champs personnalisés SFDC, journal d’activité.
* Score de lead maximal
* [!DNL Sales Insight] - Ouvre la page de liste complète des contacts

## Mise en page du compte {#account-layout}

Pages Visualforce :

* Compte - Inclut l&#39;option de cliquer sur hyper « Aller à la liste complète », vous serez envoyé à un nouvel onglet dans Salesforce où le panneau MSI sera visible dans une mise en page complète
* Liste complète des comptes - N’inclut pas l’option « Accéder à la liste complète »
* Compte mobile : visible dans l’application mobile Salesforce.

Champs :

* [!DNL Sales Insight] - Ouvre la page de liste complète des contacts

Actions :

* Ajouter à la campagne Marketo
* Envoyer l&#39;e-mail Marketo
* Ajouter/Supprimer de la liste de surveillance

Les fonctionnalités suivantes ne sont **pas disponibles** dans la page Disposition du compte :

* Étoiles et flammes

## Mise en page de l’opportunité {#opportunity-layout}

Pages Visualforce :

* Opportunité - Inclut l’option de cliquer sur hyper « Accéder à la liste complète » ; vous êtes envoyé à un nouvel onglet de Salesforce où le panneau MSI est visible dans une mise en page complète.
* Liste complète des opportunités - N’inclut pas l’option « Accéder à la liste complète »
* Opportunité mobile : visible dans l’application mobile Salesforce

Champs :

* [!DNL Sales Insight] - Ouvre la page de liste complète des contacts
* Analyse des opportunités Marketo - Ouvre l’analyseur d’influence des opportunités dans Marketo

Actions :

* Ajouter à la campagne Marketo
* Envoyer l&#39;e-mail Marketo
* Ajouter/Supprimer de la liste de surveillance

Les fonctionnalités suivantes ne sont **pas disponibles** dans la page Mise en page de l’opportunité :

* Étoiles et flammes

## Vue Liste des leads et des contacts (actions en bloc) {#lead-and-contact-list-view-bulk-actions}

[!DNL Salesforce Lightning] : boutons d’action Ajouter à la watchlist, Ajouter à Marketo Campaign et Envoyer un e-mail Marketo en bloc dans la vue Liste de prospects et de contacts.

[!DNL Salesforce Classic] : boutons d’action Ajouter à la liste de contrôle, Ajouter à Marketo Campaign et Envoyer un e-mail Marketo en bloc dans la vue Liste de prospects et de contacts.

## Onglet Marketo {#marketo-tab}

* [!DNL Best Bets]

   * Permet de créer et de modifier des vues. Possibilité de masquer les meilleurs résultats selon la configuration de l’option « Masquer par défaut » dans la page de configuration de Marketo
   * Colonnes : nom, compte, dernier moment intéressant, en-tête de statut, engagement (étoiles et flammes), masquer

* Ma liste de surveillance

   * Possibilité de créer et de modifier des vues
   * Colonnes : nom, compte, dernier moment intéressant, en-tête de statut, engagement (étoiles et flammes), supprimer

* Activité Web

   * Inclut la possibilité de créer et de modifier des vues, la fonctionnalité de filtre de période
   * Colonne - Page vue, Nom, Compte, Dernière visite

* Activité Web anonyme

   * Inclut la possibilité de créer et de modifier des vues, la fonctionnalité de filtre de période
   * Colonnes - Page vue, Société, Dernière visite, Recherche (ouvre la page LinkedIn de la société)

* Mes e-mails

   * Possibilité de créer et de modifier des vues
   * Colonnes - Nom, Compte, Objet, Date, Ouverture, Clic

* Flux de lead - Inclut la possibilité de s’abonner à des moments intéressants. Le flux RSS sur la page de configuration doit être activé pour utiliser cette fonctionnalité.

   * Lead/Contact ayant vécu ce moment intéressant
   * Type de moment intéressant (web, e-mail ou jalon) et description
   * Nom de compte
   * Heure à laquelle ce moment intéressant s’est produit
   * Option d’abonnement permettant de recevoir une notification par e-mail pour ce type d’événement
   * Icône Haute priorité pour afficher cette personne est un meilleur résultat

## Onglet Configuration [!DNL Marketo Sales Insight] {#marketo-sales-insight-configuration-tab}

* Paramètres opérationnels : inclut les informations d’identification d’API Soap et Rest nécessaires pour configurer MSI dans SFDC
* Configuration MSI : comprend la configuration de l’onglet Marketo et du panneau MSI visualforce
* Réinitialiser le [!DNL Marketo Sales Insight] : inclut la possibilité d’effacer toutes les configurations

>[!MORELIKETHIS]
>
>[[!DNL Marketo Sales Insight] Onglet Configuration dans [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## Rapports de performance [!DNL Sales Insight] {#sales-insight-performance-reports}

Affichez les performances des e-mails envoyés par le biais de [!DNL Salesforce], [!DNL Microsoft Dynamics] ou d’un plug-in Gmail ou [!DNL Outlook]

## MSI pour Mobile {#msi-for-mobile}

Les fonctionnalités MSI sont prises en charge dans [!DNL Salesforce] application mobile

## Prise en charge linguistique {#language-support}

[!DNL Marketo Sales Insight] est stocké par langue. Ainsi, si vous souhaitez qu’il fonctionne pour plusieurs langues, vous devez saisir les informations d’identification séparément pour chaque langue.

>[!NOTE]
>
>* Un contact/prospect doit se trouver dans la partition Par défaut pour être ajouté à la watchlist.
>
>* Le package MSI [!DNL Salesforce] ne prend pas en charge les vues personnalisées avec des champs dépendants.
