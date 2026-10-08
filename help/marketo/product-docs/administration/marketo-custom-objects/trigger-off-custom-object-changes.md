---
unique-page-id: 11378713
description: 'Utilisation d’un objet personnalisé : ajouter ou modifier des déclencheurs dans une liste dynamique de campagne pour les objets personnalisés Marketo, avec les étapes permettant d’ajouter le déclencheur et de définir des contraintes.'
title: Déclenchement basé sur les modifications d’objets personnalisés
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
TQID: 'https://experienceleague.adobe.com/KjZuM-gPLIFa1umPF4pzN2OTak51i9I5TUcC7SacmZ8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: ea4e3ff5-e7b9-4b4c-a5a0-dc27cc3f4275
    internal-label: Custom objects
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 8%
---
# Déclenchement basé sur les modifications d’objets personnalisés {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement :
>
>* À utiliser uniquement avec des objets personnalisés Marketo, et non avec des objets personnalisés synchronisés par le biais de l’intégration native [!DNL Salesforce] ou [!DNL Microsoft Dynamics]
>
>* Comme déclencheur, pas comme filtre
>
>Contactez l’assistance Marketo [](https://nation.marketo.com/t5/Support/ct-p/Support) pour activer les déclencheurs de changement d’objet personnalisé.

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

1. La modification est automatiquement enregistrée.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Présentation des objets personnalisés Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
