---
description: Configuration des vues MSI - Documents Marketo - Documentation du produit
title: Configuration des vues MSI
source-git-commit: 8227648ce67bf0f9f8b3b2fea7445850d8e154d5
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Configuration des vues MSI {#setting-up-msi-views}

L’installation du plug-in Sales Insight dans Dynamics ajoute automatiquement les Meilleurs billets et les tableaux de bord associés sur la carte du site. Si, pour une raison quelconque, les tableaux de bord ne sont pas ajoutés, voici comment les ajouter manuellement.

1. Dans Dynamics, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres avancés** dans la liste déroulante.

1. Dans le coin supérieur gauche de l’écran, cliquez sur **Paramètres**. Sous Personnalisation , choisissez **Personnalisations**.

1. Cliquez sur **Personnalisation du système**.

1. Dans l’arborescence de gauche, cliquez sur **Extensions client** et double-cliquez **Carte du site**.

1. Cliquez sur la flèche droite pour accéder à la page suivante. Sous Ventes, vous devriez voir Marketo. Dans le cas contraire, assurez-vous d’avoir importé le package correctement.

   >[!NOTE]
   >
   >Sous Marketo, vous devez disposer des éléments suivants : Meilleurs paris, Mon email, Activité web et Activité web anonyme. Si l’un de ces tableaux de bord est manquant, cliquez sur le signe + au-dessus de Ventes et ajoutez-les en tant que sous-zone.

1. Cliquez sur un tableau de bord pour le sélectionner. Dans la colonne de droite, saisissez les informations correspondantes ci-dessous pour chacune d’elles. Vous pouvez ignorer les catégories qui ne sont pas répertoriées.

   **Meilleurs paris**</br>
URL : MainviewBestbets.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID : marketo_bestbets</br>
Titre : Meilleurs paris

   **Mon courriel**</br>
URL : mkt_/MainViewMyEmail.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID : marketo_myemail</br>
Titre : Mon courriel

   **Activité web**</br>
URL : mkt_/MainViewWebActivity.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID : marketo_webactivity</br>
Titre : Activité web

   **Activité Web anonyme**</br>
URL : mkt_/MainViewWebActivity.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID : marketo_anonymous_webactivity</br>
Titre : Activité Web anonyme

1. Cliquez sur **Enregistrer** une fois terminé.
