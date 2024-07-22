---
unique-page-id: 2950617
description: Utilisation de contenu dynamique dans un courrier électronique - Documents Marketo - Documentation du produit
title: Utilisation de contenu dynamique dans un email
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Utilisation de contenu dynamique dans un email {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Créer une segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Utilisez Contenu dynamique dans les emails pour envoyer les informations ciblées de prospects.

>[!NOTE]
>
>L&#39;utilisation de variables dans le contenu dynamique d&#39;un email n&#39;est prise en charge que lors de l&#39;utilisation des campagnes de déclenchement. Il n’est **pas** pris en charge lors de l’utilisation de campagnes par lots.

## Ajouter une segmentation {#add-segmentation}

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities.png)

1. Sélectionnez votre adresse électronique et cliquez sur **Modifier le brouillon**.

   ![](assets/1.2.png)

1. Dans cet exemple, nous rendons l&#39;objet dynamique. Cliquez dans le champ Objet , puis cliquez sur le bouton **Rendre dynamique** .

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Vous pouvez également créer un élément dans la dynamique de l&#39;email. Pour ce faire, sélectionnez la zone, cliquez sur l’icône d’engrenage, puis sélectionnez **Rendre dynamique** (ou [Remplacer par un extrait de code](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), selon ce que vous faites).

1. Saisissez le nom de la segmentation, sélectionnez-le, puis cliquez sur **Enregistrer**.

   ![](assets/1.4.png)

   Votre segmentation et ses segments apparaissent sous l’onglet Dynamique à droite.

   ![](assets/1.5.png)

## Appliquer du contenu dynamique {#apply-dynamic-content}

>[!CAUTION]
>
>Le nombre d’éléments de contenu dynamique autorisé est illimité. Bien qu’il n’existe aucune limite de nombre spécifique (elle peut varier en fonction de la combinaison de contenu), l’utilisation excessive de contenu dynamique peut avoir une incidence négative sur les performances de l’email. Nous vous recommandons de conserver la quantité d’éléments de contenu dynamique utilisée pour moins de 20 par email.

1. Cliquez sur vos segments et ajoutez votre objet.

![](assets/2.1.png)

1. Répétez l’opération pour chaque segment.

   ![](assets/2.2.png)

>[!TIP]
>
>Créez un email par défaut avant d&#39;appliquer le contenu aux différents segments.

>[!CAUTION]
>
>Les modifications apportées au bloc de contenu Segment par défaut sont appliquées à tous les segments.

Doux ! Vous pouvez désormais envoyer des emails flexibles à votre audience cible.

>[!MORELIKETHIS]
>
>* [Aperçu d’un email avec du contenu dynamique](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [Utiliser du contenu dynamique dans une page d’entrée](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
