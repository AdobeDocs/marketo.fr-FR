---
unique-page-id: 2359663
description: Définir une valeur de champ de formulaire masqué - Documents marketing - Documentation du produit
title: Définir une valeur de champ de formulaire masqué
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Définir une valeur de champ de formulaire masqué {#set-a-hidden-form-field-value}

Les champs masqués sont généralement renseignés de manière dynamique. Ils ne sont pas présentés à la personne qui remplit le formulaire. Voici comment définir la valeur.

>[!NOTE]
>
>**Conditions préalables**
>
>[Définir un champ de formulaire comme masqué](set-a-form-field-as-hidden.md)

## Sélectionner le champ {#select-the-field}

1. Dans votre formulaire, sélectionnez le champ masqué et cliquez sur **Modifier** pour **Remplir automatiquement**.

   ![](assets/autofill.png)

## Utiliser la valeur par défaut {#use-default-value}

En sélectionnant Utiliser la valeur par défaut, vous pouvez coder en dur une valeur spécifique qui sera toujours utilisée lors de l’envoi de ce formulaire. Saisissez la valeur par défaut et cliquez sur Enregistrer.

![](assets/image2014-9-15-13-3a5-3a27.png)

## Paramètre d’URL {#url-parameter}

Si vous souhaitez capturer des paramètres d’URL (chaînes de Requête) à partir de la page sur laquelle se trouve la personne lors du remplissage du formulaire, vous pouvez utiliser les **paramètres** d’ **URL** pour renseigner votre champ masqué.

>[!NOTE]
>
>Les paramètres sont plutôt techniques, n&#39;est-ce pas ? Une fois qu&#39;on les trouve, ils sont puissants. Cette page [Wikipédia sur Requête Strings](http://en.wikipedia.org/wiki/Query_string) est quelque peu utile.

1. Sélectionnez Paramètre **** d’URL pour le type **** Get Value.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Saisissez le nom **du** paramètre, puis cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Vous pouvez entrer une valeur par défaut au cas où le paramètre d’URL serait introuvable.

## Valeur du cookie {#cookie-value}

Si vous stockez des données dans des cookies, vous pouvez utiliser **la** valeur **du cookie** pour récupérer les données lorsque le formulaire est envoyé.

1. Sélectionnez **Cookie** **Value** pour **Get** **Value From.******

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Saisissez le nom de paramètre du cookie que vous souhaitez, puis cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Vous pouvez entrer une valeur par défaut au cas où le paramètre/cookie serait introuvable.

## Paramètre de parrain {#referrer-parameter}

Si vous souhaitez capturer des données à partir de la page d’où provient le visiteur avant de remplir le formulaire, vous pouvez utiliser le **paramètre de** Parrain ****.

1. Définissez **Get** **Value** **From** to **Parrain Parameter.******

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Saisissez le nom **du** paramètre que vous souhaitez extraire de l’URL du parrain et cliquez sur **Enregistrer**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Vous pouvez saisir une **valeur** par défaut **** au cas où le paramètre de parrain serait introuvable.

1. Cliquez sur **Terminer**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Cliquez sur **Approuver et fermer**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)

Doux ! Vous vous en sortez plutôt bien. Il y a plus à apprendre sur les [formulaires](http://docs.marketo.com/display/docs/forms).
