---
unique-page-id: 2359947
description: Transition Personnes entre les flux d’engagement - Documents Marketo - Documentation du produit
title: Personnes de transition entre les flux d’engagement
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 1%

---

# Personnes de transition entre les flux d’engagement {#transition-people-between-engagement-streams}

Les programmes d’engagement peuvent comporter plusieurs flux. Si vous [ajout d’un flux](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), vous allez définir un moyen pour les gens de passer d’un flux à un autre. Elles sont appelées **règles de transition.**

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Sélectionnez votre programme d’engagement en continu et accédez à **Flux**.

   ![](assets/multistream.jpg)

1. Cliquez sur **Règles de transition** pour le flux que vous souhaitez extraire d’autres flux, puis cliquez sur **Modification des règles de transition**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Les règles de transition s’extraient dans un flux ; définissez toujours les règles sur le flux que vous souhaitez extraire.

   Une fois la fenêtre des règles de transition ouverte, recherchez et faites glisser le déclencheur de votre choix. Dans ce cas, nous voulons déplacer les personnes vers l’état intermédiaire lorsqu’il est ajouté à une opportunité.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Définissons l’opérateur sur **est quelconque** pour que les gens passent à autre chose pour n&#39;importe quelle opportunité.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Vous pouvez ajouter plusieurs déclencheurs et filtres à une règle de transition, mais celle-ci utilise tous les filtres (TOUS les filtres sont la seule option). Si vous devez utiliser OU dans une règle de transition, nous vous recommandons de configurer plutôt une campagne dynamique externe.

1. Cliquez sur **Fermer**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Fantastique ! Désormais, toute personne de votre programme d’engagement ajoutée à une opportunité sera déplacée dans le flux intermédiaire de l’évaluation intermédiaire.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Les étapes décrites ci-dessus *do* s’appliquent aux personnes qui [en pause](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) ainsi que .
