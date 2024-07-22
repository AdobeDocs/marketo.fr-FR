---
unique-page-id: 11383953
description: Configuration des conversions hors ligne Facebook - Documents Marketo - Documentation du produit
title: Configuration des conversions hors ligne de Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 2%

---

# Configuration des conversions hors ligne de Facebook {#set-up-facebook-offline-conversions}

En renvoyant les données de conversion hors ligne à Facebook pour les personnes créées par le biais de pistes publicitaires, votre équipe publicitaire peut optimiser les dépenses publicitaires de manière plus optimale que jamais. Voici comment le mettre en place.

>[!PREREQUISITES]
>
>* Vous devez [configurer Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* Vous devez disposer d’un modèle approuvé dans [Revenue Cycle Modeler](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

## Configuration de l’administrateur {#admin-configuration}

1. Accédez à Marketo **Admin**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Accédez à **LaunchPoint** et double-cliquez sur le service Facebook Lead Ads que vous avez créé précédemment.

   >[!NOTE]
   >
   >Si vous n’avez pas fait cela, allez-y et [Configurez Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md), puis revenez ici.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Si vous le souhaitez, modifiez le **nom d’affichage** afin d’inclure les conversions hors ligne. Cliquez sur **Suivant**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Cochez **Activer les conversions hors ligne** et cliquez sur **Suivant**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Cliquez sur **Suivant**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Doux ! Vous avez terminé à mi-chemin d’activer les conversions hors ligne de Facebook. Passez à la Modeler du cycle de revenu pour mapper les scènes.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configuration de Recettes Cycle Modeler {#revenue-cycle-modeler-configuration}

1. Accédez à **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Sélectionnez votre modèle et cliquez sur **Modifier le brouillon**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Actuellement, il existe 10 événements Facebook que vous pouvez mettre en correspondance des étapes du cycle du chiffre d’affaires avec :
   >
   >* Ajout d’informations de paiement
   >* Ajouts au panier
   >* Ajoute à la liste des souhaits
   >* Inscriptions terminées
   >* Passages en caisse commencés
   >* Individu
   >* Autres
   >* Achat
   >* Recherches
   >* Affichage de contenu

1. Sélectionnez l’étape à mapper, puis, dans la liste déroulante **Conversion Facebook**, sélectionnez l’événement Facebook auquel vous souhaitez le mapper. Répétez cette étape pour mapper toutes les étapes de votre CRM aux étapes de conversion hors ligne sur Facebook.

   ![](assets/1-1.png)

1. Une fois le mappage terminé, fermez le modèle.

   ![](assets/2.png)

1. Approuvez votre modèle et vous avez terminé !

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Désormais, lorsque les pistes publicitaires de piste atteignent les étapes que vous avez mappées, les conversions sont envoyées à Facebook pour la création de rapports.

   >[!CAUTION]
   >
   >Vérifiez votre compte Facebook et assurez-vous que toutes les [publicités sont associées](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) au jeu d’événements de conversion hors ligne Marketo. Si ce n’est pas le cas, l’attribution des publicités peut ne pas fonctionner.

   >[!NOTE]
   >
   >Les données de conversion hors ligne sont envoyées de Marketo à Facebook plusieurs fois par jour.

>[!MORELIKETHIS]
>
>[Comprendre les conversions hors ligne de Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
