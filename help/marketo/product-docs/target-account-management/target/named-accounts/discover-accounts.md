---
unique-page-id: 11378812
description: Discover Comptes - Documents Marketo - Documentation du produit
title: Découverte des comptes
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 1%

---

# Découverte des comptes {#discover-accounts}

Utilisez l’option Discover pour identifier les comptes cibles potentiels.

## Découvrir les comptes CRM {#discover-crm-accounts}

Identifiez les comptes cibles potentiels à partir de votre CRM.

>[!NOTE]
>
>Une fois que vous avez connecté votre CRM à Marketo TAM, **Découverte des comptes CRM** affiche tous les comptes CRM et les informations pertinentes pour vous aider à choisir les comptes nommés appropriés. Marketo ajoute des informations supplémentaires sur ce qui est reçu du CRM.

**Personnes** (Dans Comptes CRM Discover et sociétés Marketo Discover) : Inclut à la fois les contacts et les pistes. Les pistes peuvent être découvertes à l’aide de Marketo [correspondance de piste à compte](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md).

**Personnes potentielles** (Dans Comptes CRM Discover et sociétés Marketo Discover) : Indique le nombre de pistes trouvées par Marketo qui peuvent appartenir à un compte CRM.

**Champ CRM personnalisé** (Dans les comptes CRM Discover uniquement) : Cela vous aidera à aligner votre organisation commerciale et marketing pour la sélection de comptes cibles corrects. Une fois que [faire correspondre le champ CRM personnalisé](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) avec Marketo TAM, nous vous montrerons les données mappées pour vous aider à identifier vos comptes cibles.

1. Dans Comptes nommés, cliquez sur le bouton **Nouveau** et sélectionnez **Découverte des comptes CRM**.

   ![](assets/disc-crm-one.png)

1. Une nouvelle fenêtre ou un nouvel onglet s’ouvre. Sélectionnez le ou les comptes CRM que vous souhaitez ajouter à vos comptes nommés et cliquez sur **Suivant**.

   ![](assets/disc-crm-two.png)

1. L’écran de prévisualisation confirme le nombre de sélections. Cliquez sur **Créer**.

   ![](assets/disc-three.png)

   C&#39;est tout ce qu&#39;il y a à ça !

   ![](assets/disc-four.png)

## Découvrir les sociétés Marketo {#discover-marketo-companies}

Identifiez les bonnes entreprises pour le ciblage.

>[!NOTE]
>
>Dans les sociétés Discover Marketo, vous verrez les sociétés Marketo qui ne proviennent pas de votre système de gestion de la relation client.

1. Dans Comptes nommés, cliquez sur le bouton **Nouveau** et sélectionnez **Découvrez les entreprises Marketo**.

   ![](assets/one-1.png)

1. Une nouvelle fenêtre ou un nouvel onglet s’ouvre. Sélectionnez les sociétés à ajouter à vos comptes nommés, puis cliquez sur **Suivant**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >Dans les entreprises Discover Marketo et Discover CRM, Marketo automatiquement :
   >
   >* Recherche les personnes de votre base de données Marketo dont l’entreprise est répertoriée dans leur enregistrement. Si plusieurs valeurs s’affichent pour certains attributs (secteur, par exemple), c’est parce que Marketo a trouvé des valeurs différentes répertoriées pour ces personnes. L’attribut avec le plus d’accès gagne
   >
   >Dans **Discover CRM** uniquement, Marketo automatiquement :
   >
   >* Synchronise et associe les contacts CRM au compte nommé
   >
   >Dans **Découvrez les entreprises Marketo** uniquement, Marketo automatiquement :
   >
   >* Filtre la plupart des fournisseurs de services Internet et des domaines publics (par exemple, yahoo.com, gmail.com) comme noms de société
   >
   >* déduplique les comptes CRM. Si vous avez &quot;Acme&quot; dans un enregistrement et &quot;Acme Inc&quot; (ou l’un des suffixes suivants : Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), nous les fusionnerons dans TAM en tant que simplement &quot;Acme&quot;.

   >
   >Si vous souhaitez que Marketo déduplique les comptes par identifiant CRM ou propriétaire de compte au lieu de par nom de société, contactez [Prise en charge de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Cliquez sur la flèche vers le bas située sous la colonne Compte nommé pour afficher le menu déroulant.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >Dorénavant, toutes les nouvelles personnes issues de ces sociétés sélectionnées seront automatiquement affectées à leurs comptes nommés respectifs. Vérifiez deux fois ces sociétés et assurez-vous qu’elles sont affectées au compte nommé approprié.

1. Pour sélectionner un compte existant, cliquez sur le bouton **Compte nommé** , sélectionnez le compte de votre choix, puis cliquez sur **Suivant**.

   ![](assets/disc-comp-four.png)

   Vous avez également la possibilité de créer un compte nommé en saisissant directement le nom de votre choix dans la liste déroulante. Lorsque vous avez terminé, cliquez en dehors de la zone...

   ![](assets/disc-comp-five.png)

   ...et votre nouveau compte nommé s’affiche. À ce stade, cliquez simplement sur **Suivant** comme à l’étape 4.

   ![](assets/disc-comp-six.png)

1. Cliquez sur **Créer**.

   ![](assets/disc-comp-seven.png)

   Beau travail !

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Si vous constatez une incohérence entre les comptes CRM que vous avez sélectionnés et ce qui se trouve dans la grille CRM Discover, cela est probablement dû à l’une ou plusieurs des raisons suivantes :
>
>* Disposer de différents comptes CRM avec des noms similaires qui ont été dédupliqués
>* La synchronisation planifiée suivante ne s’est pas encore produite


>[!MORELIKETHIS]
>
>[Correspondance de pistes de comptes](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
