---
unique-page-id: 11383953
description: Configurer les conversions hors ligne Facebook - Documents marketing - Documentation du produit
title: Configurer les conversions hors connexion Facebook
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# Configurer les conversions hors connexion Facebook {#set-up-facebook-offline-conversions}

En renvoyant les données de conversion hors ligne à Facebook pour les personnes créées par le biais des publicités de piste, votre équipe publicitaire peut optimiser ses dépenses publicitaires mieux que jamais. Voici comment le configurer.

>[!PREREQUISITES]
>
>* Vous devez [configurer des publicités de piste Facebook](set-up-facebook-lead-ads.md).
>* Vous devez disposer d&#39;un modèle approuvé dans [Revenus Cycle Modeler](http://docs.marketo.com/display/docs/revenue+cycle+models).

>



## Configuration de l’administrateur {#admin-configuration}

1. Accédez à Marketo **Admin**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Accédez à **LaunchPoint** et doublon-cliquez sur le service Publicités de piste Facebook que vous avez créé précédemment.

   >[!NOTE]
   >
   >Si vous n&#39;avez pas fait cela, allez-y et [Configurez les publicités Facebook ](set-up-facebook-lead-ads.md), puis revenez ici.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Si vous le souhaitez, modifiez le **nom d’affichage** pour inclure les conversions hors ligne. Cliquez sur **Suivant**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Cochez **Activer les conversions hors ligne** et cliquez sur **Suivant**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Cliquez sur **Suivant**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Doux ! Vous avez terminé la moitié du processus d’activation des conversions hors ligne Facebook. Passez à la modélisation du cycle de production pour mapper les étapes.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configuration du module de modélisation de cycle de production {#revenue-cycle-modeler-configuration}

1. Accédez à **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Sélectionnez votre modèle et cliquez sur **Modifier le brouillon**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Actuellement, 10 événements Facebook vous permettent de mettre en correspondance des étapes du cycle de recettes avec :
   >
   >    
   >    
   >    * Ajoutes des informations de paiement
   >    * Ajoutes au panier
   >    * Ajoutes à la Liste des souhaits
   >    * Inscriptions terminées
   >    * Passages en caisse commencés
   >    * Personne
   >    * Autre
   >    * Achat
   >    * Recherches
   >    * Vues de contenu


1. Sélectionnez l’étape à mapper, puis, dans la liste déroulante **Conversion Facebook**, sélectionnez le Événement Facebook vers lequel vous souhaitez mapper. Répétez cette étape pour mapper toutes les étapes de votre RCM aux étapes de conversion hors ligne sur Facebook.

   ![](assets/1-1.png)

1. Une fois le mappage terminé, fermez le modèle.

   ![](assets/2.png)

1. Approuvez votre modèle et vous avez terminé !

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Désormais, lorsque les pistes publicitaires de piste atteignent les étapes que vous avez mises en correspondance, les conversions sont envoyées à Facebook pour rapports.

   >[!CAUTION]
   >
   >Vérifiez votre compte Facebook et assurez-vous que toutes les [publicités sont associées](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) au jeu de Événements Conversions hors ligne du marketing. Si ce n&#39;est pas le cas, l&#39;attribution des publicités peut ne pas fonctionner.

   >[!NOTE]
   >
   >Les données de conversion hors ligne sont envoyées de Marketo à Facebook plusieurs fois par jour.

>[!NOTE]
>
>**Articles connexes**
>
>* [Présentation des conversions hors ligne Facebook](understanding-facebook-offline-conversions.md)

>



