---
unique-page-id: 4720145
description: Découvrez l’implémentation de rtp à l’aide de Google Tag Manager dans Marketo Engage, y compris l’implémentation de rtp à l’aide de dnl google. Utilisez ce guide pour passer à l’étape suivante.
title: Mise en œuvre de RTP à l’aide de Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 3%

---

# Mise en œuvre du RTP à l’aide de [!DNL Google Tag Manager] {#implementing-rtp-using-google-tag-manager}

Pour implémenter votre balise RTP, suivez les instructions d’installation ci-dessous.

1. Connectez-vous à votre compte [!DNL Google Tag Manager].

1. Ajoutez une nouvelle **[!UICONTROL Balise]** > **[!UICONTROL Configurations des balises]** > **[!UICONTROL Balise HTML personnalisée].** l’appelle **RTP**.

1. Connectez-vous à votre **compte RTP**.

1. Accédez à **[!UICONTROL Paramètres du compte]**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance, passez à l’étape 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Sous [!UICONTROL Domaine], recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copiez la balise JavaScript RTP et collez-la dans la nouvelle **balise HTML personnalisée** créée (étape 1).

1. Cliquez sur **[!UICONTROL Ajouter une règle à la balise Fire]**. Sélectionnez **[!UICONTROL Toutes les pages]**.

1. Cliquez sur **[!UICONTROL Enregistrer]** et [publier la nouvelle version](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Vérifiez qu’il apparaît sur toutes les pages, y compris les pages de destination et les sous-domaines.

   a. Pour ce faire, cliquez avec le bouton droit de la souris sur la page de votre site web. Accédez à **[!UICONTROL Inspecter l’élément]**, recherchez **RTP** pour localiser la balise.
