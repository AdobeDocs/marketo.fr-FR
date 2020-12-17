---
unique-page-id: 10099680
description: Importer des données d’objet personnalisées - Documents marketing - Documentation du produit
title: Importer des données d’objet personnalisées
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Importer des données d&#39;objet personnalisé {#import-custom-object-data}

Il est facile d&#39;importer des données d&#39;objet personnalisées dans votre base de données. Si vous utilisez des objets personnalisés avec des sociétés, voir [Utilisation d’objets personnalisés avec des Sociétés](http://docs.marketo.com/display/DOCS/Understanding+Marketo+Custom+Objects#UnderstandingMarketoCustomObjects-customcompanyUsingCustomObjectswithCompanies) pour plus d’informations.

1. Dans Mon Marketo, accédez à **Base de données**.

   ![](assets/db-1.png)

1. Cliquez sur **New** et sélectionnez **Importer les données d’objet personnalisé**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Cliquez sur **Parcourir** pour localiser le fichier de données. Sélectionnez le format de fichier (valeurs séparées par des virgules dans cet exemple).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Sélectionnez votre objet personnalisé.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Sélectionnez le mode déduplication dans la liste déroulante. Cliquez sur **Suivant**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Utilisez le ou les champs de déduplication comme identifiants uniques lorsque vous créez ou mettez à jour des enregistrements d’objets personnalisés. Cet exemple utilise le champ Dédupe de l&#39;objet personnalisé **car** - numéro d&#39;identification du véhicule. Si vous mettez uniquement à jour des enregistrements d’objets personnalisés, vous pouvez sélectionner le Guide marketing comme mode de déduplication.

1. Faites correspondre chaque colonne à un champ Marqué, en la sélectionnant dans la liste déroulante.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Assurez-vous que les valeurs de votre fichier correspondent au type de champ auquel vous faites correspondre (par exemple, texte, entier, etc.), sinon le fichier sera rejeté.

1. Cliquez sur **Suivant**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Cliquez sur **Importer**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >La taille maximale des objets personnalisés est de 100 Mo.

   >[!TIP]
   >
   >Entrez votre adresse de courriel dans le champ **Envoyer l&#39;alerte à :** et Marketo vous enverra un courriel une fois votre importation terminée !

1. Dans le coin supérieur droit de l’écran, une notification s’affiche pendant l’exécution de l’importation et les résultats finaux une fois l’importation terminée.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Ouais !

>[!MORELIKETHIS]
>
>* [Compréhension des objets personnalisés de marketing](understanding-marketo-custom-objects.md)

>



