---
unique-page-id: 10099680
description: Importation de données d’objet personnalisées - Documents Marketo - Documentation du produit
title: Importer les données de l’objet personnalisé
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Importer les données de l’objet personnalisé {#import-custom-object-data}

Vous pouvez facilement importer des données d’objet personnalisées dans votre base de données. Si vous utilisez des objets personnalisés avec des entreprises, reportez-vous à la section [Utilisation d’objets personnalisés avec des entreprises](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) pour plus d’informations.

1. Dans My Marketo, accédez à **[!UICONTROL Base de données]**.

   ![](assets/import-custom-object-data-1.png)

1. Cliquez sur **[!UICONTROL New]** et sélectionnez **[!UICONTROL Importer des données d’objet personnalisées]**.

   ![](assets/import-custom-object-data-2.png)

1. Cliquez sur **[!UICONTROL Parcourir]** pour localiser le fichier de données. Sélectionnez le format de fichier (valeurs séparées par des virgules dans cet exemple).

   ![](assets/import-custom-object-data-3.png)

1. Sélectionnez votre [!UICONTROL objet personnalisé].

   ![](assets/import-custom-object-data-4.png)

1. Sélectionnez le [!UICONTROL mode déduplication] dans la liste déroulante. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Utilisez des champs de déduplication comme identifiants uniques lorsque vous créez ou mettez à jour des enregistrements d’objet personnalisés. Cet exemple utilise le champ Dedupe de l’objet personnalisé **car** - numéro d’identification du véhicule). Si vous mettez uniquement à jour des enregistrements d’objet personnalisés, vous pouvez sélectionner le [!UICONTROL Marketo Guid] comme .

1. Faites correspondre chaque colonne à un champ Marketo, en la sélectionnant dans la liste déroulante.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Assurez-vous que les valeurs de votre fichier correspondent au type de champ auquel vous les associez (par exemple, texte, entier, etc.), sinon le fichier sera rejeté.

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-custom-object-data-7.png)

1. Cliquez sur **[!UICONTROL Importer]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >La taille des objets personnalisés est limitée à 100 Mo.

   >[!TIP]
   >
   >Entrez votre adresse électronique dans le champ **[!UICONTROL Envoyer une alerte à]** et Marketo vous enverra par courrier électronique une fois votre importation terminée !

1. Dans le coin supérieur droit de l’écran, une notification s’affiche pendant l’exécution de l’importation et les résultats finaux une fois l’importation terminée.

   ![](assets/import-custom-object-data-9.png)

   Oui !

>[!MORELIKETHIS]
>
>[Compréhension des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
