---
unique-page-id: 2359947
description: Découvrez comment configurer des règles de transition pour déplacer des personnes entre les flux d’engagement. Définissez des règles sur le flux que vous souhaitez extraire.
title: Transférer des personnes entre des flux d’engagement
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/viGLYAkvGqF-9K5bhAHWDSOMYaiBuKRe8F2QginuYps
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 6%

---

# Transférer des personnes entre des flux d’engagement {#transition-people-between-engagement-streams}

Les programmes de mobilisation peuvent avoir plusieurs volets. Si vous [ajoutez un flux](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), définissez une manière pour les personnes de passer d’un flux à un autre. Elles sont appelées **règles de transition**.

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/ma.png)

1. Sélectionnez votre programme d’engagement à flux multiples et accédez à **[!UICONTROL Flux]**.

   ![](assets/multistream.jpg)

1. Cliquez sur **[!UICONTROL Règles de transition]** pour le flux que vous souhaitez extraire d’autres flux, puis cliquez sur **[!UICONTROL Modifier les règles de transition]**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Les règles de transition extraient dans un flux ; définissez toujours les règles sur le flux que vous souhaitez extraire.

   Une fois la fenêtre des règles de transition ouverte, recherchez et faites glisser le déclencheur de votre choix. Dans cet exemple, les personnes seront déplacées dans [!UICONTROL Phase intermédiaire] lorsqu’elles seront ajoutées à une opportunité.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Définissez l’opérateur sur **[!UICONTROL est n’importe lequel]** afin que les personnes soient transférées pour toute opportunité ajoutée.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Vous pouvez ajouter plusieurs déclencheurs et filtres à une règle de transition, mais celle-ci utilise tous les filtres (utiliser TOUS les filtres est la seule option). Si vous devez utiliser OU dans une règle de transition, il est recommandé de configurer plutôt une campagne intelligente externe.

1. Cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Désormais, toute personne de votre programme d’engagement ajoutée à une opportunité sera déplacée dans le flux [!UICONTROL Phase intermédiaire].

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Les étapes décrites ci-dessus *do* s’appliquent également aux personnes [en pause](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).
