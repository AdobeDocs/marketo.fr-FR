---
description: Configuration de Sales Insight pour votre équipe - Marketo Docs - Documentation sur les produits
title: Configuration de Sales Insight pour votre équipe
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Configuration de Sales Insight pour votre équipe {#setting-up-sales-insight-for-your-team}

Voici comment créer un profil avec accès à Sales Insight tout en supprimant l&#39;accès pour vos autres profils. Il s’agit des utilisateurs qui ont déjà installé le [module d’AppExchange Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).

## Créer un nouveau Profil pour Sales Insight {#create-a-new-profile-for-sales-insight}

Si vous disposez d&#39;un profil dédié pour vos utilisateurs de Sales Insight, vous pouvez ignorer cette étape.

1. Dans Salesforce, accédez à la page Configuration.

1. Recherchez des profils dans Recherche rapide et sélectionnez l&#39;option **Profil**.

1. Cliquez sur le bouton **Nouveau Profil** en haut de la page.

1. Choisissez un profil à cloner et donnez-lui un nom (ex : Utilisateur Sales Insight).

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

## Autorisations d&#39;Ajoute Sales Insight {#add-sales-insight-permissions}

1. Retournez à votre liste de Profils.

1. Cliquez sur le lien **Modifier** pour le nouveau profil que vous venez de créer (ou tout autre profil existant auquel vous souhaitez donner accès à Sales Insight).

1. Dans la page de modification, vous devez modifier quelques paramètres.

   **Pour les profils autorisés à accéder à Sales Insight** :

   * Dans Paramètres d’application personnalisés, cochez la case Marketo pour rendre l’application Marketo visible.
   * Dans les paramètres d’onglet, remplacez les onglets Marqueur par Par défaut activé.
   * Dans Autorisations d’objet personnalisé, cochez les options Lire, Créer, Modifier et Supprimer dans la configuration de Marketing Cloud Sales Insight (si l’utilisateur doit avoir accès aux paramètres de configuration - généralement utilisés pour les administrateurs).

   **Pour les profils qui n&#39;ont pas accès à Sales Insight** :

   * Dans Paramètres d’application personnalisés, décochez la case Marketo pour masquer l’application Marketo.
   * Dans les paramètres d’onglet, remplacez les onglets Marque par Tabulation masquée.
   * Dans Autorisations d’objet personnalisées, décochez la case Lire, Créer, Modifier et Supprimer dans la configuration des statistiques commerciales de marketing.


1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

## Créer une mise en page pour Sales Insight {#create-layout-for-sales-insight}

1. Accédez à la page Configuration, puis cliquez sur **Configuration de l’application** > **Personnaliser** > **Pistes** > **Mise en page**. Cliquez ensuite sur le bouton **Nouveau**.

1. Clonez votre mise en page de votre choix et donnez-lui un nom approprié (ex : Disposition des statistiques commerciales).

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

1. Répétez ces étapes pour les dispositions de page Contacts, Opportunités et Comptes.

## Attribuer le Profil à la mise en page {#assign-profile-to-layout}

1. Retournez à la section Mise en page et cliquez sur le bouton **Affectation de mise en page**.

1. Sélectionnez **Modifier l&#39;affectation**.

1. Sélectionnez votre profil Sales Insight dans la liste, puis sélectionnez votre mise en page Sales Insight dans la liste déroulante Select Page Layout (Sélectionner la mise en page).

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

1. Répétez ces étapes pour les dispositions de page Contacts, Opportunités et Comptes.

## Autres modifications {#other-changes}

Voici d&#39;autres endroits où des articles Sales Insight peuvent apparaître. Vous devrez les supprimer immédiatement, car vous ne pouvez pas utiliser de Profils pour limiter leur accès :

* Supprimer les boutons Sales Insight des dispositions de recherche pour les contacts, les pistes et les comptes
* Supprimer les colonnes Sales Insight des listes de contacts et de pistes
