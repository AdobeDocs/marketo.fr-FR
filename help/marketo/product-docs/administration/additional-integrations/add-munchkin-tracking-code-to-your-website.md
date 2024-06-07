---
unique-page-id: 2360354
description: "Ajouter [!DNL Munchkin] Code de suivi sur votre site web - Documents Marketo - Documentation du produit"
title: "Ajouter [!DNL Munchkin] Code de suivi sur votre site web"
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Ajouter [!DNL Munchkin] Code de suivi sur votre site web {#add-munchkin-tracking-code-to-your-website}

Marketo un code de suivi JavaScript personnalisé, appelé [!DNL Munchkin], effectue le suivi de toutes les personnes qui visitent votre site web afin que vous puissiez réagir à leurs visites à l’aide de campagnes marketing automatisées. Même les visiteurs anonymes sont suivis avec leurs adresses IP et d’autres informations. **Sans ce code de suivi, vous ne pourrez pas effectuer le suivi des visites ou d’autres activités sur votre site web.**!

>[!PREREQUISITES]
>
>Assurez-vous d’avoir accès à un développeur JavaScript expérimenté. L’assistance technique de Marketo n’est pas configurée pour faciliter le dépannage du code JavaScript personnalisé.

## Ajout du code de suivi à votre site web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Les utilisateurs de Adobe Experience Cloud peuvent également utiliser la variable [Intégration de Marketo dans Adobe Launch](https://exchange.adobe.com/apps/ec/100223/adobe-launch-core-extension){target="_blank"} à inclure [!DNL Munchkin] script sur leurs pages web. Si vous utilisez Adobe Launch, _la valeur [!DNL Munchkin] Le script est automatiquement ajouté_, vous n’avez donc pas besoin de l’ajouter vous-même.

1. Accédez au **[!UICONTROL Administration]** zone.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Cliquez sur **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Sélectionner **[!UICONTROL Asynchrone]** pour **[!UICONTROL Type de code de suivi]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >Dans la plupart des cas, vous devez utiliser le code asynchrone. [En savoir plus](#types-of-munchkin-tracking-codes).

1. Cliquez sur et copiez le code de suivi JavaScript à placer sur votre site web.

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >N’utilisez pas le code affiché dans cette capture d’écran. Vous devez utiliser le code unique qui apparaît dans votre compte.

   >[!TIP]
   >
   >Placez le code de suivi sur les pages Web dont vous souhaitez effectuer le suivi. Il peut s’agir de toutes les pages des petits sites ou uniquement des pages clés des sites qui comportent de nombreuses pages Web générées dynamiquement, des forums d’utilisateurs, etc.

   Pour de meilleurs résultats, utilisez le mode asynchrone [!DNL Munchkin] et placez-le dans la balise `<head>` des éléments de vos pages. Si vous utilisez le code simple (non recommandé), il se trouve juste avant l’événement `</body>` balise .

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Pour les sites dont le trafic est important (des centaines de milliers de visites par mois, par exemple), nous vous recommandons de ne pas suivre les personnes anonymes. [En savoir plus](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking/){target="_blank"}.

## Ajout d’un code de suivi lors de l’utilisation de plusieurs espaces de travail {#add-tracking-code-when-using-multiple-workspaces}

Si vous utilisez des espaces de travail dans votre compte Marketo, il est probable que vous ayez également des présences web distinctes qui correspondent à vos espaces de travail. Dans ce cas, vous pouvez utiliser le [!DNL Munchkin] suivi Javascript pour affecter vos personnes anonymes à l’espace de travail et à la partition corrects.

1. Accédez au **[!UICONTROL Administration]** zone.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Cliquez sur **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Sélectionnez l’espace de travail approprié pour les pages Web dont vous souhaitez effectuer le suivi.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Si vous n’utilisez pas l’espace de travail spécial [!DNL Munchkin] , les personnes seront affectées à la partition par défaut qui a été créée lors de la configuration de votre compte. Il s’appelle &quot;&quot;[!UICONTROL Par défaut]&quot; au début, mais vous avez peut-être modifié cela dans votre propre compte Marketo.

1. Sélectionner **[!UICONTROL Asynchrone]** pour **[!UICONTROL Type de code de suivi]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Cliquez sur le code de suivi JavaScript à insérer dans votre site web, puis copiez-le.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >N’utilisez pas le code affiché dans cette capture d’écran. Vous devez utiliser le code unique qui apparaît dans votre compte.

1. Placez le code de suivi sur vos pages web dans la variable `<head>` élément . Les nouvelles personnes qui visitent cette page seront affectées à cette partition.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Vous ne pouvez utiliser qu’un seul [!DNL Munchkin] script de suivi pour une partition unique et un espace de travail sur une page. N’incluez pas de scripts de suivi pour plusieurs partitions/espaces de travail sur votre site web.

   >[!NOTE]
   >
   >Les landing pages créées dans Marketo contiennent automatiquement du code de suivi. Vous n’avez donc pas besoin de placer ce code dessus.

## Types de [!DNL Munchkin] Codes de suivi {#types-of-munchkin-tracking-codes}

Il existe trois types de [!DNL Munchkin] codes de suivi que vous pouvez choisir. Chacune a un impact différent sur les temps de chargement de la page web.

1. **[!UICONTROL Simple]**: contient le moins de lignes de code, mais n’optimise pas le temps de chargement des pages web. Ce code charge la bibliothèque jQuery chaque fois qu’une page web est chargée.
1. **[!UICONTROL Asynchrone]**: réduit le temps de chargement des pages web.
1. **[!UICONTROL jQuery asynchrone]**: réduit le temps de chargement des pages web et améliore également les performances du système. Ce code suppose que vous disposez déjà de jQuery et ne vérifie pas son chargement.

## Testez si votre [!DNL Munchkin] Le code fonctionne {#test-if-your-munchkin-code-is-working}

Pour vérifier que [!DNL Munchkin] fonctionne après l’ajout du code :

1. Visitez votre page web.

1. Dans votre [!DNL My Marketo], cliquez sur le **[!UICONTROL Analytics]** mosaïque.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Cliquez sur **[!UICONTROL Activité de page web]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Cliquez sur le bouton **[!UICONTROL Configuration]** onglet, double-clic **[!UICONTROL Source de l’activité]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Modifiez la variable [!UICONTROL Source de l’activité] to **[!UICONTROL Visiteurs anonymes (y compris les FAI)]** et cliquez sur **[!UICONTROL Appliquer]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Cliquez sur le bouton **[!UICONTROL Rapport]** .

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Si vous ne voyez aucune donnée, patientez quelques minutes, puis cliquez sur l’icône d’actualisation en bas de la page.
