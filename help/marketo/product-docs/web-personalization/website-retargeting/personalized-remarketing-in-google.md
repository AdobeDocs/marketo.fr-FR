---
unique-page-id: 4720810
description: Remarketing personnalisé dans Google - Documents Marketo - Documentation du produit
title: Remarketing personnalisé dans Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Remarketing personnalisé dans Google {#personalized-remarketing-in-google}

Le remarketing personnalisé vous permet de réengager vos utilisateurs à l’aide des données RTP et de la puissance des Google Analytics grâce à la portée du réseau d’affichage Google.

>[!PREREQUISITES]
>
>* Procédez comme suit : [Reciblage à l’aide de données de personnalisation web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) configuration
>* Réviser [Aide sur les remarques avec les Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) documentation.

## Création d’une audience de remarketing dans Google {#creating-a-remarketing-audience-in-google}

1. Connectez-vous à vos Google Analytics. Cliquez sur **Administration**, **Compte**, **Propriété**. Cliquez sur **Définitions d’audience** et **Audiences**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Cliquez sur **+Nouvelle audience**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Configuration des liens**: Lien vers votre compte Google AdWords. **Définition de l’audience**: Cliquez sur **Créer**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Dans Audience Builder, cliquez sur **Séquences** et **Recherche des données RTP** sous Dimensions personnalisées, Variables personnalisées, Événements.

>[!TIP]
>
>Comment trouver les données RTP dans Analytics pour créer votre audience ?
>
>En Google Analytics :
>
>* Variables personnalisées : Organisation, industrie
>* Catégorie d’événements : Segment, Insightera-CTA, RTP-Remarketing
>* Libellé de l’événement : Nom du segment, nom de la campagne, nom de l’audience segmentée
>
>Dans Google Universal Analytics :
>
>* Dimensions personnalisées : Organisation, secteur, catégorie (Fortune 500,1000, Global 2000), groupe (Enterprise, SMB), liste ABM (Liste de comptes nommés)
>* Catégorie d’événements : RTP-Segment, RTP-Campaign-Remarketing
>* Libellé de l’événement : Nom du segment, nom de la campagne, nom de l’audience segmentée

**Exemple d’audience de remarketing à partir de données d’audience segmentées RTP**

1. Cliquez sur **Séquences.**
1. Sélectionner **Libellé de l’événement.**
1. Entrée **Nom de l’audience segmentée** (tel qu’il apparaît dans RTP).
1. Cliquez sur **Appliquer**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exemple d’audience à partir de données du secteur RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Cliquez sur **Séquences**.
1. Sélectionner **RTP-Industry**.
1. Entrée **Nom du secteur industriel** (p. ex. Services financiers, éducation..).
1. Cliquez sur **Appliquer**.
1. Saisissez un **Nom de l’audience**. Cliquez sur **Enregistrer**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Créer une campagne d’annonce de remarketing dans Google AdWords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Connectez-vous à **Google Adwords**. Cliquez sur **Campagnes**, sélectionnez **Afficher le réseau uniquement**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Entrée **Nom de la campagne**, Sélectionner **Saisissez Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Entrée **Nom du groupe publicitaire,** enter **CPC amélioré**, Sélectionner **Liste de remarketing**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Cliquez sur Enregistrer et continuez.
1. Ajoutez votre image ou annonce textuelle et lancez votre campagne de remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Reciblage à l’aide de données de personnalisation web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personnalisé dans Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
