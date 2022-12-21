---
unique-page-id: 10099680
description: Importation de données d’objet personnalisées - Documents Marketo - Documentation du produit
title: Importer les données de l’objet personnalisé
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Importer les données de l’objet personnalisé {#import-custom-object-data}

Il est facile d’importer des données d’objet personnalisées dans votre base de données. Si vous utilisez des objets personnalisés avec des entreprises, reportez-vous à la section [Utilisation d’objets personnalisés avec des entreprises](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) pour plus d’informations.

1. Dans Mon Marketo, accédez à **Base**.

   ![](assets/db-1.png)

1. Cliquez sur **Nouveau** et sélectionnez **Importer des données d’objet personnalisées**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Cliquez sur **Parcourir** pour localiser le fichier de données. Sélectionnez le format de fichier (valeurs séparées par des virgules dans cet exemple).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Sélectionnez votre objet personnalisé.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Sélectionnez le mode Déduplication dans la liste déroulante. Cliquez sur **Suivant**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Utilisez des champs de déduplication comme identifiants uniques lorsque vous créez ou mettez à jour des enregistrements d’objet personnalisés. Cet exemple utilise le champ Déduplication de la propriété **car** objet personnalisé - numéro d’identification du véhicule. Si vous mettez uniquement à jour des enregistrements d’objet personnalisés, vous pouvez sélectionner le guide Marketo comme mode de déduplication.

1. Faites correspondre chaque colonne à un champ Marketo, en la sélectionnant dans la liste déroulante.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Assurez-vous que les valeurs de votre fichier correspondent au type de champ auquel vous les associez (par exemple, texte, entier, etc.), sinon le fichier sera rejeté.

1. Cliquez sur **Suivant**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Cliquez sur **Importer**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >La taille des objets personnalisés est limitée à 100 Mo.

   >[!TIP]
   >
   >Saisissez votre adresse électronique dans la zone **Envoyer une alerte à :** et Marketo vous enverra un e-mail une fois votre importation terminée.

1. Dans le coin supérieur droit de l’écran, une notification s’affiche pendant l’exécution de l’importation et les résultats finaux une fois l’importation terminée.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Oui !

>[!MORELIKETHIS]
>
>[Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
