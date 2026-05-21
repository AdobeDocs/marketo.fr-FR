---
unique-page-id: 30081815
description: Découvrez comment configurer l’intégration de Adobe Experience Manager à Marketo. Configurez AEM afin de pouvoir accéder aux ressources et les importer dans Design Studio.
title: Configuration de l’intégration d’Adobe Experience Manager
hide: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
TQID: https://experienceleague.adobe.com/nJBydVi8mRwVf1vAIFuI1S3nEuX0FGiztp8fhRHq6RM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 8%

---

# Configuration de l’intégration d’Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configurez Adobe Experience Manager (AEM) pour pouvoir accéder aux ressources AEM, les sélectionner et les importer dans Marketo Engage Design Studio.

>[!NOTE]
>
>**Autorisations d’administration requises**

>[!IMPORTANT]
>
>* Cette intégration fonctionne uniquement avec les implémentations On-Premise d’AEM et n’est pas prise en charge pour les implémentations AEM Cloud Service.
>
>* Actuellement, cette fonctionnalité n’est entièrement prise en charge que dans Firefox. Il n’est pas pris en charge dans Safari et peut ne pas fonctionner dans la dernière version de Chrome, selon les paramètres de vos cookies SameSite.

1. Accédez au Adobe Experience Manager (l’URL est spécifique à votre société).

   ![](assets/one.png)

1. Vous pouvez vous connecter à l’aide d’Adobe ou vous connecter localement. Cet exemple utilise la connexion locale.

   ![](assets/two.png)

1. Dans **[!UICONTROL Outils]**, cliquez sur **[!UICONTROL Opérations]** et sélectionnez **[!UICONTROL Console web]**.

   ![](assets/2a.png)

1. Dans votre navigateur, recherchez « [!UICONTROL Politique de partage de ressources entre origines multiples Adobe Granite ] » (ctrl+f sous Windows, cmd+f sous Mac).

   ![](assets/three.png)

1. Cliquez sur le signe **+** à droite.

   ![](assets/four.png)

1. Dans la zone de texte **[!UICONTROL Origines autorisées (Regexp)]**, saisissez `https://.*\.marketo\.com` et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/five-psd.png)

1. Dans l’en-tête situé en haut de la page, cliquez sur **[!UICONTROL Console web]** et sélectionnez **[!UICONTROL Informations système]**.

   ![](assets/six.png)

1. Sous Server Information, cliquez sur le bouton **[!UICONTROL Redémarrer]**.

   ![](assets/seven.png)

1. Cliquez sur **[!UICONTROL OK]** pour confirmer.

   ![](assets/eight.png)

1. Dans Marketo Engage, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/nine.png)

1. Sous Intégration, sélectionnez ****.

   ![](assets/ten.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/eleven.png)

1. Saisissez l’URL d’AEM, puis cliquez sur **[!UICONTROL OK]**.

   ![](assets/twelve.png)
