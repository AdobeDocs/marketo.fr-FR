---
description: Modifier les limites de récupération d'objets personnalisés dans les scripts Velocity - Marketo Docs - Documentation du produit
title: Modifier les limites de récupération d’objets personnalisés dans les scripts Velocity
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Modifier les limites de récupération d&#39;objets personnalisés dans les scripts Velocity {#change-custom-object-retrieval-limits-in-velocity-scripting}

Si vous utilisez le script Velocity pour afficher des données d’objet personnalisé dans des courriers électroniques, cette fonction peut être adaptée à vos besoins. Par défaut, vous pouvez accéder à 10 objets personnalisés parents à partir du script Velocity. Si vous avez besoin d&#39;accéder à plus d&#39;informations, lisez la suite.

## Qu&#39;est-ce que Velocity {#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/) est un langage basé sur Java conçu pour modéliser et écrire du contenu HTML. Marketo permet de l’utiliser dans le contexte des courriels à l’aide de [jetons de script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Cela permet, entre autres, d’accéder aux données stockées dans des objets personnalisés.

Vous pouvez référencer des objets personnalisés parents et enfants directement connectés au prospect ou contact, mais pas des objets personnalisés de troisième niveau. Pour chaque objet personnalisé, les 10 enregistrements les plus récemment mis à jour par personne/contact sont disponibles au moment de l’exécution et sont commandés de la dernière mise à jour (à 0) à la plus ancienne mise à jour (à 9).

## Comment modifier la limite {#how-to-change-the-limit}

1. Accédez à la section **Admin**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Cliquez sur **Courriel**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Dans le tableau Limites de récupération d’objets personnalisés, entrez une nouvelle limite de récupération parente et cliquez sur **Enregistrer les modifications**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>La valeur limite de récupération parent doit être comprise entre 10 et 100. La limite de récupération de l’enfant est automatiquement définie. Pour ce faire, il divise 1000 par la limite de récupération parente. Par exemple, si vous définissez la limite Parent sur 50, la limite Enfant devient 20 (1 000 × 50 = 20).

Doux ! Vous pouvez désormais accéder à davantage d’objets personnalisés à partir du script Velocity.
