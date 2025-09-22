---
description: Configuration des vues MSI - Documents Marketo - Documentation du produit
title: Configuration des vues MSI
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 4%

---

# Configuration des vues MSI {#setting-up-msi-views}

L’installation du plug-in [!DNL Sales Insight] dans Dynamics ajoute automatiquement les [!DNL Best Bets] et les tableaux de bord associés sur la carte du site. Si, pour une raison quelconque, les tableaux de bord ne sont pas ajoutés, voici comment les ajouter manuellement.

1. Dans Dynamics, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres avancés]** dans la liste déroulante.

1. Dans le coin supérieur gauche de l’écran, cliquez sur **[!UICONTROL Paramètres]**. Sous Personnalisation, choisissez **[!UICONTROL Personnalisations]**.

1. Cliquez sur **[!UICONTROL Personnaliser le système]**.

1. Dans l’arborescence de gauche, cliquez sur **[!UICONTROL Extensions client]** puis double-cliquez sur **[!UICONTROL Plan du site]**.

1. Cliquez sur la flèche de droite pour accéder à la page suivante. Sous Ventes, vous devriez voir Marketo. Si ce n&#39;est pas le cas, veillez à importer le package correctement.

   >[!NOTE]
   >
   >Sous Marketo, vous devriez avoir : Meilleurs paris, Mon e-mail, Activité web et Activité web anonyme. Si l’un de ces tableaux de bord est manquant, cliquez sur le signe + au-dessus des Ventes et ajoutez-les en tant que sous-zone.

1. Cliquez sur un tableau de bord pour le sélectionner. Dans la colonne de droite, saisissez les informations respectives ci-dessous pour chacun d’eux. Vous pouvez ignorer les catégories non répertoriées.

   **Meilleurs paris**</br>
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
Titre : activité web

   **Activité Web anonyme**</br>
URL : mkt_/MainViewWebActivity.html</br>
Icône : /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID : marketo_anonymous_webactivity</br>
Titre : activité Web anonyme

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.
