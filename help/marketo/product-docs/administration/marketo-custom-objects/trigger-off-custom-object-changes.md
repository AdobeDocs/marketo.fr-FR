---
unique-page-id: 11378713
description: Déclenchement Des Modifications D’Objet Personnalisées - Documents Marketo - Documentation Du Produit
title: Déclenchement Des Modifications D’Objet Personnalisé
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Déclenchement Des Modifications D’Objet Personnalisé {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement :
>
>* Pour les clients de l’infrastructure Orion
>* À utiliser uniquement avec des objets personnalisés Marketo, et non avec des objets personnalisés synchronisés via l’intégration Salesforce ou Microsoft Dynamics native
>* Comme déclencheur, pas comme filtre
>
>Veuillez contacter [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) pour activer les déclencheurs de modification d’objet personnalisés.

Dans la liste dynamique d’une campagne dynamique, vous pouvez déclencher une action de flux lorsqu’un objet personnalisé est ajouté à une personne ou à une entreprise. Vous pouvez également créer une liste dynamique qui utilise une *change* dans un objet personnalisé comme déclencheur. Par exemple, utilisez-le pour envoyer un email lorsqu’un nom de cours est mis à jour.

>[!NOTE]
>
>Une entrée de journal d’activité n’est pas créée lorsqu’un enregistrement d’objet personnalisé est modifié.

1. Dans Marketo, accédez à **Activités marketing.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Créez ou ouvrez une campagne dynamique existante, puis sélectionnez la liste dynamique.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Recherchez le déclencheur dont vous avez besoin et faites-le glisser sur la zone de travail.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Sélectionnez l’attribut trigger.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Vous pouvez éventuellement définir une contrainte.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. Et voilà. La modification est enregistrée automatiquement.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [Création d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

