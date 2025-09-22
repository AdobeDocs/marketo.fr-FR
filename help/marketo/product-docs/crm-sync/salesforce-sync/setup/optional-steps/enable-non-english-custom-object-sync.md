---
unique-page-id: 4719302
description: Activer La Synchronisation D’Objets Personnalisés Non Anglais - Documents Marketo - Documentation Du Produit
title: Activer la synchronisation des objets personnalisés dans des langues autres que l’anglais
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 9%

---

# Activer la synchronisation des objets personnalisés dans des langues autres que l’anglais {#enable-non-english-custom-object-sync}

Si votre utilisateur de synchronisation Marketo est défini sur une langue autre que l’anglais, une erreur peut se produire lors de l’activation d’une synchronisation d’objet personnalisée.

## L’erreur {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Contournement {#getting-around-it}

1. Connectez-vous à [!DNL Salesforce] à l’aide de l’utilisateur de synchronisation marketo.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Sous le nom d’utilisateur, accédez à **[!UICONTROL Configuration]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Sous **[!UICONTROL Informations personnelles]**, cliquez sur **[!UICONTROL Mes informations personnelles]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Remplacez **[!UICONTROL Langue]** par **[!UICONTROL Anglais]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. De retour dans Marketo, sous **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objets]**, cliquez sur **[!UICONTROL Actualiser le schéma]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. La liste d’objets sera alors extraite en anglais. Sélectionnez maintenant l’objet de votre choix et cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Notez que votre objet personnalisé est maintenant activé et en cours de synchronisation.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Revenez maintenant à [!DNL Salesforce] et suivez les étapes ci-dessus pour rétablir la langue de votre choix pour l’utilisateur de la synchronisation.

>[!NOTE]
>
>N’oubliez pas d’actualiser le schéma une dernière fois pour récupérer les objets dans votre langue.
