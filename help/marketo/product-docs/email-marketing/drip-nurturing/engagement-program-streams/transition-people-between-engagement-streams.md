---
unique-page-id: 2359947
description: Transition des personnes entre les flux d’engagement - Documents marketing - Documentation du produit
title: Transition des personnes entre les flux d’engagement
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# Transitions entre les flux d’engagement {#transition-people-between-engagement-streams}

Les programmes d’engagement peuvent comporter plusieurs flux. Si vous [ajoutez un flux](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), vous voudrez définir un moyen pour les personnes de passer d’un flux à un autre. Elles sont appelées **règles de transition.**

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Sélectionnez votre programme d’engagement multi-flux et accédez à **Flux**.

   ![](assets/multistream.jpg)

1. Cliquez sur **Règles de Transition** pour le flux que vous souhaitez extraire des autres flux, puis sur **Modifier les règles de Transition**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >les règles de transition s&#39;insèrent dans un cours d&#39;eau ; toujours définir les règles sur le flux que vous souhaitez intégrer.

   Une fois la fenêtre de la règle de transition ouverte, recherchez et faites glisser le déclencheur de votre choix. Dans ce cas, nous voulons amener les gens à mi-chemin quand il est ajouté à une opportunité.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Définissons l&#39;opérateur sur **est n&#39;importe quel** afin que les personnes passent à l&#39;autre pour toute opportunité ajoutée.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Vous pouvez ajouter plusieurs déclencheurs et filtres à une règle de transition, mais la règle de transition utilise tous les filtres (l’utilisation de TOUS les filtres est la seule option). Si vous devez utiliser OU dans une règle de transition, nous vous recommandons de configurer une campagne dynamique externe à la place.

1. Cliquez sur **Fermer**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Super ! Désormais, toute personne de votre programme d’engagement qui est ajoutée à une opportunité sera déplacée dans le flux Mid Stage.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Les étapes décrites ci-dessus *do* s&#39;appliquent également aux personnes [en pause](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md).
