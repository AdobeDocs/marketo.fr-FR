---
unique-page-id: 42762514
description: Présentation Des Fonctionnalités Du Tableau De Bord Insights - Documents Marketo - Documentation Du Produit
title: Vue d’ensemble des fonctionnalités du tableau de bord des informations
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 0%

---

# Vue d’ensemble des fonctionnalités du tableau de bord des informations {#insights-dashboard-feature-overview}

En savoir plus sur les fonctionnalités disponibles dans votre tableau de bord [!DNL Sales Insights].

>[!PREREQUISITES]
>
>Vous devez disposer du dernier package MSI SFDC et de la [configuration](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

![](assets/insights-dashboard-feature-overview-1.png)

## Mise en page du contact {#contact-layout}

**Grille de vitesse d’engagement**

* Cette grille dynamique comprend les moments significatifs, les e-mails et l’activité web au cours des 90 derniers jours
* L’utilisateur peut choisir l’activité « [!UICONTROL Afficher le compte] ». Elle s’étendra à tous les moments significatifs au niveau du compte, à l’e-mail et à l’activité web dans la vue de contact
* L’utilisateur peut mettre en surbrillance une semaine spécifique afin d’afficher les activités de cette semaine
* Affichage par défaut : la semaine en cours est sélectionnée

**Analyse et résumé de l’engagement**

* Accéder aux cartes d’activité pour les moments significatifs, l’e-mail et l’activité web
* Carte d’activité Moments significatifs - Inclut l’option S’abonner
* Carte d’activité E-mail - Inclut l’option Aperçu
* Carte d’activité web - Inclut la possibilité de cliquer sur le lien
* La barre de résumé hebdomadaire affiche les moments significatifs, l’e-mail et l’activité web de la semaine. Chaque icône est cliquable et peut être utilisée comme filtre pour afficher une activité spécifique
* Affichage par défaut : il s’agit d’une liste des activités de l’affichage actuel

**Campagnes et événements par e-mail à venir**

Onglet Campagnes par e-mail :

* Inclut les campagnes qui font partie de programmes de messagerie ou de programmes par défaut planifiés au cours des 90 prochains jours
* Non spécifique au contact/prospect (c’est-à-dire que la liste des campagnes est une liste générique de toutes les campagnes par e-mail planifiées dans l’instance Marketo). La liste des campagnes sur tous les panneaux de lead, contact, compte et opportunité sera la même
* Si la périodicité de la campagne est telle qu’elle s’exécute plus de trois fois au cours des 90 prochains jours, seules les trois exécutions suivantes s’affichent à un moment donné (comme dans Marketo)
* La vignette des détails de l’activité de cette section comporte une option de prévisualisation. Si le flux comprend plusieurs étapes d’envoi d’e-mail, tous les e-mails seront disponibles pour la prévisualisation. Dans l’étape Envoyer un e-mail , s’il existe plusieurs « choix d’e-mail », l’option par défaut est disponible pour la prévisualisation
* Les filtres incluent « [!UICONTROL Recherche] » et « [!UICONTROL Période] »

![](assets/insights-dashboard-feature-overview-2.png)

Onglet Événement :

* Inclut les programmes d’événement planifiés au cours des 90 prochains jours
* Utilisez l’option de filtre pour afficher tous les événements/événements invités (en fonction des paramètres d’administration)
* La sélection des événements invités affiche les événements auxquels un contact spécifique a été invité, ainsi que le statut de membre
* Lorsque vous sélectionnez tous les événements, la liste des événements planifiés pour les 90 prochains jours s’affiche
* La carte Détails de l’activité de cette section comporte une option de prévisualisation
* Le filtre comprend « [!UICONTROL Rechercher] », « [!UICONTROL Afficher uniquement les événements invités] » et « [!UICONTROL Période] »

![](assets/insights-dashboard-feature-overview-3.png)

## Mise en page du lead {#lead-layout}

**Grille de vitesse d’engagement**

* Cette grille dynamique comprend les moments significatifs, les e-mails et l’activité web au cours des 90 derniers jours
* L’utilisateur peut mettre en surbrillance une semaine spécifique afin d’afficher les activités de cette semaine
* Affichage par défaut : la semaine en cours est sélectionnée
* La fonctionnalité « [!UICONTROL &#x200B; Afficher l’activité du compte &#x200B;] » n’est pas disponible sur les prospects, car elle ne fait partie d’aucun compte dans [!DNL Salesforce] jusqu’à sa conversion en contact

**Analyse et résumé de l’engagement**

* Cartes d’activité d’analyse pour les moments significatifs, l’e-mail et l’activité web
* Carte d’activité Moments significatifs - Inclut l’option S’abonner
* Carte d’activité E-mail - Inclut l’option Aperçu
* Carte d’activité web - Inclut la possibilité de cliquer sur le lien
* La barre de résumé hebdomadaire affiche les moments significatifs, l’e-mail et l’activité web de la semaine. Chaque icône est cliquable et peut être utilisée comme filtre pour afficher une activité spécifique
* Affichage par défaut : il s’agit d’une liste des activités de l’affichage actuel

**Campagnes et événements par e-mail à venir :**

Onglet Campagnes par e-mail :

* Inclut les campagnes qui font partie de programmes de messagerie ou de programmes par défaut planifiés au cours des 90 prochains jours
* Non spécifique au contact/prospect (c’est-à-dire que la liste des campagnes est une liste générique de toutes les campagnes par e-mail planifiées dans l’instance Marketo). La liste des campagnes sur tous les panneaux de lead, contact, compte et opportunité sera la même
* Si la périodicité de la campagne est telle qu’elle s’exécute plus de trois fois au cours des 90 prochains jours, seules les trois exécutions suivantes s’affichent à un moment donné (comme dans Marketo)
* La vignette des détails de l’activité de cette section comporte une option de prévisualisation. Si le flux comprend plusieurs étapes d’envoi d’e-mail, tous les e-mails seront disponibles pour la prévisualisation. Dans l’étape Envoyer un e-mail , s’il existe plusieurs « choix d’e-mail », l’option par défaut est disponible pour la prévisualisation
* Les filtres incluent « [!UICONTROL Recherche] » et « [!UICONTROL Période] »

![](assets/insights-dashboard-feature-overview-4.png)

Onglet Événement :

* Inclut les programmes d’événement planifiés au cours des 90 prochains jours
* Utilisez l’option de filtre pour afficher tous les événements/événements invités (en fonction des paramètres d’administration)
* La sélection des événements invités affiche les événements auxquels un contact spécifique a été invité, ainsi que le statut de membre
* Lorsque vous sélectionnez tous les événements, la liste des événements planifiés pour les 90 prochains jours s’affiche
* La carte Détails de l’activité de cette section comporte une option de prévisualisation
* Le filtre comprend « [!UICONTROL Rechercher] », « [!UICONTROL Afficher uniquement les événements invités] » et « [!UICONTROL Période] »

![](assets/insights-dashboard-feature-overview-5.png)

## Mise en page du compte {#account-layout}

**Grille de vitesse d’engagement**

* Cette grille dynamique comprend les moments significatifs, l’activité e-mail et web au cours des 90 derniers jours pour tous les contacts du compte
* L’utilisateur peut mettre en surbrillance une semaine spécifique afin d’afficher les activités de cette semaine
* Affichage par défaut : la semaine en cours est sélectionnée

**Analyse et résumé de l’engagement**

* Cartes d’activité d’analyse pour les moments significatifs, l’e-mail et l’activité web, y compris le nom du contact
* Carte d’activité Moments significatifs - Inclut l’option S’abonner
* Carte d’activité E-mail - Inclut l’option Aperçu
* Carte d’activité web - Inclut la possibilité de cliquer sur le lien
* La barre de résumé hebdomadaire affiche les moments significatifs, l’e-mail et l’activité web de la semaine. Chaque icône est cliquable et peut être utilisée comme filtre pour afficher une activité spécifique
* Affichage par défaut : il s’agit d’une liste des activités de l’affichage actuel

**Campagnes et événements par e-mail à venir**

Onglet Campagnes par e-mail :

* Inclut les campagnes qui font partie de programmes de messagerie ou de programmes par défaut planifiés au cours des 90 prochains jours
* Non spécifique au contact/prospect (c’est-à-dire que la liste des campagnes est une liste générique de toutes les campagnes par e-mail planifiées dans l’instance Marketo). La liste des campagnes sur tous les panneaux de lead, contact, compte et opportunité sera la même
* Si la périodicité de la campagne est telle qu’elle s’exécute plus de trois fois au cours des 90 prochains jours, seules les trois exécutions suivantes s’affichent à un moment donné (comme dans Marketo)
* La vignette des détails de l’activité de cette section comporte une option de prévisualisation. Si le flux comprend plusieurs étapes d’envoi d’e-mail, tous les e-mails seront disponibles pour la prévisualisation. Dans l’étape Envoyer un e-mail , s’il existe plusieurs « choix d’e-mail », l’option par défaut est disponible pour la prévisualisation
* Les filtres incluent « [!UICONTROL Recherche] » et « [!UICONTROL Période] »

Onglet Événement :

* Inclut les programmes d’événement planifiés au cours des 90 prochains jours
* Utilisez l’option de filtre pour afficher tous les événements/événements invités (en fonction des paramètres d’administration)
* La sélection des événements invités affiche les événements auxquels un contact spécifique a été invité, ainsi que le statut de membre
* Lorsque vous sélectionnez tous les événements, la liste des événements planifiés pour les 90 prochains jours s’affiche
* La carte Détails de l’activité de cette section comporte une option de prévisualisation
* Le filtre comprend « [!UICONTROL Rechercher] », « [!UICONTROL Afficher uniquement les événements invités] » et « [!UICONTROL Période] »

## Mise en page de l’opportunité {#opportunity-layout}

**Grille de vitesse d’engagement**

* Cette grille dynamique comprend les moments significatifs, l’activité e-mail et web au cours des 90 derniers jours pour tous les contacts de l’opportunité
* L’utilisateur peut mettre en surbrillance une semaine spécifique afin d’afficher les activités de cette semaine
* Affichage par défaut : la semaine en cours est sélectionnée

**Analyse et résumé de l’engagement**

* Cartes d’activité d’analyse pour les moments significatifs, l’e-mail et l’activité web, y compris le nom du contact
* Carte d’activité Moments significatifs - Inclut l’option S’abonner
* Carte d’activité E-mail - Inclut l’option Aperçu
* Carte d’activité web - Inclut la possibilité de cliquer sur le lien
* La barre de résumé hebdomadaire affiche les moments significatifs, l’e-mail et l’activité web de la semaine. Chaque icône est cliquable et peut être utilisée comme filtre pour afficher une activité spécifique
* Affichage par défaut : il s’agit d’une liste des activités de l’affichage actuel

**Campagnes et événements par e-mail à venir** onglet Campagnes par e-mail :

* Inclut les campagnes qui font partie de programmes de messagerie ou de programmes par défaut planifiés au cours des 90 prochains jours
* Non spécifique au contact/prospect (c’est-à-dire que la liste des campagnes est une liste générique de toutes les campagnes par e-mail planifiées dans l’instance Marketo). La liste des campagnes sur tous les panneaux de lead, contact, compte et opportunité sera la même
* Si la périodicité de la campagne est telle qu’elle s’exécute plus de trois fois au cours des 90 prochains jours, seules les trois exécutions suivantes s’affichent à un moment donné (comme dans Marketo)
* La vignette des détails de l’activité de cette section comporte une option de prévisualisation. Si le flux comprend plusieurs étapes d’envoi d’e-mail, tous les e-mails seront disponibles pour la prévisualisation. Dans l’étape Envoyer un e-mail , s’il existe plusieurs « choix d’e-mail », l’option par défaut est disponible pour la prévisualisation
* Les filtres incluent « [!UICONTROL Recherche] » et « [!UICONTROL Période] »

Onglet Événement :

* Inclut les programmes d’événement planifiés au cours des 90 prochains jours
* Utilisez l’option de filtre pour afficher tous les événements/événements invités (en fonction des paramètres d’administration)
* La sélection des événements invités affiche les événements auxquels un contact spécifique a été invité, ainsi que le statut de membre
* Lorsque vous sélectionnez tous les événements, la liste des événements planifiés pour les 90 prochains jours s’affiche
* La carte Détails de l’activité de cette section comporte une option de prévisualisation
* Le filtre comprend « [!UICONTROL Rechercher] », « [!UICONTROL Afficher uniquement les événements invités] » et « [!UICONTROL Période] »

>[!NOTE]
>
>Si votre compte ou votre opportunité compte plus de 800 contacts, le tableau de bord n’affiche aucune donnée. Cependant, vous pouvez accéder à des contacts individuels pour voir leurs informations et leur engagement. Si votre compte comporte plus de 800 contacts, l’option « [!UICONTROL &#x200B; Afficher l’activité au niveau du compte &#x200B;] » est désactivée.
