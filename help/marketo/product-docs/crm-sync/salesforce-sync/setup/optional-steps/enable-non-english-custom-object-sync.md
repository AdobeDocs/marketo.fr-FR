---
unique-page-id: 4719302
description: Découvrez comment activer la synchronisation d’objets personnalisée lorsque l’utilisateur de la synchronisation Marketo utilise une langue autre que l’anglais. Définissez la langue de synchronisation des utilisateurs sur Anglais dans Salesforce et actualisez le schéma.
title: Activer la synchronisation des objets personnalisés dans des langues autres que l’anglais
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/kPzDEdjDnDAvuJmCtPj0I2Lfl63Lset00t-LwB8DDhI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 67c57a9162946c4b9c424ab3fd445b70e90b530a
workflow-type: tm+mt
source-wordcount: 195
ht-degree: 9%

---

# Activer la synchronisation des objets personnalisés dans des langues autres que l’anglais {#enable-non-english-custom-object-sync}

Si votre utilisateur de synchronisation Marketo est défini sur une langue autre que l’anglais, une erreur peut se produire lors de l’activation d’une synchronisation d’objet personnalisée.

![](assets/image2014-12-10-13-3a17-3a51.png)

## Comment résoudre le problème {#how-to-fix}

1. Connectez-vous à [!DNL Salesforce] à l’aide de l’utilisateur de synchronisation marketo.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Cliquez sur le menu déroulant du nom d’utilisateur et sélectionnez **[!UICONTROL Configuration]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Sous **[!UICONTROL Informations personnelles]**, cliquez sur **[!UICONTROL Mes informations personnelles]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Remplacez **[!UICONTROL Langue]** par **[!UICONTROL Anglais]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Dans votre [profil de compte &#x200B;](https://account.adobe.com/profile){target="_blank"}, faites défiler l’écran jusqu’à **[!UICONTROL Langues préférées]** et assurez-vous que la langue maternelle est l’anglais.

   ![](assets/enable-non-english-custom-object-sync-step-6.5.png)

1. Dans Marketo Engage, accédez à **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objets]**. Cliquez sur **[!UICONTROL Actualiser le schéma]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. La liste des objets est alors extraite en anglais. Sélectionnez l’objet de votre choix et cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Votre objet personnalisé est maintenant activé et synchronisé.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Revenez à [!DNL Salesforce] et suivez les étapes ci-dessus pour rétablir la langue de votre choix pour l’utilisateur de synchronisation.

>[!NOTE]
>
>Actualisez le schéma une dernière fois pour récupérer les objets dans votre langue.
