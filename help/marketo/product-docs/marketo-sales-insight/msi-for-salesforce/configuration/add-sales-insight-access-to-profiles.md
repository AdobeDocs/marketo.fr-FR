---
description: Ajout de l’accès Sales Insight aux profils - Documents Marketo - Documentation du produit
title: Ajout de l’accès Sales Insight aux profils
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 3%

---

# Ajout de l’accès Sales Insight aux profils {#add-sales-insight-access-to-profiles}

Voici comment créer un profil ayant accès à Sales Insight tout en supprimant l’accès pour vos autres profils. Cela est destiné aux utilisateurs qui ont déjà installé le [package d’AppExchange Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Si vous avez auparavant donné l’accès à Sales Insight à tous les profils, vous devez [ supprimer l’accès au niveau de profil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} pour utiliser ce jeu d’autorisations.

## Création d’un profil pour Sales Insight {#create-a-new-profile-for-sales-insight}

Si vous disposez d’un profil dédié pour vos utilisateurs de Sales Insight, vous pouvez ignorer cette étape.

1. Dans Salesforce, accédez à la page Configuration .

1. Recherchez des profils dans Recherche rapide et sélectionnez l’option **Profil** .

1. Cliquez sur le bouton **Nouveau profil** en haut de la page.

1. Sélectionnez un profil à cloner et donnez-lui un nom (ex : utilisateur Sales Insight).

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

## Ajout d’autorisations Sales Insight {#add-sales-insight-permissions}

1. Revenez à votre liste Profils .

1. Cliquez sur le lien **Modifier** pour le nouveau profil que vous venez de créer (ou tout autre profil existant auquel vous souhaitez donner accès aux statistiques sur les ventes).

1. Sur la page de modification, vous devez modifier quelques paramètres.

   **Pour les profils qui ont accès à Sales Insight** :

   * Dans les paramètres de tabulation, définissez les onglets Marketo sur Activé par défaut.
   * Dans Autorisations d’objet personnalisé, cochez l’option Lire, Créer, Modifier et Supprimer dans la configuration de Marketo Sales Insight (si l’utilisateur doit avoir accès aux paramètres de configuration, généralement utilisés pour les administrateurs).

   **Pour les profils qui n’ont pas accès à Sales Insight** :

   * Dans les paramètres de tabulation, remplacez les onglets Marketo par Tabulation masquée
   * Dans Autorisations d’objet personnalisé, désélectionnez Lire, Créer, Modifier et Supprimer dans la configuration de Marketo Sales Insight

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

## Créer une mise en page pour Sales Insight {#create-layout-for-sales-insight}

1. Accédez à la page Configuration, puis cliquez sur **Configuration de l’application** > **Personnaliser** > **Pistes** > **Mises en page**. Cliquez ensuite sur le bouton **New** .

1. Cloner votre mise en page de votre choix et attribuer un nom approprié à la mise en page (par exemple : disposition des statistiques sur les ventes).

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

1. Répétez ces étapes pour les mises en page de vos contacts, opportunités et comptes.

## Attribution d’un profil à la mise en page {#assign-profile-to-layout}

1. Revenez à la section Mise en page et cliquez sur le bouton **Attribution de mise en page** .

1. Sélectionnez **Modifier l’affectation**.

1. Sélectionnez votre profil Sales Insight dans la liste, puis sélectionnez votre disposition Sales Insight dans la liste déroulante &quot;Select Page Layout&quot; (Sélectionner la mise en page).

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

1. Répétez ces étapes pour les mises en page de vos contacts, opportunités et comptes.

## Autres modifications {#other-changes}

Voici d’autres endroits où des éléments d’aperçu commercial peuvent apparaître. Vous devrez les supprimer immédiatement, car vous ne pouvez pas utiliser Profils pour limiter leur accès :

* Suppression des boutons Insight sur les ventes des dispositions de recherche pour les contacts, les pistes et les comptes
* Suppression des colonnes Sales Insight des listes de contacts et de pistes
