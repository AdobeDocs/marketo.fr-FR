---
unique-page-id: 11370892
description: Découvrez comment tester l’intégration des publicités de lead Facebook sur les ordinateurs de bureau avec Marketo. Vérifiez correctement les envois d’annonces de leads depuis la synchronisation de bureau.
title: Tester les publicités de lead Facebook pour l’intégration de bureau à Marketo
exl-id: 2025b6e9-ecd7-4677-9f76-bc7813884e93
feature: Integrations
TQID: https://experienceleague.adobe.com/I4eS9oQyilDMuEigreugkCgPCKvfCw1uX3zSmKyftN8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 213
ht-degree: 5%

---

# Tester [!DNL Facebook] publicités de lead pour l’intégration des ordinateurs de bureau avec Marketo {#test-facebook-lead-ads-for-desktop-integration-with-marketo}

Après avoir créé votre annonce principale, vous devez la tester. Pour ce faire, procédez comme suit sur votre bureau.

>[!PREREQUISITES]
>
>Vous devez [Configurer l’intégration [!UICONTROL publicités de prospect Facebook]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).

1. Dans Facebook Power Editor, sélectionnez une campagne, une publicité, puis cliquez sur **[!UICONTROL Modifier]**.

1. Sous **[!UICONTROL Liens]**, cliquez sur le lien **[!UICONTROL Afficher dans les flux d’actualités]**.

   ![](assets/image2016-5-13-14-3a35-3a36.png)

1. Vous serez redirigé vers [!DNL Facebook] dans un nouvel onglet de votre navigateur. Cliquez sur le  dans l’unité Publicité du prospect [!DNL Facebook].

   ![](assets/image2016-5-13-14-3a42-3a45.png)

   >[!NOTE]
   >
   >Il s’agit d’un exemple qui utilise un Call to action En savoir plus . Le Call to action de votre lead publicitaire peut être différent.

1. Envoyez votre lead publicitaire de test en remplissant le formulaire sur votre bureau. Cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/image2016-5-13-14-3a47-3a43.png)

1. L’envoi du formulaire d’annonce de prospect est terminé.

   ![](assets/image2016-5-13-14-3a52-3a57.png)

1. Après avoir envoyé votre formulaire, [créez une liste dynamique dans Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) dans le cadre d’un programme ou dans la base de données qui utilise le filtre de formulaire [!DNL Facebook] de publicités de leads rempli. Insérez le nom du formulaire d’annonce de prospect du formulaire que vous avez envoyé.

   ![](assets/image2016-3-11-8-3a59-3a34-1.png)

1. Cliquez maintenant sur l’onglet **[!UICONTROL Personnes]** pour vérifier que la synchronisation fonctionne correctement.

   ![](assets/people.png)

>[!MORELIKETHIS]
>
>[Configuration [!UICONTROL Publicités de leads Facebook]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
