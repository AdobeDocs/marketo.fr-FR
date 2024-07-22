---
unique-page-id: 2359947
description: Transition Personnes entre les flux d’engagement - Documents Marketo - Documentation du produit
title: Personnes de transition entre les flux d’engagement
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 1%

---

# Personnes de transition entre les flux d’engagement {#transition-people-between-engagement-streams}

Les programmes d’engagement peuvent comporter plusieurs flux. Si vous [ajoutez un flux](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), vous voudrez définir un moyen pour les personnes de passer d’un flux à un autre. Elles sont appelées **règles de transition.**

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Sélectionnez votre programme d’engagement multi-flux et accédez à **Streams**.

   ![](assets/multistream.jpg)

1. Cliquez sur **Règles de transition** pour le flux que vous souhaitez extraire des autres flux, puis cliquez sur **Modifier les règles de transition**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Les règles de transition s’extraient dans un flux. Définissez toujours les règles du flux dans lequel vous souhaitez les extraire.

   Une fois la fenêtre des règles de transition ouverte, recherchez et faites glisser le déclencheur de votre choix. Dans ce cas, nous voulons déplacer les personnes vers l’état intermédiaire lorsqu’il est ajouté à une opportunité.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Définissons l’opérateur sur **est n’importe quel** afin que les personnes passent au-dessus de toute opportunité supplémentaire.

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
   >Les étapes décrites ci-dessus *do* s’appliquent également aux personnes qui sont [ sur pause](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).
