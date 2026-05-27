---
unique-page-id: 2359675
description: Découvrez comment désactiver le préremplissage d’un champ de formulaire dans Marketo. Empêchez les données de visiteur connues de remplir automatiquement le champ.
title: Désactiver le préremplissage d’un champ de formulaire
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
feature: Forms
TQID: https://experienceleague.adobe.com/loH0b6d25kDL0dReI7lU62IFyXGr3p8tygqwTPx-OVk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 192
ht-degree: 10%

---

# Désactiver le préremplissage d’un champ de formulaire {#disable-pre-fill-for-a-form-field}

Lorsqu’un visiteur web est connu (cookie), les formulaires Marketo préremplissent les champs avec leurs informations par défaut. Si vous souhaitez désactiver cette option, voici comment procéder.

>[!NOTE]
>
>Le **préremplissage de formulaire** est activé par défaut. Les paramètres de préremplissage au niveau de la page de destination et au niveau de l’administrateur remplacent le paramètre de niveau du formulaire :
>
>Formulaire > Page De Destination > Administrateur

## Comment désactiver le préremplissage {#how-to-disable-pre-fill}

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/login-marketing-activities-7.png)

1. Sélectionnez votre formulaire et cliquez sur **[!UICONTROL Modifier le formulaire]**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >Le préremplissage de formulaire ne fonctionne pas lors de l’incorporation d’un formulaire sur vos propres pages. Cela ne fonctionne que sur les pages de destination de Marketo.

1. Sélectionnez l’un des champs et définissez **[!UICONTROL Préremplissage de formulaire]** sur **[!UICONTROL Désactivé]**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >Vous pouvez également désactiver le préremplissage du formulaire au niveau de la page de destination ou au niveau administrateur.

1. Cliquez sur **[!UICONTROL Terminer]**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. Cliquez sur **[!UICONTROL Approuver et fermer]**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## Champs Sensibles {#sensitive-fields}

Lorsque vous [marquez un champ comme sensible](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md), ce qui empêche ses valeurs d’être préremplies dans les formulaires, cela s’affiche sur l’option de préremplissage.

![](assets/disable-pre-fill.png)
