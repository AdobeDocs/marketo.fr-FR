---
unique-page-id: 2359663
description: Définir une valeur de champ de formulaire masqué - Documents Marketo - Documentation du produit
title: Définir une valeur de champ de formulaire masquée
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 7%

---

# Définir une valeur de champ de formulaire masquée {#set-a-hidden-form-field-value}

Les champs masqués sont généralement renseignés dynamiquement. Elles ne sont pas présentées à la personne qui remplit le formulaire. Voici comment définir la valeur.

>[!PREREQUISITES]
>
>[Définir un champ de formulaire comme masqué](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Sélectionner le champ {#select-the-field}

1. Dans votre formulaire, sélectionnez le champ masqué et cliquez sur **[!UICONTROL Modifier]** pour **[!UICONTROL Remplissage automatique]**.

   ![](assets/autofill.png)

## Utiliser la valeur par défaut : {#use-default-value}

En sélectionnant Utiliser **[!UICONTROL valeur par défaut]** vous pouvez coder en dur une valeur spécifique qui sera toujours utilisée lors de l’envoi de ce formulaire. Saisissez la **[!UICONTROL Valeur par défaut]** puis cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL Parameter {#url-parameter}

Si vous souhaitez capturer les paramètres d’URL (chaînes de requête) à partir de la page sur laquelle la personne se trouve lors du remplissage du formulaire, vous pouvez utiliser **[!UICONTROL paramètres d’URL]** pour remplir votre champ masqué.

>[!NOTE]
>
>Les paramètres sont un peu techniques, non ? Une fois qu&#39;on les a, ils sont puissants. Cette page [Wikipedia sur les chaînes de requête](https://en.wikipedia.org/wiki/Query_string) est quelque peu utile.

1. Sélectionnez **[!UICONTROL Paramètre d’URL]** pour **[!UICONTROL Obtenir le type de valeur]**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Saisissez le **[!UICONTROL Nom du paramètre]** et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Vous pouvez saisir une **[!UICONTROL Valeur par défaut]** au cas où le paramètre d’URL serait introuvable.

## Valeur du cookie {#cookie-value}

Si vous stockez des données dans des cookies, vous pouvez utiliser **[!UICONTROL Valeur du cookie]** pour récupérer les données lors de l’envoi du formulaire.

1. Sélectionnez **[!UICONTROL Valeur du cookie]** pour **[!UICONTROL Obtenir la valeur de]**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Saisissez le cookie **[!UICONTROL Nom du paramètre]** souhaité, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Vous pouvez saisir une **[!UICONTROL Valeur par défaut]** au cas où le paramètre/cookie est introuvable.

## Paramètre référent {#referrer-parameter}

Si vous souhaitez capturer les données de la page d’où provient le visiteur avant de remplir le formulaire, vous pouvez utiliser **[!UICONTROL Paramètre référent]**.

1. Définissez **[!UICONTROL Obtenir la valeur de]** sur **[!UICONTROL Paramètre de référent]**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Saisissez le **[!UICONTROL Nom du paramètre]** à extraire de l’URL du référent et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Vous pouvez saisir une **[!UICONTROL Valeur par défaut]** au cas où le paramètre référent serait introuvable.

1. Cliquez sur **[!UICONTROL Terminer]**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Cliquez sur **[!UICONTROL Approuver et fermer]**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
