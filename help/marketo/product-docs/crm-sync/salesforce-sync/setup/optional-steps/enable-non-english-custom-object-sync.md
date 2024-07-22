---
unique-page-id: 4719302
description: Activer la synchronisation d’objets personnalisés non anglais - Documents Marketo - Documentation du produit
title: Activer la synchronisation d’objets personnalisés non anglais
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 1%

---

# Activer la synchronisation d’objets personnalisés non anglais {#enable-non-english-custom-object-sync}

Si votre utilisateur de synchronisation Marketo est défini sur une autre langue que l’anglais, une erreur peut se produire lors de l’activation d’une synchronisation d’objet personnalisée.

## L’erreur {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Comment le contourner {#getting-around-it}

1. Connectez-vous à [!DNL Salesforce] à l’aide de l’utilisateur de synchronisation Marketo.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Sous le nom d’utilisateur, accédez à **[!UICONTROL Configuration]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Sous **[!UICONTROL Personal Information]**, cliquez sur **[!UICONTROL My Personal Information]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Remplacez la **[!UICONTROL langue]** par **[!UICONTROL anglais]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. De retour dans Marketo, sous **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objets]**, cliquez sur **[!UICONTROL Actualiser le schéma]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Cette opération extrait la liste des objets en anglais. Sélectionnez maintenant l’objet de votre choix et cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Notez que votre objet personnalisé est maintenant activé et synchronisé.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Revenez maintenant à Salesforce et utilisez les étapes ci-dessus pour redéfinir l’utilisateur de synchronisation dans la langue de votre choix.

>[!NOTE]
>
>N’oubliez pas d’actualiser le schéma une dernière fois pour récupérer les objets dans votre langue.
