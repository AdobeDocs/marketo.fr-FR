---
description: Modification des limites de récupération d’objets personnalisés dans un script Velocity - Documents Marketo - Documentation du produit
title: Modification des limites de récupération d’objets personnalisés dans les scripts Velocity
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Modification des limites de récupération d’objets personnalisés dans les scripts Velocity {#change-custom-object-retrieval-limits-in-velocity-scripting}

Si vous utilisez le script Velocity pour afficher des données d’objet personnalisé dans des emails, cette fonctionnalité peut vous être utile. Par défaut, vous êtes autorisé à accéder à 10 objets personnalisés parents à partir du script Velocity. Si vous avez besoin d’accéder à plus d’informations, lisez la suite.

## Présentation de Velocity {#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/) est un langage basé sur Java conçu pour modéliser et scripter le contenu d’un HTML. Marketo permet de l’utiliser dans le contexte des emails via l’utilisation de la fonction [jetons de script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Cela permet notamment d’accéder aux données stockées dans des objets personnalisés.

Vous pouvez référencer des objets personnalisés parents et enfants directement connectés au prospect ou au contact, mais pas des objets personnalisés de troisième niveau. Pour chaque objet personnalisé, les 10 enregistrements les plus récemment mis à jour par personne/contact sont disponibles au moment de l’exécution et sont classés de la mise à jour la plus récente (à 0) à la mise à jour la plus ancienne (à 9).

## Comment modifier la limite {#how-to-change-the-limit}

1. Accédez au **Administration** .

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Cliquez sur **Email**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Dans le tableau Limites de récupération d’objets personnalisés, saisissez une nouvelle Limite de récupération parente, puis cliquez sur **Enregistrer les modifications**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>La valeur de la limite de récupération parente doit être comprise entre 10 et 100. La limite de récupération des enfants est définie automatiquement. Pour ce faire, divisez 1 000 par la limite de récupération parente. Par exemple, si vous définissez la limite Parent sur 50, la limite Enfant devient 20 (1 000 ÷ 50 = 20).

Doux ! Vous pouvez désormais accéder à d’autres objets personnalisés à partir du script Velocity.
