---
unique-page-id: 4720151
description: Mise en œuvre du RTP sur les pages de destination de Marketo - Documents Marketo - Documentation du produit
title: Mise en œuvre du RTP sur les pages de destination de Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Mise en œuvre du RTP sur les pages de destination de Marketo {#implementing-rtp-on-marketo-landing-pages}

Pour implémenter votre balise [!UICONTROL RTP] suivez les instructions d’installation ci-dessous :

1. Accédez au **[!UICONTROL Design Studio].** Ouvrez l’élément que vous souhaitez modifier. Sélectionnez **[!UICONTROL Actions de modèle]**, puis **[!UICONTROL Modifier le brouillon]**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Apportez vos modifications de modèle dans l’onglet **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Dans votre compte RTP, accédez à **[!UICONTROL Paramètres du compte]**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Sous [!UICONTROL Domaine], recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copiez la balise JavaScript RTP et collez-la dans tous les modèles de page de destination compris entre les balises **`<head> </head>`**.

1. Cliquez sur **[!UICONTROL Enregistrer]** et **[!UICONTROL Fermer]** dans la fenêtre.

1. De retour dans **[!UICONTROL Design Studio]**, approuvez la page de destination à partir de **[!UICONTROL Actions de modèle]**, puis cliquez sur **[!UICONTROL Approuver]**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Enfin, vous devrez **réapprouver** toutes les pages de destination utilisant ce modèle pour que les modifications du modèle prennent effet. Vous pouvez toutes les approuver de nouveau en même temps à partir de la section principale [!UICONTROL Pages de destination].

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Vérifiez qu’il apparaît sur toutes les pages, y compris les pages de destination et les sous-domaines.

   Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **[!UICONTROL Afficher la page Source].** Rechercher **[!UICONTROL RTP]** pour localiser la balise.
