---
unique-page-id: 37356893
description: Présentation des fonctionnalités MSI - Documentation sur le marketing - Documentation sur les produits
title: Présentation des fonctionnalités MSI
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---


# Présentation des fonctionnalités MSI {#msi-feature-overview}

MSI propose les fonctionnalités suivantes dans Salesforce Lightning et Classic.

## Panneau Visualforce {#visualforce-panel}

Le panneau MSI Visualforce comprend les fonctionnalités suivantes :

* Onglets

   * [Tableau de bord d’informations](http://docs.marketo.com/x/EoGMAg)
   * Moment intéressant
   * Activité Web
   * Courriel
   * Score

* Actions

   * Ajouter à Marketo Campaign
   * Envoyer un courriel marketing
   * Ajouter/Supprimer de la Liste de surveillance

* Stars &amp; Flames

## Disposition de piste {#lead-layout}

Pages Visualforce :

* Piste - Inclut l&#39;option de cliquer sur l&#39;hyperlien &quot;Aller à la Liste complète&quot;. Vous serez envoyé vers un nouvel onglet de Salesforce où le panneau MSI sera visible dans une mise en page complète.
* Liste complète de piste - N&#39;inclut pas l&#39;option &quot;Atteindre la Liste complète&quot;
* Lead Mobile - Visible dans l&#39;application mobile Salesforce
* Pont de contact de piste : affiche le panneau MSI du contact que vous avez ajouté dans le champ ID de contact MSI.

Champs :

* Dernier moment intéressant
* Date du dernier moment intéressant
* Dernier moment intéressant Desc
* Dernière source intéressante
* Dernier type de moment intéressant
* Dernière Activité du marché par vente
* Dernier engagement marketing par vente
* Note relative
* Valeur de score relative
* Urgence
* Valeur d’urgence
* Vue dans Marketo - Cliquez sur ce champ pour ouvrir une vue de piste non modifiable dans Marketo. Comprend : Infos de piste, Infos de Société, Infos de piste SFDC, Champs personnalisés SFDC, Journal des Activités
* ID de contact MSI : Ajoutez un contact Salesforce à ce champ et ajoutez le panneau &quot;Pont de contact de piste&quot; dans la mise en page de piste pour afficher le panneau MSI du contact.

## Disposition du contact {#contact-layout}

Pages Visualforce :

* Contact - Inclut l&#39;option permettant de cliquer sur l&#39;hyperlien &quot;Aller à la Liste complète&quot;. Vous serez envoyé vers un nouvel onglet de Salesforce où le panneau MSI sera visible dans une mise en page complète.
* Contact Liste complète - N&#39;inclut pas l&#39;option &quot;Atteindre la Liste complète&quot;
* Contact Mobile - Visible dans l&#39;application mobile Salesforce
* Ajouter à la page de contact de Marketo Campaign - La fonction Ajouter à Marketo Campaign est disponible dans ce panneau

Champs :

* Dernier moment intéressant
* Date du dernier moment intéressant
* Dernier moment intéressant Desc
* Dernière source intéressante
* Dernier type de moment intéressant
* Dernière Activité du marché par vente
* Note relative
* Valeur de score relative
* Urgence
* Valeur d’urgence
* Vue dans Marketo - Cliquez sur ce champ pour ouvrir une vue de piste non modifiable dans Marketo. Comprend : Infos de piste, Infos de Société, Infos de piste SFDC, Champs personnalisés SFDC, Journal des Activités
* Note de piste Mkto
* Sales Insight - Ouvre la page de liste complète des contacts

## Disposition du compte {#account-layout}

Pages Visualforce :

* Compte - Inclut l&#39;option permettant de cliquer sur l&#39;hyperlien &quot;Aller à la Liste complète&quot;, vous serez envoyé vers un nouvel onglet de Salesforce où le panneau MSI sera visible dans une mise en page complète.
* Liste complète du compte - N’inclut pas l’option &quot;Atteindre la Liste complète&quot;.
* Compte mobile - Visible dans l&#39;application mobile Salesforce

Champs :

* Sales Insight - Ouvre la page de liste complète des contacts

Les fonctionnalités suivantes **ne sont pas disponibles** dans la page Disposition du compte :

* Actions : Ajouter à Marketo Campaign, Envoyer un courriel à Marketo, Ajouter/Supprimer de la Liste de contrôle
* Stars &amp; Flames

## Mise en page des opportunités {#opportunity-layout}

Pages Visualforce :

* Opportunité - Inclut l&#39;option permettant de cliquer sur l&#39;hyperlien &quot;Aller à la Liste complète&quot;. Vous serez envoyé vers un nouvel onglet de Salesforce où le panneau MSI sera visible dans une mise en page complète.
* Liste complète de l&#39;opportunité - N&#39;inclut pas l&#39;option &quot;Atteindre la Liste complète&quot;
* Opportunité mobile - Visible dans l&#39;application mobile Salesforce

Champs :

* Sales Insight - Ouvre la page de liste complète des contacts
* Analyse des opportunités marketing - Ouvre l&#39;analyseur d&#39;influence des opportunités dans Marketo

Les fonctionnalités suivantes **ne sont pas disponibles** dans la page Mise en page des opportunités :

* Actions : Ajouter à Marketo Campaign, Envoyer un courriel à Marketo, Ajouter/Supprimer de la Liste de contrôle
* Stars &amp; Flames

## Vue de Liste de piste et de contact (actions en masse) {#lead-and-contact-list-view-bulk-actions}

Salesforce Lightning : Ajoutez à Watchlist, Ajoutez à Marketo Campaign et Envoyer Marketo par courriel les boutons d’action en bloc dans Lead et Contact liste vue.

Salesforce Classic : Ajoutez à Watchlist, Ajoutez à Marketo Campaign et envoyez le marketing par courriel pour les boutons d’action en masse dans Lead et Contact liste vue.

## Onglet Marqueur {#marketo-tab}

* Meilleurs paris

   * Inclut la possibilité de créer et de modifier des vues. Possibilité de masquer les meilleurs paris en fonction de la configuration de l’option &quot;Masquer par défaut&quot; sur la page de configuration du marketing.
   * Colonnes - Nom, Compte, Dernier moment intéressant, En-tête d’état, Engagement (étoiles et flammes), Masquer

* Ma Liste de surveillance

   * Possibilité de créer et de modifier des vues
   * Colonnes - Nom, Compte, Dernier moment intéressant, En-tête d’état, Engagement (étoiles et flammes), Supprimer

* Activité Web

   * Inclut la possibilité de créer et de modifier des vues, la fonctionnalité de filtrage des périodes
   * Colonne - vue de page, nom, compte, dernière visite

* Activité Web anonyme

   * Inclut la possibilité de créer et de modifier des vues, la fonctionnalité de filtrage des périodes
   * Colonnes - Vue de page, Société, Dernière visite, Recherche (ouvre la page LinkedIn de la société)

* Mon courriel

   * Possibilité de créer et de modifier des vues
   * Colonnes - Nom, Compte, Objet, Date, Ouvrir, Cliquer

* Flux de piste - Inclut la possibilité de s&#39;abonner à des moments intéressants, le flux RSS sur la page Configuration doit être activé pour utiliser cette fonctionnalité.

   * Responsable/contact ayant vécu ce moment intéressant
   * Type de moment intéressant (Web, courriel ou jalon) et description
   * Nom du compte
   * Heure de ce moment intéressant
   * Option d’abonnement pour recevoir une notification par courrier électronique pour ce type de événement
   * Icône de priorité élevée pour montrer que cette personne est mieux placée

## Onglet de configuration de Marketing Cloud Sales Insight {#marketo-sales-insight-configuration-tab}

* Paramètres opérationnels : Inclut les informations d’identification de l’API Soap &amp; Rest nécessaires pour configurer MSI dans SFDC
* Configuration MSI : Inclut la configuration de l’onglet Marketo et du panneau MSI Visualforce
* Réinitialiser les statistiques commerciales de marketing : Inclut la possibilité d&#39;effacer toutes les configurations

>[!MORELIKETHIS]
>
>[Onglet Configuration des statistiques de ventes du marketing dans Salesforce](http://docs.marketo.com/x/UoCMAg)

## Rapports sur les performances de Sales Insight {#sales-insight-performance-reports}

Vue des performances des courriers électroniques envoyés par l&#39;intermédiaire de Salesforce, Microsoft Dynamics ou d&#39;un module externe Gmail ou Outlook

## MSI pour Mobile {#msi-for-mobile}

Les fonctionnalités MSI sont prises en charge dans l&#39;application mobile Salesforce

## Prise en charge des langues {#language-support}

Les statistiques des ventes de marketing sont stockées par langue. Donc, si vous voulez qu&#39;il fonctionne pour plusieurs langues, vous devez entrer les informations d&#39;identification séparément pour chaque langue.
