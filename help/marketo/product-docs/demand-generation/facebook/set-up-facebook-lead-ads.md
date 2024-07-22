---
unique-page-id: 11379622
description: Configuration des publicités Facebook - Documents Marketo - Documentation du produit
title: Configuration de publicités Facebook
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Configuration de publicités Facebook {#set-up-facebook-lead-ads}

Utilisez [Facebook Lead Ads](https://www.facebook.com/business/a/lead-ads) pour exécuter des campagnes publicitaires dans Facebook et générer des pistes pour Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!AVAILABILITY]
>
>Pour que les pistes publicitaires Facebook soient ajoutées à votre instance, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

1. Accédez à Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Accédez à **LaunchPoint**, cliquez sur **Nouveau,** et sélectionnez **Nouveau service**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Saisissez un **nom d’affichage** pour votre service, sélectionnez le service **Facebook Lead Ads** dans la liste déroulante, puis cliquez sur **Créer**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. Ouvrez un nouvel onglet dans le même navigateur et accédez à [facebook.com](https://www.facebook.com). Connectez-vous à Facebook à l’aide du compte que vous souhaitez utiliser pour l’intégration.

   >[!NOTE]
   >
   >Le compte Facebook devra accéder à toutes les pages d’entreprise de Facebook à partir desquelles vous souhaitez extraire des publicités de piste.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Une fois connecté à Facebook, revenez à Marketo et cliquez sur **Autoriser**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. Si vous y êtes invité, cliquez sur **OK** pour accepter l’installation de l’application Marketo dans Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Vous remarquerez que vous êtes maintenant autorisé. Cliquez sur **Suivant**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. Sélectionnez la ou les pages à partir desquelles Marketo doit extraire des publicités Facebook et cliquez sur **Suivant**.

   >[!TIP]
   >
   >Si vous ne voyez pas de page que vous attendez, assurez-vous que le compte Facebook utilisé pour vous authentifier est ajouté à la page sur Facebook et réessayez.

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. Pour accepter les mappages de champ Facebook vers Marketo par défaut, cliquez simplement sur **Créer**.

   >[!TIP]
   >
   >En modifiant les mappages, vous pouvez personnaliser l’emplacement de stockage des données des publicités principales dans Marketo. Vous pouvez également [ extraire des données des questions personnalisées de pistes publicitaires](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo ne prend pas en charge le mappage de deux champs Facebook à un seul champ Marketo, uniquement de 1 à 1. Si vous mappez 2 à 1, il se peut que les prospects ne parviennent pas à entrer dans le système Marketo.

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   C&#39;est joli ! Les pistes commenceront à affluer vers Marketo lorsque vous lancez des campagnes publicitaires de piste Facebook réussies.

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [Attribuer/supprimer des autorisations dans le gestionnaire d’accès Leads (Facebook)](https://www.facebook.com/business/help/540596413257598?id=735435806665862)
>* [Utiliser des filtres et des déclencheurs de piste dans une campagne dynamique](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [Mapper des champs personnalisés à Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)
