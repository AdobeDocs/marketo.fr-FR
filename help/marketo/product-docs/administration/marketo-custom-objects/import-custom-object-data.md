---
unique-page-id: 10099680
description: Étapes d’importation de données d’objet personnalisées à l’aide d’un fichier CSV, notamment la sélection de l’objet personnalisé, le mode de déduplication et le mappage des champs.
title: Importer les données de l’objet personnalisé
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 40d7e8a0723946970c49a6dfc4f0de4c71b0df65
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 4%

---

# Importer les données de l’objet personnalisé {#import-custom-object-data}

Suivez les étapes ci-dessous pour importer des données d’objet personnalisées dans votre base de données. Si vous utilisez des objets personnalisés avec des sociétés, voir [Utilisation d’objets personnalisés avec des sociétés](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) pour plus d’informations.

1. Dans Mon Marketo, accédez à **[!UICONTROL Base de données]**.

   ![](assets/import-custom-object-data-1.png)

1. Cliquez sur **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Importer des données d’objet personnalisé]**.

   ![](assets/import-custom-object-data-2.png)

1. Cliquez sur **[!UICONTROL Parcourir]** pour localiser le fichier de données. Sélectionnez le format du fichier (valeurs séparées par des virgules dans cet exemple).

   ![](assets/import-custom-object-data-3.png)

1. Sélectionnez votre [!UICONTROL objet personnalisé].

   ![](assets/import-custom-object-data-4.png)

1. Sélectionnez le [!UICONTROL Mode de déduplication] dans la liste déroulante. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Utilisez un ou plusieurs champs Dédupliquer comme identifiants uniques lorsque vous créez ou mettez à jour des enregistrements d’objet personnalisés. Cet exemple utilise le champ Dédupliquer de l’objet personnalisé **car** vin (numéro d’ID du véhicule). Si vous mettez uniquement à jour les enregistrements d&#39;objet personnalisés, vous pouvez sélectionner le Guid de Marketo  comme [!UICONTROL Mode de déduplication].

1. Mappez chaque colonne à un champ Marketo, en la sélectionnant dans la liste déroulante.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Assurez-vous que les valeurs de votre fichier correspondent au type de champ auquel vous les faites correspondre (par exemple, texte, entier, etc.), sinon le fichier sera rejeté.

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-custom-object-data-7.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >La limite de taille des objets personnalisés est 100MB.

   >[!TIP]
   >
   >Saisissez votre adresse e-mail dans le champ **[!UICONTROL Envoyer l’alerte à]** et Marketo vous enverra un e-mail une fois l’importation terminée.

1. Dans le coin supérieur droit de l’écran, une notification s’affiche pendant l’exécution de l’importation et les résultats finaux une fois celle-ci terminée.

   ![](assets/import-custom-object-data-9.png)

>[!MORELIKETHIS]
>
>[Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
