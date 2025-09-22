---
unique-page-id: 2359947
description: Transition Des Personnes Entre Les Flux D’Engagement - Documents Marketo - Documentation Du Produit
title: Transférer des personnes entre des flux d’engagement
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 5%

---

# Transférer des personnes entre des flux d’engagement {#transition-people-between-engagement-streams}

Les programmes de mobilisation peuvent avoir plusieurs volets. Si vous [ajoutez un flux](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), vous voudrez définir une façon pour les gens de passer d&#39;un flux à un autre. Elles sont appelées **règles de transition**.

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/ma.png)

1. Sélectionnez votre programme d’engagement à flux multiples et accédez à **[!UICONTROL Flux]**.

   ![](assets/multistream.jpg)

1. Cliquez sur **[!UICONTROL Règles de transition]** pour le flux que vous souhaitez extraire d’autres flux, puis cliquez sur **[!UICONTROL Modifier les règles de transition]**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Les règles de transition extraient dans un flux ; définissez toujours les règles sur le flux que vous souhaitez extraire.

   Une fois la fenêtre des règles de transition ouverte, recherchez et faites glisser le déclencheur de votre choix. Dans ce cas, nous voulons faire passer les utilisateurs dans [!UICONTROL Mid Stage] lorsqu’il est ajouté à une opportunité.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Définissons l’opérateur sur **[!UICONTROL est n’importe lequel]** afin que les personnes puissent se déplacer pour toute opportunité supplémentaire.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Vous pouvez ajouter plusieurs déclencheurs et filtres à une règle de transition, mais celle-ci utilise tous les filtres (utiliser TOUS les filtres est la seule option). Si vous devez utiliser OU dans une règle de transition, nous vous recommandons de configurer plutôt une campagne intelligente externe.

1. Cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Fantastique ! Désormais, toute personne de votre programme d’engagement ajoutée à une opportunité sera déplacée dans le flux [!UICONTROL Phase intermédiaire].

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Les étapes décrites ci-dessus *do* s’appliquent également aux personnes [en pause](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).
