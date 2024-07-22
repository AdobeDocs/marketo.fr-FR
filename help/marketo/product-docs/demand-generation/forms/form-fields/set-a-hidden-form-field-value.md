---
unique-page-id: 2359663
description: Définir une valeur de champ de formulaire masqué - Documents Marketo - Documentation du produit
title: Définition d’une valeur de champ de formulaire masqué
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 2%

---

# Définition d’une valeur de champ de formulaire masqué {#set-a-hidden-form-field-value}

Les champs masqués sont généralement renseignés dynamiquement. Ils ne sont pas présentés à la personne qui remplit le formulaire. Voici comment définir la valeur.

>[!PREREQUISITES]
>
>[Définir un champ de formulaire comme masqué](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Sélection du champ {#select-the-field}

1. Dans votre formulaire, sélectionnez le champ masqué et cliquez sur **Modifier** pour **Remplissage automatique**.

   ![](assets/autofill.png)

## Utiliser la valeur par défaut : {#use-default-value}

En sélectionnant Utiliser la valeur par défaut , vous pouvez coder en dur une valeur spécifique qui sera toujours utilisée lors de l’envoi de ce formulaire. Saisissez la valeur par défaut et cliquez sur Enregistrer.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Paramètre URL {#url-parameter}

Si vous souhaitez capturer les paramètres d’URL (chaînes de requête) à partir de la page sur laquelle se trouve la personne lors du remplissage du formulaire, vous pouvez utiliser les **paramètres d’URL** pour remplir votre champ masqué.

>[!NOTE]
>
>Les paramètres sont plutôt techno, n&#39;est-ce pas ? Une fois qu&#39;on les trouve, ils sont puissants. Cette [page Wikipédia sur les chaînes de requête](https://en.wikipedia.org/wiki/Query_string) est quelque peu utile.

1. Sélectionnez **Paramètre d’URL** pour **Obtenir le type de valeur**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Saisissez le **Nom du paramètre** et cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Vous pouvez saisir une valeur par défaut si le paramètre d’URL est introuvable.

## Valeur du cookie {#cookie-value}

Si vous stockez des données dans des cookies, vous pouvez utiliser la **valeur du cookie** pour récupérer les données lors de l’envoi du formulaire.

1. Sélectionnez **Valeur du cookie** pour **Obtenir la valeur de**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Saisissez le nom du paramètre de cookie que vous souhaitez, puis cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Vous pouvez saisir une valeur par défaut au cas où le paramètre/cookie serait introuvable.

## Paramètre référent {#referrer-parameter}

Si vous souhaitez capturer les données de la page d’où provient le visiteur avant de remplir le formulaire, vous pouvez utiliser **Paramètre du référent**.

1. Définissez **Obtenir la valeur de** sur **Paramètre du référent**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Saisissez le **Nom de paramètre** que vous souhaitez extraire de l’URL du référent et cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Vous pouvez saisir une **valeur par défaut** au cas où le paramètre de référent serait introuvable.

1. Cliquez sur **Terminer**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Cliquez sur **Approuver et fermer**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
