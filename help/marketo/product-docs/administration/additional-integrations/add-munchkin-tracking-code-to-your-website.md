---
unique-page-id: 2360354
description: Ajout du code de suivi Munchkin à votre site web - Documents Marketo - Documentation du produit
title: Ajout du code de suivi Munchkin à votre site web
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
source-git-commit: dbb7478ac7b7e811bb9dfeb7c5e4a80ae400ab9b
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 2%

---

# Ajout du code de suivi Munchkin à votre site web {#add-munchkin-tracking-code-to-your-website}

Le code de suivi JavaScript personnalisé de Marketo, appelé Munchkin, effectue le suivi de tous les visiteurs de votre site web afin que vous puissiez réagir à leurs visites à l’aide de campagnes marketing automatisées. Même les visiteurs anonymes sont suivis avec leurs adresses IP et d’autres informations. **Sans ce code de suivi, vous ne pourrez pas effectuer le suivi des visites ou d’autres activités sur votre site web.**!

>[!PREREQUISITES]
>
>Assurez-vous d’avoir accès à un développeur JavaScript expérimenté. L’assistance technique de Marketo n’est pas configurée pour faciliter le dépannage du code JavaScript personnalisé.

## Ajout du code de suivi à votre site web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Les clients Adobe Experience Cloud peuvent également utiliser l’intégration Marketo dans Adobe Launch pour inclure le script Munchkin sur leurs pages web. Obtention de l’application [here](https://www.adobeexchange.com/experiencecloud.details.101054.html).

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Cliquez sur **Munchkin**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Sélectionnez Asynchrone pour Type de code de suivi.

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

   Pour de meilleurs résultats, utilisez le code Munchkin asynchrone et placez-le dans la variable `<head>` des éléments de vos pages. Si vous utilisez le code simple (non recommandé), il se trouve juste avant l’événement `</body>` balise .

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Pour les sites dont le trafic est important (des centaines de milliers de visites par mois, par exemple), nous vous recommandons de ne pas suivre les personnes anonymes. [En savoir plus](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## Ajout d’un code de suivi lors de l’utilisation de plusieurs espaces de travail {#add-tracking-code-when-using-multiple-workspaces}

Si vous utilisez des espaces de travail dans votre compte Marketo, il est probable que vous ayez également des présences web distinctes qui correspondent à vos espaces de travail. Dans ce cas, vous pouvez utiliser le code JavaScript de suivi de Munchkin pour affecter vos personnes anonymes à l’espace de travail et à la partition appropriés.

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Cliquez sur **Munchkin**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Sélectionnez l’espace de travail approprié pour les pages Web dont vous souhaitez effectuer le suivi.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Si vous n’utilisez pas le code Munchkin de l’espace de travail spécial, les personnes seront affectées à la partition par défaut qui a été créée lors de la configuration de votre compte. Il s’appelle initialement &quot;Par défaut&quot;, mais vous avez peut-être modifié cela dans votre propre compte Marketo.

1. Sélectionner **Asynchrone** pour le type de code de suivi.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Cliquez sur et copiez le code de suivi JavaScript à placer sur votre site web.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >N’utilisez pas le code affiché dans cette capture d’écran. Vous devez utiliser le code unique qui apparaît dans votre compte.

1. Placez le code de suivi sur vos pages web dans la variable `<head>` élément . Les nouvelles personnes qui visitent cette page seront affectées à cette partition.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Vous ne pouvez utiliser qu’un seul script de suivi Munchkin pour une partition unique et un espace de travail sur une page. N’incluez pas de scripts de suivi pour plusieurs partitions/espaces de travail sur votre site web.

   >[!NOTE]
   >
   >Les landing pages créées dans Marketo contiennent automatiquement du code de suivi. Vous n’avez donc pas besoin de placer ce code dessus.

## Types de codes de suivi Munchkin {#types-of-munchkin-tracking-codes}

Vous pouvez choisir trois types de codes de suivi Munchkin. Chacune a un impact différent sur les temps de chargement de la page web.

1. **Simple**: comporte le moins de lignes de code, mais ne s’optimise pas pour le temps de chargement des pages web. Ce code charge la bibliothèque jQuery chaque fois qu’une page web est chargée.
1. **Asynchrone**: réduit le temps de chargement des pages web.
1. **jQuery asynchrone**: réduit le temps de chargement des pages web et améliore également les performances du système. Ce code suppose que vous disposez déjà de jQuery et ne vérifie pas son chargement.

## Test du fonctionnement de votre code Munchkin {#test-if-your-munchkin-code-is-working}

Pour vérifier que votre code Munchkin fonctionne après l’avoir ajouté :

1. Visitez votre page web.

1. Dans votre Marketo, cliquez sur le bouton **Analytics** mosaïque.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Cliquez sur **Activité de page web**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Cliquez sur le bouton **Configuration** onglet, double-clic **Source de l’activité**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Remplacez la source de l’activité par **Visiteurs anonymes (y compris les FAI)** et cliquez sur **Appliquer**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Cliquez sur le bouton **Rapport** .

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Si vous ne voyez aucune donnée, patientez quelques minutes, puis cliquez sur l’icône d’actualisation en bas de la page.
