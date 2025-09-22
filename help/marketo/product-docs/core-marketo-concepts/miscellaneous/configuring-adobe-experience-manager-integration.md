---
unique-page-id: 30081815
description: Configuration de l’intégration Adobe Experience Manager - Documentation de Marketo - Documentation du produit
title: Configuration de l’intégration d’Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 7%

---

# Configuration de l’intégration d’Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configurez Adobe Experience Manager (AEM) pour pouvoir accéder aux ressources AEM, les sélectionner et les importer dans Marketo Engage Design Studio.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!IMPORTANT]
>
>* Cette intégration fonctionne uniquement avec les implémentations On-Premise d’AEM et n’est pas prise en charge pour les implémentations AEM Cloud Service.
>
>* Actuellement, cette fonctionnalité n’est entièrement prise en charge que dans Firefox. Il n’est pas pris en charge dans Safari et peut ne pas fonctionner dans la dernière version de Chrome, selon les paramètres de vos cookies SameSite.

1. Accédez au Adobe Experience Manager (l’URL est spécifique à votre société).

   ![](assets/one.png)

1. Vous pouvez vous connecter à l’aide d’Adobe ou vous connecter localement. Dans cet exemple, nous nous connecterons localement.

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

1. Sous Intégration, sélectionnez **[!UICONTROL Adobe Experience Manager]**.

   ![](assets/ten.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/eleven.png)

1. Saisissez l’URL d’AEM, puis cliquez sur **[!UICONTROL OK]**.

   ![](assets/twelve.png)
