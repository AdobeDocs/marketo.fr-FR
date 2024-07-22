---
unique-page-id: 2359675
description: Désactiver le préremplissage d’un champ de formulaire - Documents Marketo - Documentation du produit
title: Désactiver le préremplissage d’un champ de formulaire
exl-id: c600e0ce-1b94-4f7b-b75d-f550a2904799
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# Désactiver le préremplissage d’un champ de formulaire {#disable-pre-fill-for-a-form-field}

Lorsqu’un visiteur web est connu (cookie), les formulaires Marketo préremplissent les champs avec leurs informations par défaut. Si vous voulez l&#39;éteindre, voici comment le faire.

>[!NOTE]
>
>**Form Pre-fill** est activé par défaut. Les paramètres de préremplissage au niveau de la page d’entrée et les paramètres de préremplissage au niveau de l’administrateur sont prioritaires sur le paramètre au niveau du formulaire :
>
>Formulaire > Landing Page > Admin

## Comment désactiver le préremplissage {#how-to-disable-pre-fill}

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities-7.png)

1. Sélectionnez votre formulaire et cliquez sur **Modifier le formulaire**.

   ![](assets/image2014-9-15-14-3a26-3a46.png)

   >[!CAUTION]
   >
   >Le préremplissage de formulaire ne fonctionne pas lors de l’incorporation d’un formulaire sur vos propres pages. Il ne fonctionne que sur les landing pages Marketo.

1. Sélectionnez l’un des champs et définissez **Form Pre-fill** sur **Disabled**.

   ![](assets/image2014-9-15-14-3a26-3a54.png)

   >[!TIP]
   >
   >Vous pouvez également désactiver le préremplissage de formulaire au niveau de la landing page ou au niveau de l’administrateur.

1. Cliquez sur **Terminer**.

   ![](assets/image2014-9-15-14-3a27-3a1.png)

1. Cliquez sur **Approuver et fermer**.

   ![](assets/image2014-9-15-14-3a27-3a6.png)

## Champs sensibles {#sensitive-fields}

Lorsque vous [marquez un champ comme sensible](/help/marketo/product-docs/administration/field-management/mark-a-field-as-sensitive.md), empêchant ses valeurs d’être préremplies dans les formulaires, l’option Préremplir s’affiche.

![](assets/disable-pre-fill.png)