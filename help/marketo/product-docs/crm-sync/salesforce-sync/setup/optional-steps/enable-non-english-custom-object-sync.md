---
unique-page-id: 4719302
description: Activer la synchronisation d'objets personnalisés en d'autres langues que l'anglais - Documents marketing - Documentation du produit
title: Activer la synchronisation d’objets personnalisés en anglais non
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Activer la synchronisation d&#39;objets personnalisés non anglais {#enable-non-english-custom-object-sync}

Si votre utilisateur de synchronisation Marketo utilise une autre langue que l’anglais, vous pouvez rencontrer une erreur lors de l’activation d’une synchronisation d’objets personnalisée.

## Erreur {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Obtenir le résultat {#getting-around-it}

1. Connectez-vous à Salesforce à l’aide de l’utilisateur de synchronisation marketing.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Sous le nom d’utilisateur, accédez à **Configuration**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Sous **Informations personnelles**, cliquez sur **Mes informations personnelles**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Cliquez sur **Modifier**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Remplacez **Language** par **English**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. De retour dans Marketo, sous **Admin > Salesforce > Objets** cliquez sur **Actualiser le Schéma**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Cela va extraire les objets liste en anglais. Sélectionnez maintenant l’objet de votre choix et cliquez sur **Activer la synchronisation**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Notez que votre objet personnalisé est désormais activé et synchronisé.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Revenez maintenant à Salesforce et suivez les étapes ci-dessus pour rétablir la langue de votre choix pour l’utilisateur de synchronisation.

>[!NOTE]
>
>**Rappel**
>
>N&#39;oubliez pas d&#39;actualiser le Schéma une dernière fois pour retirer les objets dans votre langue.

