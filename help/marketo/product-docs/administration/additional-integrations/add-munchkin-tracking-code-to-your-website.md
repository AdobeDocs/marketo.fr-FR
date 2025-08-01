---
unique-page-id: 2360354
description: Ajout  [!DNL Munchkin]  code de suivi à votre site web - Documents Marketo - Documentation du produit
title: Ajout  [!DNL Munchkin]  code de suivi à votre site web
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Ajout [!DNL Munchkin] code de suivi à votre site web {#add-munchkin-tracking-code-to-your-website}

Le code de suivi JavaScript personnalisé de Marketo, appelé [!DNL Munchkin], permet de suivre toutes les personnes qui visitent votre site web afin que vous puissiez réagir à leurs visites à l’aide de campagnes marketing automatisées. Même les visiteurs anonymes sont suivis avec leurs adresses IP et d’autres informations. **Sans ce code de suivi, vous ne pourrez pas suivre les visites ou toute autre activité sur votre site Web** !

>[!PREREQUISITES]
>
>Assurez-vous d’avoir accès à un développeur JavaScript expérimenté. L’assistance technique de Marketo n’est pas configurée pour vous aider à résoudre les problèmes liés au JavaScript personnalisé.

## Ajout d’un code de suivi à votre site web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Les utilisateurs de Adobe Experience Cloud peuvent également utiliser l’intégration [Marketo dans Adobe Launch](https://exchange.adobe.com/apps/ec/100223/adobe-launch-core-extension){target="_blank"} pour inclure [!DNL Munchkin] script sur leurs pages web. Si vous utilisez Adobe Launch, _le script [!DNL Munchkin] est ajouté automatiquement_ vous n’avez donc pas besoin de l’ajouter vous-même.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Cliquez sur **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Sélectionnez **[!UICONTROL Asynchrone]** pour **[!UICONTROL Type de code de suivi]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >Dans la plupart des cas, vous devez utiliser le code asynchrone. [En savoir plus](#types-of-munchkin-tracking-codes).

1. Cliquez sur le code de suivi JavaScript à placer sur votre site web, puis copiez-le.

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >N’utilisez pas le code affiché dans cette capture d’écran. Vous devez utiliser le code unique qui apparaît dans votre compte.

   >[!TIP]
   >
   >Placez le code de suivi sur les pages web que vous souhaitez suivre. Il peut s’agir de chaque page pour les sites de plus petite taille ou uniquement des pages clés des sites comportant de nombreuses pages web générées dynamiquement, de forums d’utilisateurs, etc.

   Pour de meilleurs résultats, utilisez le code [!DNL Munchkin] asynchrone et placez-le dans les éléments `<head>` de vos pages. Si vous utilisez le code simple (déconseillé), il se trouve juste avant la balise `</body>`.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Pour les sites qui enregistrent un volume de trafic élevé (c’est-à-dire des centaines de milliers de visites par mois), nous vous recommandons de ne pas effectuer le suivi des personnes anonymes. [En savoir plus](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking){target="_blank"}.

## Ajout Du Code De Suivi Lors De L’Utilisation De Plusieurs Espaces De Travail {#add-tracking-code-when-using-multiple-workspaces}

Si vous utilisez des espaces de travail dans votre compte Marketo, il est probable que vous disposiez également d’espaces de travail distincts qui correspondent à vos espaces de travail. Dans ce cas, vous pouvez utiliser le JavaScript de suivi [!DNL Munchkin] pour affecter vos personnes anonymes à l’espace de travail et à la partition appropriés.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Cliquez sur **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Sélectionnez l’espace de travail approprié pour les pages web dont vous souhaitez effectuer le suivi.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Si vous n’utilisez pas le code de [!DNL Munchkin] de l’espace de travail spécial, les personnes seront affectées à la partition par défaut créée lors de la configuration de votre compte. Il s’appelle « [!UICONTROL Default] » au départ, mais vous l’avez peut-être modifié dans votre propre compte Marketo.

1. Sélectionnez **[!UICONTROL Asynchrone]** pour **[!UICONTROL Type de code de suivi]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Cliquez sur le code de suivi JavaScript à placer sur votre site web, puis copiez-le.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >N’utilisez pas le code affiché dans cette capture d’écran. Vous devez utiliser le code unique qui apparaît dans votre compte.

1. Placez le code de suivi sur vos pages web dans l’élément `<head>`. Les nouvelles personnes qui visitent cette page seront affectées à cette partition.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Vous ne pouvez utiliser qu’un seul script de suivi [!DNL Munchkin] pour une seule partition et un seul espace de travail sur une page. N’incluez pas de scripts de suivi pour plusieurs partitions/espaces de travail sur votre site web.

   >[!NOTE]
   >
   >Les landing pages créées dans Marketo contiennent automatiquement le code de suivi. Vous n’avez donc pas besoin de placer ce code dessus.

## Types de codes de suivi [!DNL Munchkin] {#types-of-munchkin-tracking-codes}

Vous pouvez choisir trois types de codes de suivi [!DNL Munchkin]. Chacun a un impact différent sur le temps de chargement de la page web.

1. **[!UICONTROL Simple]** : contient le moins de lignes de code, mais ne s’optimise pas pour le temps de chargement des pages web. Ce code charge la bibliothèque jQuery chaque fois qu’une page web est chargée.
1. **[!UICONTROL Asynchrone]** : réduit le temps de chargement des pages web.
1. **[!UICONTROL Requête jQuery asynchrone]** : réduit le temps de chargement des pages web et améliore également les performances du système. Ce code suppose que vous disposez déjà de jQuery et ne vérifie pas pour le charger.

## Tester si votre code [!DNL Munchkin] fonctionne {#test-if-your-munchkin-code-is-working}

Pour vérifier que votre code [!DNL Munchkin] fonctionne après l’avoir ajouté :

1. Visitez votre page web.

1. Dans votre [!DNL My Marketo], cliquez sur la mosaïque **[!UICONTROL Analytics]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Cliquez sur **[!UICONTROL Activité de la page web]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Cliquez sur l’onglet **[!UICONTROL Configuration]**, double-cliquez sur **[!UICONTROL Source d’activité]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Remplacez [!UICONTROL Source d’activité] par **[!UICONTROL Visiteurs anonymes (y compris les FAI)]** puis cliquez sur **[!UICONTROL Appliquer]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Cliquez sur l’onglet **[!UICONTROL Rapport]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Si vous ne voyez aucune donnée, patientez quelques minutes, puis cliquez sur l’icône [!UICONTROL actualiser] en bas.
