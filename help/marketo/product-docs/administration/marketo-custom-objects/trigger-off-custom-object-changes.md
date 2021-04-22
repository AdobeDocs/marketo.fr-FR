---
unique-page-id: 11378713
description: Déclencheur des modifications d’objets personnalisés - Documents Marketo - Documentation du produit
title: Déclencher les modifications d’objet personnalisé
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Déclencher les modifications d&#39;objet personnalisé {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement :
>
>* Pour les clients de l&#39;infrastructure Orion
>* Pour une utilisation uniquement avec des objets personnalisés Marketo, et non avec des objets personnalisés synchronisés via l&#39;intégration native Salesforce ou Microsoft Dynamics
>* Comme déclencheur, pas comme filtre

>
>
Pour activer les déclencheurs de modification d&#39;objet personnalisé, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

Dans la liste intelligente d’une campagne dynamique, vous pouvez déclencher une action d’enchaînement lorsqu’un objet personnalisé est ajouté à une personne ou à une société. Vous pouvez également créer une liste dynamique qui utilise comme déclencheur *change* dans un objet personnalisé. Par exemple, utilisez-la pour envoyer un courriel lorsqu’un nom de cours est mis à jour.

>[!NOTE]
>
>Aucune entrée de journal d&#39;activité n&#39;est créée lorsqu&#39;un enregistrement d&#39;objet personnalisé est modifié.

1. Dans Marketo, accédez à **Activités marketing.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Créez ou ouvrez une Campaign dynamique existante, puis sélectionnez la Liste dynamique.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Recherchez le déclencheur dont vous avez besoin et faites-le glisser sur la trame.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Sélectionnez l’attribut de déclenchement.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Vous pouvez éventuellement définir une contrainte.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. Et vous voilà. La modification est enregistrée automatiquement.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [Création d’une Liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

