---
unique-page-id: 11378713
description: Déclenchement Des Modifications D’Objet Personnalisées - Documents Marketo - Documentation Du Produit
title: Déclenchement Des Modifications D’Objet Personnalisé
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
source-git-commit: acaf2b421ed65f74bedf18b121ce54e30c19c721
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Déclenchement Des Modifications D’Objet Personnalisé {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement :
>
>* Pour une utilisation uniquement avec des objets personnalisés Marketo, pas avec des objets personnalisés synchronisés via l’intégration native [!DNL Salesforce] ou [!DNL Microsoft Dynamics]
>* Comme déclencheur, pas comme filtre
>
>Contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) pour activer les déclencheurs de modification d’objet personnalisé.

Dans la liste dynamique d’une campagne dynamique, vous pouvez déclencher une action de flux lorsqu’un objet personnalisé est ajouté à une personne ou à une entreprise. Vous pouvez également créer une liste dynamique qui utilise un _changement_ dans un objet personnalisé comme déclencheur. Par exemple, utilisez-le pour envoyer un email lorsqu’un nom de cours est mis à jour.

>[!NOTE]
>
>Une entrée de journal d’activité n’est pas créée lorsqu’un enregistrement d’objet personnalisé est modifié.

1. En Marketo Engage, accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Créez ou ouvrez une campagne dynamique existante, puis sélectionnez la liste dynamique.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Recherchez le déclencheur dont vous avez besoin et faites-le glisser sur la zone de travail.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Sélectionnez l’ [!UICONTROL attribut déclencheur].

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Vous pouvez éventuellement définir une contrainte.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. Et voilà. La modification est enregistrée automatiquement.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Compréhension des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
