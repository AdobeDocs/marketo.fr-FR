---
description: Configuration des vues MSI - Documentation Marketo Docs - Documentation du produit
title: Configuration des vues MSI
hide: true
hidefromtoc: true
source-git-commit: f4930d1747f1ca893d7494afc3dcbeb8c6398e93
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Configuration des vues MSI {#setting-up-msi-views}

L’installation du module externe Sales Insight dans Dynamics ajoute automatiquement les Best Bets et les tableaux de bord associés sur la carte du site. Si, pour une raison quelconque, les tableaux de bord ne sont pas ajoutés, voici comment les ajouter manuellement.

1. Dans Dynamics, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres avancés** dans la liste déroulante.

1. Dans le coin supérieur gauche de l’écran, cliquez sur **Paramètres**. Sous Personnalisation, choisissez Personnalisations.

1. Cliquez sur **Personnalisation du système**.

1. Dans l’arborescence de gauche, cliquez sur **Extensions client** et double-cliquez sur **Plan du site**.

1. Cliquez sur la flèche droite pour accéder à la page suivante. Sous Ventes, vous devriez voir Marketo. Si ce n’est pas le cas, assurez-vous d’avoir importé le package correctement.

   >[!NOTE]
   >
   >Sous Marketo, vous devriez avoir : Meilleurs paris, Mon e-mail, Activité Web et Activité Web anonyme. Si l’un de ces tableaux de bord est manquant, cliquez sur le signe + au-dessus de Ventes et ajoutez-les en tant que sous-zone.

1. Cliquez sur un tableau de bord pour le sélectionner. Dans la colonne de droite, entrez les informations correspondantes ci-dessous pour chacune d’elles. Vous pouvez ignorer les catégories non répertoriées.

   **Meilleurs résultats**</br>
URL : MainviewBestbets.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID : marketo_bestbets</br>
Titre : Meilleurs résultats

   **Mon e-mail**</br>
URL : mkt_/MainViewMyEmail.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID : marketo_myemail</br>
Titre : Mon e-mail

   **Activité Web**</br>
URL : mkt_/MainViewWebActivity.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID : marketo_webactivity</br>
Titre : Activité Web

   **Activité Web anonyme**</br>
URL : mkt_/MainViewWebActivity.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID : marketo_anonymous_webactivity</br>
Titre : Activité Web anonyme

1. Cliquez sur **Enregistrer** une fois terminé.
