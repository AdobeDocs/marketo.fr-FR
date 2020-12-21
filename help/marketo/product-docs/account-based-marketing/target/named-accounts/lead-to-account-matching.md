---
unique-page-id: 11381156
description: Correspondance de compte - Documents marketing - Documentation du produit
title: Correspondance de piste avec compte
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Correspondance de compte {#lead-to-account-matching}

La correspondance à droite conduit à des comptes nommés à droite à l’aide de la correspondance de pistes vers comptes de marketing.

>[!NOTE]
>
>**La** correspondance de pistes/comptes est une fonctionnalité intégrée du marketing basé sur les comptes de marketing. Il utilise une logique floue pour faire correspondre automatiquement les pistes aux bons comptes nommés en temps quasi réel. Il peut s’agir de comptes CRM ou de sociétés marketing.

La mise en correspondance de pistes vers comptes du marketing suit un processus en 4 étapes :

**Étape 1 -** Notre processus de rapprochement commence par l&#39;utilisation d&#39;informations clés sur les enregistrements de piste, telles que :

* Domaine de courriel (acme.com, par exemple)
* Nom de société déduit de l&#39;adresse IP
* Nom de la société : il peut s&#39;agir du nom du compte CRM ou de l&#39;attribut du nom de la société de piste (par exemple, provenant du remplissage du formulaire)

**Étape 2 -** Nous normalisons les noms de société que nous trouvons en fonction de divers attributs de piste (par exemple, Acme Inc. et Acme Corp sont automatiquement normalisés en Acme). Cette étape permet de garantir une représentation unique du compte nommé dans Marketo et d&#39;afficher toutes les pistes dans un seul compte nommé.

**Étape 3 -** Nous partageons les pistes correspondantes dans 2 compartiments : Correspondance forte et Correspondance faible.

* Les pistes avec correspondance faible s&#39;affichent sur les comptes nommés, qui peuvent ensuite être résolues manuellement.

**Étape 4 -** Nous présentons une liste de sociétés proposées avec des correspondances fortes et faibles. Lorsqu&#39;un compte nommé est créé en fonction de l&#39;une des sociétés proposées, nous créons des règles de correspondance pour associer automatiquement de nouvelles pistes (par exemple, des pistes renseignées dans un formulaire) vers les comptes nommés de droite. Ainsi, vous pouvez vous inquiéter moins de la correspondance des pistes que de l&#39;obtention de recettes !

La mise en correspondance des pistes vers les comptes étant une fonction intégrée du marketing basé sur les comptes de marketing, la mise en correspondance des pistes vers les comptes se produit en temps quasi réel (par exemple, dès qu&#39;une piste remplit un formulaire de marketing, nous associons cette piste au bon compte nommé). Ce événement peut être utilisé pour déclencher des alertes et avertir les propriétaires des comptes des nouvelles pistes provenant de leurs comptes nommés.

>[!NOTE]
>
>Si vous utilisez LeanData dans Salesforce pour effectuer une correspondance de piste vers compte, Marketo dispose d’une intégration qui synchronisera ces correspondances avec votre instance Marketo. Pour activer cette fonction, contactez le [Support marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Discover Comptes](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md)
