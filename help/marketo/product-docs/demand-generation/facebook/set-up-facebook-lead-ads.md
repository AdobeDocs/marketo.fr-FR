---
unique-page-id: 11379622
description: Configuration des publicités de lead Facebook - Documents Marketo - Documentation du produit
title: Configurer les publicités de lead Facebook
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Configurer les publicités de lead Facebook {#set-up-facebook-lead-ads}

Utilisez [Facebook Lead Ads](https://www.facebook.com/business/ads/ad-objectives/lead-generation){target="_blank"} pour exécuter des campagnes publicitaires sur Facebook et générer des leads pour Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!AVAILABILITY]
>
>Pour ajouter des annonces de leads Facebook à votre instance, contactez l’équipe de compte Adobe (votre gestionnaire de compte).

1. Dans Marketo Engage, accédez à la zone **Admin**.

   ![](assets/set-up-facebook-lead-ads-1.png)

1. Accédez à **LaunchPoint**, cliquez sur le menu déroulant **Nouveau** et sélectionnez **Nouveau service**.

   ![](assets/set-up-facebook-lead-ads-2.png)

1. Saisissez un **[!UICONTROL Nom d’affichage]** pour votre service, sélectionnez le service **[!UICONTROL Publicités de prospect Facebook]** dans la liste déroulante, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/set-up-facebook-lead-ads-3.png)

1. Ouvrez un nouvel onglet dans le même navigateur et accédez à [facebook.com](https://www.facebook.com){target="_blank"}. Connectez-vous à Facebook à l’aide du compte que vous souhaitez utiliser pour l’intégration.

   >[!NOTE]
   >
   >Le compte [!DNL Facebook] devra accéder à toutes les pages professionnelles [!DNL Facebook] à partir desquelles vous souhaitez extraire les publicités de lead.

   ![](assets/set-up-facebook-lead-ads-4.png)

1. Une fois connecté à [!DNL Facebook], revenez à Marketo et cliquez sur **[!UICONTROL Autoriser]**.

   ![](assets/set-up-facebook-lead-ads-5.png)

1. Si vous y êtes invité, cliquez sur **[!UICONTROL OK]** pour accepter l’installation de l’application Marketo dans [!DNL Facebook].

   ![](assets/set-up-facebook-lead-ads-6.png)

1. Vous remarquerez que vous êtes désormais autorisé. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/set-up-facebook-lead-ads-7.png)

1. Sélectionnez la ou les pages sur lesquelles Marketo doit extraire [!UICONTROL publicités de prospect Facebook] et cliquez sur **[!UICONTROL Suivant]**.

   >[!TIP]
   >
   >Si aucune page attendue ne s’affiche, vérifiez que le compte [!DNL Facebook] utilisé pour l’authentification est ajouté à la page le [!DNL Facebook] et réessayez.

   ![](assets/set-up-facebook-lead-ads-8.png)

1. Pour accepter les [!DNL Facebook] par défaut aux mappages de champs Marketo, cliquez simplement sur **[!UICONTROL Créer]**.

   >[!TIP]
   >
   >En modifiant les mappages, vous pouvez personnaliser l’emplacement de stockage des données des annonces de prospects dans Marketo. Vous pouvez également [extraire des données à partir des questions personnalisées des annonces de leads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md){target="_blank"}.

   >[!CAUTION]
   >
   >Marketo ne prend pas en charge le mappage de deux champs [!DNL Facebook] à un seul champ Marketo, uniquement de 1 à 1. Si vous mappez 2 à 1, les prospects peuvent ne pas entrer dans le système Marketo.

   ![](assets/set-up-facebook-lead-ads-9.png)

   Bien joué ! Les leads commenceront à affluer dans Marketo lorsque vous exécuterez avec succès [!DNL Facebook] campagnes publicitaires de leads.

   ![](assets/set-up-facebook-lead-ads-10.png)

>[!MORELIKETHIS]
>
>* [Attribuer/supprimer des autorisations dans le Gestionnaire d’accès des leads (Facebook)](https://www.facebook.com/business/help/540596413257598?id=735435806665862){target="_blank"}
>* [Utilisation des filtres et des triggers des publicités de lead dans une campagne dynamique](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md){target="_blank"}
>* [Mapper des champs personnalisés à Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md){target="_blank"}
