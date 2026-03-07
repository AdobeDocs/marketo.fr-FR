---
unique-page-id: 11378713
description: 'Utilisation d’un objet personnalisé : ajouter ou modifier des déclencheurs dans une liste dynamique de campagne pour les objets personnalisés Marketo, avec les étapes permettant d’ajouter le déclencheur et de définir des contraintes.'
title: Déclencher des modifications d’objet personnalisé
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 5%

---

# Déclencher des modifications d’objet personnalisé {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement :
>
>* À utiliser uniquement avec des objets personnalisés Marketo, et non avec des objets personnalisés synchronisés par le biais de l’intégration native [!DNL Salesforce] ou [!DNL Microsoft Dynamics]
>* Comme déclencheur, pas comme filtre
>
>Contactez le support technique de [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) pour activer les déclencheurs de changement d&#39;objet personnalisé.

Dans la liste dynamique d’une campagne dynamique, vous pouvez déclencher une action de flux lorsqu’un objet personnalisé est ajouté à une personne ou à une entreprise. Vous pouvez également créer une liste dynamique qui utilise une _modification_ dans un objet personnalisé comme déclencheur. Par exemple, utilisez-le pour envoyer un e-mail lorsqu’un nom de cours est mis à jour.

>[!NOTE]
>
>Une entrée de journal d’activité n’est pas créée lorsqu’un enregistrement d’objet personnalisé est modifié.

1. Dans Marketo Engage, accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Créez ou ouvrez une campagne dynamique existante, puis sélectionnez la liste dynamique.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Recherchez le déclencheur dont vous avez besoin et faites-le glisser sur la zone de travail.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Sélectionnez l’attribut [!UICONTROL trigger].

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Vous pouvez éventuellement définir une contrainte.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. Et voilà. La modification est automatiquement enregistrée.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
