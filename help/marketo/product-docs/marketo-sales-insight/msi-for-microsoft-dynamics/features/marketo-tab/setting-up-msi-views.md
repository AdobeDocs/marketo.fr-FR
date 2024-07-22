---
description: Configuration des vues MSI - Documents Marketo - Documentation du produit
title: Configuration des vues MSI
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 1%

---

# Configuration des vues MSI {#setting-up-msi-views}

L’installation du plug-in Sales Insight dans Dynamics ajoute automatiquement les Meilleurs billets et les tableaux de bord associés sur la carte du site. Si, pour une raison quelconque, les tableaux de bord ne sont pas ajoutés, voici comment les ajouter manuellement.

1. Dans Dynamics, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres avancés** dans la liste déroulante.

1. Dans le coin supérieur gauche de l’écran, cliquez sur **Paramètres**. Sous Personnalisation, sélectionnez **Personnalisations**.

1. Cliquez sur **Personnaliser le système**.

1. Dans l’arborescence de gauche, cliquez sur **Client Extensions** et double-cliquez sur **Site Map**.

1. Cliquez sur la flèche droite pour accéder à la page suivante. Sous Ventes, vous devriez voir Marketo. Dans le cas contraire, assurez-vous d’avoir importé le package correctement.

   >[!NOTE]
   >
   >Sous Marketo, vous devez disposer des éléments suivants : Meilleurs paris, Mon e-mail, Activité web et Activité web anonyme. Si l’un de ces tableaux de bord est manquant, cliquez sur le signe + au-dessus de Ventes et ajoutez-les en tant que sous-zone.

1. Cliquez sur un tableau de bord pour le sélectionner. Dans la colonne de droite, saisissez les informations correspondantes ci-dessous pour chacune d’elles. Vous pouvez ignorer les catégories qui ne sont pas répertoriées.

   **Meilleurs billets**</br>
URL : MainviewBestbets.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID : marketo_bestbets</br>
Titre : Best Bets

   **Mon email**</br>
URL : mkt_/MainViewMyEmail.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID : marketo_myemail</br>
Titre : My Email

   **Activité Web**</br>
URL : mkt_/MainViewWebActivity.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID : marketo_webactivity</br>
Titre : activité web

   **Activité Web anonyme**</br>
URL : mkt_/MainViewWebActivity.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID : marketo_anonymous_webactivity</br>
Titre : Activité Web anonyme

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.
