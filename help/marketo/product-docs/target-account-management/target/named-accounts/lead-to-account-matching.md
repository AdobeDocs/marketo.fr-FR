---
unique-page-id: 11381156
description: Correspondance de comptes - Documents Marketo - Documentation du produit
title: Correspondance de pistes de comptes
exl-id: 676ae500-7691-492d-abec-0cac708216b7
source-git-commit: 98388f1ed941b321449e6e8badac0153dc2245ba
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Correspondance de pistes de comptes {#lead-to-account-matching}

La correspondance à droite mène à des comptes nommés à droite à l’aide de la correspondance de piste vers compte de Marketo.

>[!NOTE]
>
>**La** mise en correspondance de pistes/comptes est une fonctionnalité intégrée de la gestion de compte Marketo Target. Elle utilise une logique floue pour faire correspondre automatiquement les prospects aux comptes nommés appropriés en temps quasi réel. Ces comptes nommés peuvent être des comptes CRM ou des sociétés Marketo.

## APERÇU {#overview}

La correspondance de piste vers compte de Marketo suit un processus en 4 étapes :

**Étape 1 -** Notre processus de correspondance commence par l’utilisation d’informations clés sur les enregistrements de piste, telles que :

* Domaine de l’email (par exemple, acme.com)
* Nom de l’entreprise déduit de l’adresse IP
* Nom de la société : il peut s’agir du nom du compte CRM ou de l’attribut du nom de la société de prospect (par exemple, provenant du remplissage du formulaire).

**Étape 2 -** Nous normalisons les noms d’entreprise que nous trouvons en fonction de divers attributs de prospect (par exemple, Acme Inc. et Acme Corp sont automatiquement normalisés en Acme). Cette étape permet de s’assurer que nous disposons d’une représentation unique du compte nommé dans Marketo et que nous pouvons voir toutes les pistes dans un seul compte nommé.

**Étape 3 -** Nous avons divisé les pistes correspondantes en 2 lots : Correspondance forte et Correspondance faible.

* Les pistes présentant une faible correspondance apparaissent sur les comptes nommés, qui peuvent ensuite être résolues manuellement.

**Etape 4 -** Nous présentons une liste des entreprises proposées avec des correspondances fortes et faibles. Lorsqu’un compte nommé est créé en fonction de l’une des sociétés proposées, nous créons des règles correspondantes afin d’associer automatiquement les nouvelles pistes (par exemple, les pistes renseignées dans un formulaire) vers les comptes nommés de droite. Ainsi, vous pouvez vous soucier moins des pistes correspondantes et plus de l’obtention de recettes !

Comme la mise en correspondance de pistes vers comptes de Marketo est une fonctionnalité intégrée de la gestion de compte Target de Marketo, la mise en correspondance des pistes vers les comptes se produit presque en temps réel (par exemple, dès qu’une piste remplit un formulaire Marketo, nous associons cette piste au compte nommé approprié). Cet événement peut être utilisé pour déclencher des alertes et informer les propriétaires de compte des nouvelles pistes qui proviennent de leurs comptes nommés.

>[!NOTE]
>
>Si vous utilisez LeanData dans Salesforce pour établir une correspondance de piste vers compte, Marketo dispose d’une intégration qui synchronise ces correspondances avec votre instance Marketo. Pour que cette fonction soit activée, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) pour découvrir comment configurer LeanData ci-dessous.

## Utilisation de LeanData pour la correspondance de pistes vers des comptes {#using-leandata-for-lead-to-account-matching}

Une fois que la [prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) a activé LeanData pour votre compte, suivez les étapes ci-dessous pour le configurer.

1. Dans Salesforce, cliquez sur **Configurer l’accueil** dans le volet de navigation de gauche.

1. Toujours dans le volet de navigation de gauche, sous Administration, cliquez sur **Utilisateurs** puis sur **Profils**.

1. Recherchez et sélectionnez le profil **Synchronisation Marketo** .

1. Faites défiler l’écran jusqu’à la section Sécurité au niveau du champ et recherchez l’objet Lead. Sélectionnez **Afficher**.

1. Pour le nom du champ &quot;Compte mis en correspondance des rapports&quot;, assurez-vous que la case à cocher de la colonne **Accès en lecture** est cochée.

1. Dans Marketo, accédez à la section **Admin** .

   ![](assets/lead-to-account-matching-1.png)

1. Sélectionnez **Gestion des champs**.

   ![](assets/lead-to-account-matching-2.png)

1. Vérifiez que le champ se trouve en recherchant &quot;Compte mis en correspondance de rapports&quot;.

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
[Découverte des comptes](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)>
>
