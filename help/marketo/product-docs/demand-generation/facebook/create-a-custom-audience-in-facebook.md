---
unique-page-id: 4720275
description: Création d’une audience personnalisée sur Facebook - Documents Marketo - Documentation du produit
title: Créer une audience personnalisée dans Facebook
exl-id: a2c8d89c-16b3-44f6-a2c6-c52fe78ab39c
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 3%

---

# Création d’une audience personnalisée dans [!DNL Facebook] {#create-a-custom-audience-in-facebook}

>[!PREREQUISITES]
>
>* [Ajout  [!DNL Facebook]  audiences personnalisées en tant que service LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md){target="_blank"} dans la section Admin.
>* [Acceptez [!DNL Facebook] les conditions relatives aux audiences personnalisées](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} dans votre compte [!DNL Facebook].

>[!TIP]
>
>En savoir plus sur les [&#x200B; audiences personnalisées dans  [!DNL Facebook]](https://www.facebook.com/help/341425252616329){target="_blank"}.

1. Recherchez et sélectionnez la liste dynamique ou statique qui contient les prospects à partir desquels vous souhaitez créer l’audience.

   ![](assets/create-a-custom-audience-in-facebook-1.png)

1. Sélectionnez l’onglet **[!UICONTROL Leads]**, puis cliquez sur l’icône **Envoyer via Ad Bridge** en bas.

   ![](assets/create-a-custom-audience-in-facebook-2.png)

1. Sélectionnez **[!UICONTROL Facebook]** et cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/create-a-custom-audience-in-facebook-3.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Audience]** et sélectionnez **[!UICONTROL + Nouvelle audience]**.

   ![](assets/create-a-custom-audience-in-facebook-4.png)

   >[!IMPORTANT]
   >
   >L’API Facebook autorise jusqu’à 500 audiences personnalisées par compte publicitaire Facebook.

1. Saisissez un **[!UICONTROL Nom de l’audience]**. Cliquez sur **[!UICONTROL Mettre à jour]**.

   ![](assets/create-a-custom-audience-in-facebook-5.png)

   >[!NOTE]
   >
   >Si vous disposez de plusieurs comptes publicitaires [!DNL Facebook], une liste déroulante supplémentaire s’affiche, vous permettant de choisir dans quel compte publicitaire cette audience est créée.

   >[!TIP]
   >
   >Vous souhaitez échanger une nouvelle audience avec une audience existante actuellement associée à une visionneuse d’annonces ou à un groupe ? Cochez la case **[!UICONTROL Remplacer une audience existante]**. Cela ne supprimera **pas** l’audience remplacée.

1. Une fois cette opération terminée, la boîte de dialogue d’état est mise à jour.

   ![](assets/create-a-custom-audience-in-facebook-6.png)

   Et c&#39;est tout ! Dans Facebook, vous verrez la nouvelle audience dans **Gestionnaire de publicités** > **Audiences**.

   ![](assets/create-a-custom-audience-in-facebook-7.png)

   >[!NOTE]
   >
   >Toutes les listes que vous poussez vers [!DNL Facebook] deviennent statiques. Les listes dynamiques dans Marketo ne mettent pas automatiquement à jour la liste des audiences en [!DNL Facebook] pour refléter les modifications apportées après le transfert.

   >[!MORELIKETHIS]
   >
   >[Ajout de leads à une audience personnalisée dans  [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/add-leads-to-a-custom-audience-in-facebook.md)
