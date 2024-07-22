---
unique-page-id: 42762514
description: Présentation des fonctionnalités du tableau de bord des insights - Documents Marketo - Documentation du produit
title: Présentation des fonctionnalités du tableau de bord des insights
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1525'
ht-degree: 0%

---

# Présentation des fonctionnalités du tableau de bord des insights {#insights-dashboard-feature-overview}

En savoir plus sur les fonctionnalités disponibles dans votre tableau de bord Statistiques sur les ventes .

>[!PREREQUISITES]
>
>Vous devez disposer du dernier package MSI SFDC et de la [configuration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

![](assets/insights-dashboard-feature-overview-1.png)

## Contact Layout {#contact-layout}

**Grille de vitesse d’engagement**

* Cette grille dynamique comprend les moments intéressants, les e-mails et l’activité web au cours des 90 derniers jours.
* L’utilisateur peut choisir d’utiliser l’activité &quot;Afficher le compte&quot;, qui va regrouper tous les moments intéressants au niveau du compte, le courrier électronique et l’activité web dans la vue Contact.
* L’utilisateur peut mettre en surbrillance une semaine spécifique pour afficher les activités au cours de cette semaine.
* Mode par défaut : semaine en cours sélectionnée

**Analyse en profondeur de l’engagement et résumé**

* Exploration des cartes d’activité pour les moments intéressants, les e-mails et les activités web
* Carte d’activité Moments intéressants - Inclut l’option S’abonner
* Carte Activité du courrier électronique - Inclut l’option Aperçu
* Carte d’activité web - Inclut la possibilité de cliquer sur le lien
* La barre de résumé hebdomadaire affiche les moments intéressants, les e-mails et l’activité web pour cette semaine. Chaque icône peut faire l’objet d’un clic et peut être utilisée comme filtre pour afficher une activité spécifique.
* Vue par défaut : il s’agit d’une liste des activités de la vue actuelle.

**Campagnes et événements de messagerie à venir**

Onglet Campagnes par e-mail :

* Inclut des campagnes qui font partie de programmes de messagerie ou de programmes par défaut programmés au cours des 90 prochains jours
* Non spécifique au contact/prospect (c’est-à-dire que la liste des campagnes est une liste générique de toutes les campagnes par e-mail planifiées dans l’instance Marketo). La liste des campagnes de tous les panneaux prospect, contact, compte et opportunité sera la même.
* Si la récurrence de la campagne est telle qu’elle s’exécute plus de trois fois au cours des 90 prochains jours, seules les trois prochaines exécutions s’afficheront à un moment donné (comme dans le cas du comportement dans Marketo).
* La carte des détails de l’activité de cette section comporte une option d’aperçu. Si le flux comprend plusieurs étapes d’envoi d’email, tous les emails peuvent être prévisualisés. Au cours de l’étape Envoyer le flux d’email, s’il existe plusieurs &quot;choix d’email&quot;, l’option par défaut est disponible pour la prévisualisation.
* Les filtres incluent &quot;Recherche&quot; et &quot;Période&quot;

![](assets/insights-dashboard-feature-overview-2.png)

Onglet Événement :

* Inclut les programmes d’événement planifiés dans les 90 prochains jours
* Utilisez l’option de filtrage pour afficher tous les événements/événements invités (en fonction des paramètres d’administration).
* La sélection d’événements invités affiche les événements auxquels un contact spécifique a été invité, ainsi que le statut du membre.
* La sélection de tous les événements affiche la liste des événements programmés au cours des 90 prochains jours.
* La carte Détails de l’activité de cette section comporte une option d’aperçu.
* Le filtre inclut &quot;Rechercher&quot;, &quot;Afficher uniquement les événements invités&quot; et &quot;Période&quot;.

![](assets/insights-dashboard-feature-overview-3.png)

## Disposition de piste {#lead-layout}

**Grille de vitesse d’engagement**

* Cette grille dynamique comprend les moments intéressants, les e-mails et l’activité web au cours des 90 derniers jours.
* L’utilisateur peut mettre en surbrillance une semaine spécifique pour afficher les activités au cours de cette semaine.
* Mode par défaut : semaine en cours sélectionnée
* La fonction &quot;Afficher l’activité du compte&quot; n’est pas disponible sur les pistes, puisqu’elle ne fait partie d’aucun compte dans Salesforce tant qu’elle n’a pas été convertie en contact.

**Analyse en profondeur de l’engagement et résumé**

* Cartes d’activité de zoom déroulant pour les moments intéressants, les e-mails et l’activité web
* Carte d’activité Moments intéressants - Inclut l’option S’abonner
* Carte Activité du courrier électronique - Inclut l’option Aperçu
* Carte d’activité web - Inclut la possibilité de cliquer sur le lien
* La barre de résumé hebdomadaire affiche les moments intéressants, les e-mails et l’activité web pour cette semaine. Chaque icône peut faire l’objet d’un clic et peut être utilisée comme filtre pour afficher une activité spécifique.
* Vue par défaut : il s’agit d’une liste des activités de la vue actuelle.

**Campagnes et événements de messagerie à venir :**

Onglet Campagnes par e-mail :

* Inclut des campagnes qui font partie de programmes de messagerie ou de programmes par défaut programmés au cours des 90 prochains jours
* Non spécifique au contact/prospect (c’est-à-dire que la liste des campagnes est une liste générique de toutes les campagnes par e-mail planifiées dans l’instance Marketo). La liste des campagnes de tous les panneaux prospect, contact, compte et opportunité sera la même.
* Si la récurrence de la campagne est telle qu’elle s’exécute plus de trois fois au cours des 90 prochains jours, seules les trois prochaines exécutions s’afficheront à un moment donné (comme dans le cas du comportement dans Marketo).
* La carte des détails de l’activité de cette section comporte une option d’aperçu. Si le flux comprend plusieurs étapes d’envoi d’email, tous les emails peuvent être prévisualisés. Au cours de l’étape Envoyer le flux d’email, s’il existe plusieurs &quot;choix d’email&quot;, l’option par défaut est disponible pour la prévisualisation.
* Les filtres incluent &quot;Recherche&quot; et &quot;Période&quot;

![](assets/insights-dashboard-feature-overview-4.png)

Onglet Événement :

* Inclut les programmes d’événement planifiés dans les 90 prochains jours
* Utilisez l’option de filtrage pour afficher tous les événements/événements invités (en fonction des paramètres d’administration).
* La sélection d’événements invités affiche les événements auxquels un contact spécifique a été invité, ainsi que le statut du membre.
* La sélection de tous les événements affiche la liste des événements programmés au cours des 90 prochains jours.
* La carte Détails de l’activité de cette section comporte une option d’aperçu.
* Le filtre inclut &quot;Rechercher&quot;, &quot;Afficher uniquement les événements invités&quot; et &quot;Période&quot;.

![](assets/insights-dashboard-feature-overview-5.png)

## Disposition du compte {#account-layout}

**Grille de vitesse d’engagement**

* Cette grille dynamique comprend les moments intéressants, les e-mails et l’activité web au cours des 90 derniers jours pour tous les contacts du compte.
* L’utilisateur peut mettre en surbrillance une semaine spécifique pour afficher les activités au cours de cette semaine.
* Mode par défaut : semaine en cours sélectionnée

**Zoom avant sur l’engagement et résumé**

* Analyse des cartes d’activité pour les moments intéressants, les e-mails et l’activité web, y compris le nom du contact
* Carte d’activité Moments intéressants - Inclut l’option S’abonner
* Carte Activité du courrier électronique - Inclut l’option Aperçu
* Carte d’activité web - Inclut la possibilité de cliquer sur le lien
* La barre de résumé hebdomadaire affiche les moments intéressants, les e-mails et l’activité web pour cette semaine. Chaque icône peut faire l’objet d’un clic et peut être utilisée comme filtre pour afficher une activité spécifique.
* Vue par défaut : il s’agit d’une liste des activités de la vue actuelle.

**Campagnes et événements de messagerie à venir**

Onglet Campagnes par e-mail :

* Inclut des campagnes qui font partie de programmes de messagerie ou de programmes par défaut programmés au cours des 90 prochains jours
* Non spécifique au contact/prospect (c’est-à-dire que la liste des campagnes est une liste générique de toutes les campagnes par e-mail planifiées dans l’instance Marketo). La liste des campagnes de tous les panneaux prospect, contact, compte et opportunité sera la même.
* Si la récurrence de la campagne est telle qu’elle s’exécute plus de trois fois au cours des 90 prochains jours, seules les trois prochaines exécutions s’afficheront à un moment donné (comme dans le cas du comportement dans Marketo).
* La carte des détails de l’activité de cette section comporte une option d’aperçu. Si le flux comprend plusieurs étapes d’envoi d’email, tous les emails peuvent être prévisualisés. Au cours de l’étape Envoyer le flux d’email, s’il existe plusieurs &quot;choix d’email&quot;, l’option par défaut est disponible pour la prévisualisation.
* Les filtres incluent &quot;Recherche&quot; et &quot;Période&quot;

Onglet Événement :

* Inclut les programmes d’événement planifiés dans les 90 prochains jours
* Utilisez l’option de filtrage pour afficher tous les événements/événements invités (en fonction des paramètres d’administration).
* La sélection d’événements invités affiche les événements auxquels un contact spécifique a été invité, ainsi que le statut du membre.
* La sélection de tous les événements affiche la liste des événements programmés au cours des 90 prochains jours.
* La carte Détails de l’activité de cette section comporte une option d’aperçu.
* Le filtre inclut &quot;Rechercher&quot;, &quot;Afficher uniquement les événements invités&quot; et &quot;Période&quot;.

## Disposition des opportunités {#opportunity-layout}

**Grille de vitesse d’engagement**

* Cette grille dynamique comprend les moments intéressants, les e-mails et l’activité web au cours des 90 derniers jours pour tous les contacts de l’opportunité.
* L’utilisateur peut mettre en surbrillance une semaine spécifique pour afficher les activités au cours de cette semaine.
* Mode par défaut : semaine en cours sélectionnée

**Zoom avant sur l’engagement et résumé**

* Analyse des cartes d’activité pour les moments intéressants, les e-mails et l’activité web, y compris le nom du contact
* Carte d’activité Moments intéressants - Inclut l’option S’abonner
* Carte Activité du courrier électronique - Inclut l’option Aperçu
* Carte d’activité web - Inclut la possibilité de cliquer sur le lien
* La barre de résumé hebdomadaire affiche les moments intéressants, les e-mails et l’activité web pour cette semaine. Chaque icône peut faire l’objet d’un clic et peut être utilisée comme filtre pour afficher une activité spécifique.
* Vue par défaut : il s’agit d’une liste des activités de la vue actuelle.

**Campagnes et événements de messagerie à venir** Onglet Campagnes par e-mail :

* Inclut des campagnes qui font partie de programmes de messagerie ou de programmes par défaut programmés au cours des 90 prochains jours
* Non spécifique au contact/prospect (c’est-à-dire que la liste des campagnes est une liste générique de toutes les campagnes par e-mail planifiées dans l’instance Marketo). La liste des campagnes de tous les panneaux prospect, contact, compte et opportunité sera la même.
* Si la récurrence de la campagne est telle qu’elle s’exécute plus de trois fois au cours des 90 prochains jours, seules les trois prochaines exécutions s’afficheront à un moment donné (comme dans le cas du comportement dans Marketo).
* La carte des détails de l’activité de cette section comporte une option d’aperçu. Si le flux comprend plusieurs étapes d’envoi d’email, tous les emails peuvent être prévisualisés. Au cours de l’étape Envoyer le flux d’email, s’il existe plusieurs &quot;choix d’email&quot;, l’option par défaut est disponible pour la prévisualisation.
* Les filtres incluent &quot;Recherche&quot; et &quot;Période&quot;

Onglet Événement :

* Inclut les programmes d’événement planifiés dans les 90 prochains jours
* Utilisez l’option de filtrage pour afficher tous les événements/événements invités (en fonction des paramètres d’administration).
* La sélection d’événements invités affiche les événements auxquels un contact spécifique a été invité, ainsi que le statut du membre.
* La sélection de tous les événements affiche la liste des événements programmés au cours des 90 prochains jours.
* La carte Détails de l’activité de cette section comporte une option d’aperçu.
* Le filtre inclut &quot;Rechercher&quot;, &quot;Afficher uniquement les événements invités&quot; et &quot;Période&quot;.

>[!NOTE]
>
>Si votre compte ou opportunité compte plus de 800 contacts, le tableau de bord n’affiche aucune donnée. Vous pouvez toutefois consulter des contacts individuels pour consulter leurs informations et leur engagement. Si votre compte compte compte plus de 800 contacts, l’option &quot;Afficher l’activité au niveau du compte&quot; sera désactivée.
