---
unique-page-id: 30081815
description: Configuration de l’intégration Adobe Experience Manager - Documents Marketo - Documentation du produit
title: Configuration de l’intégration Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Configuration de l’intégration Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configurez Adobe Experience Manager (AEM) afin que vous puissiez accéder à des ressources AEM, les sélectionner et les importer dans Marketo Engage Design Studio.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!IMPORTANT]
>
>* Cette intégration fonctionne uniquement avec les implémentations on-premise d’AEM et n’est pas prise en charge pour les implémentations AEM Cloud Service.
>
>* Actuellement, cette fonctionnalité n’est entièrement prise en charge que dans Firefox. Elle n’est pas prise en charge dans Safari et peut ne pas fonctionner dans la dernière version de Chrome, selon vos paramètres de cookie SameSite.

1. Accédez à Adobe Experience Manager (l’URL est spécifique à votre entreprise).

   ![](assets/one.png)

1. Vous pouvez vous connecter avec Adobe ou vous connecter localement. Dans cet exemple, nous allons nous connecter localement.

   ![](assets/two.png)

1. Dans **[!UICONTROL Outils]**, cliquez sur **[!UICONTROL Opérations]** et sélectionnez **[!UICONTROL Console web]**.

   ![](assets/2a.png)

1. Dans votre navigateur, recherchez (ctrl+f sous Windows, cmd+f sous Mac) &quot;Adobe Granite Cross-Origin Resource Sharing Policy&quot;.

   ![](assets/three.png)

1. Cliquez sur le bouton **+** inscrivez-vous à droite.

   ![](assets/four.png)

1. Dans le **[!UICONTROL Origines autorisées (Regexp)]** zone de texte, saisissez `https://.*\.marketo\.com` et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/five-psd.png)

1. Dans l’en-tête en haut de la page, cliquez sur **[!UICONTROL Console web]** et sélectionnez **[!UICONTROL Informations système]**.

   ![](assets/six.png)

1. Sous Informations sur le serveur, cliquez sur le **[!UICONTROL Redémarrer]** bouton .

   ![](assets/seven.png)

1. Cliquez sur **[!UICONTROL OK]** pour confirmer.

   ![](assets/eight.png)

1. Dans Marketo Engage, cliquez sur **[!UICONTROL Administration]**.

   ![](assets/nine.png)

1. Sous Intégration, sélectionnez **[!UICONTROL Adobe Experience Manager]**.

   ![](assets/ten.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/eleven.png)

1. Saisissez votre URL d’AEM et cliquez sur **[!UICONTROL OK]**.

   ![](assets/twelve.png)
