---
unique-page-id: 2950617
description: Découvrez comment utiliser du contenu dynamique dans un email. Afficher un contenu différent pour différents segments en fonction des règles et des attributs.
title: Utilisation du contenu dynamique dans un e-mail
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
TQID: https://experienceleague.adobe.com/NzTat-p-dgq9wtHv-hyJJzAwud27aOBvVTIS1Tn0lnc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 271
ht-degree: 5%

---

# Utilisation du contenu dynamique dans un e-mail {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Créer une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Utilisez le contenu dynamique dans les e-mails pour envoyer les informations ciblées de vos prospects.

>[!NOTE]
>
>L’utilisation de variables dans le contenu dynamique d’un e-mail n’est prise en charge que lors de l’utilisation de campagnes Trigger. Elle n’est **pas** prise en charge lors de l’utilisation de campagnes par lots.

## Ajouter une segmentation {#add-segmentation}

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/login-marketing-activities.png)

1. Sélectionnez votre e-mail et cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/1.2.png)

1. Dans cet exemple, nous rendons la ligne d&#39;objet dynamique. Cliquez dans le champ [!UICONTROL Objet], puis sur le bouton **Rendre dynamique**.

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Vous pouvez également rendre dynamique un élément dans l’e-mail. Pour ce faire, sélectionnez la zone, cliquez sur l’icône d’engrenage, puis sélectionnez **Rendre dynamique** (ou [Remplacer par un fragment de code](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), selon ce que vous faites).

1. Saisissez le nom de la segmentation, sélectionnez-le, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/1.4.png)

   Votre segmentation et ses segments apparaissent sous l’onglet [!UICONTROL Dynamique] à droite.

   ![](assets/1.5.png)

## Application de contenu dynamique {#apply-dynamic-content}

>[!CAUTION]
>
>Le nombre d’éléments de contenu dynamique autorisés n’est pas illimité. Bien qu’il n’y ait pas de limite de nombre spécifique (elle peut varier en fonction de la combinaison de contenu), la surutilisation de contenu dynamique peut avoir une incidence négative sur les performances de l’e-mail. Nous vous recommandons de maintenir la quantité d’éléments de contenu dynamique utilisés à moins de 20 par e-mail.

1. Cliquez sur vos segments et ajoutez votre ligne d’objet.

![](assets/2.1.png)

1. Répétez l’opération pour chaque segment.

   ![](assets/2.2.png)

>[!TIP]
>
>Créez un e-mail par défaut avant d’appliquer du contenu aux différents segments.

>[!CAUTION]
>
>Les modifications apportées au bloc de contenu de segment par défaut sont appliquées à tous les segments.

Doux ! Vous pouvez désormais envoyer des e-mails flexibles à votre audience cible.

>[!MORELIKETHIS]
>
>* [Prévisualiser un e-mail avec du contenu dynamique](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [Utilisation de contenu dynamique dans une page de destination](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
