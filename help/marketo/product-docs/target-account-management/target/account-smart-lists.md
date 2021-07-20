---
unique-page-id: 11378814
description: Listes dynamiques de compte - Documents Marketo - Documentation du produit
title: Listes dynamiques de compte
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
source-git-commit: e4d581ab258a875747a6d5323764e8b4a3949cba
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 1%

---

# Listes dynamiques de compte {#account-smart-lists}

Voici comment identifier rapidement et précisément vos comptes à forte valeur ajoutée.

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que pour les personnes disposant du module complémentaire de gestion de compte Target et d’une licence TAM émise.

## Création d’une liste dynamique de comptes {#create-an-account-smart-list}

1. Dans Marketo, accédez à **Activités marketing**.

   ![](assets/account-smart-lists-1.png)

1. Recherchez et sélectionnez le programme souhaité.

   ![](assets/account-smart-lists-2.png)

1. Cliquez sur la liste déroulante **New** et sélectionnez **New Local Asset**.

   ![](assets/account-smart-lists-3.png)

1. Cliquez sur **Liste dynamique de compte**.

   ![](assets/account-smart-lists-4.png)

1. Saisissez un nom et cliquez sur **Créer** (la description et les libellés sont facultatifs).

   ![](assets/account-smart-lists-5.png)

Votre liste dynamique de comptes a été créée. Voir ci-dessous les étapes de définition de ses règles.

## Règles de la liste intelligente des comptes {#account-smart-list-rules}

Les listes dynamiques de compte fonctionnent de la même manière que les listes dynamiques standard, à une exception notable : conteneurs.

1. Pour définir votre liste dynamique de comptes, cliquez sur l’onglet **Règles de liste dynamique de comptes** .

   ![](assets/account-smart-lists-6.png)

1. Sélectionnez le ou les filtres de compte de votre choix. Dans cet exemple, nous choisissons _Le secteur industriel est celui des soins de santé_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

1. Sélectionnez votre ou vos filtres de personne(s) mappée(s). Dans cet exemple, nous choisissons _État : Californie_.

   ![](assets/account-smart-lists-9.png)

**Étape** facultative : C&#39;est là que les conteneurs entrent. Si vous choisissez un autre filtre de personne mise en correspondance, vous pouvez le déposer sous le premier, ou _dans_, ce qui crée un conteneur. Dans cet exemple, nous allons créer un conteneur en ajoutant _Le titre de la tâche est CFO_.

![](assets/account-smart-lists-10.png)

Voici à quoi ressemblera le conteneur.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>La création d’un conteneur de filtres crée une règle &quot;et&quot;, ce qui signifie qu’elle ne renverra que tous les résultats combinés. Dans cet exemple, tient compte d’un secteur de la santé, et se trouve en Californie _et_ avec une personne nommée CFO. Si vous ne souhaitez pas utiliser de conteneurs, déposez simplement le filtre en dessous/au-dessus de celui existant.

Et voilà ! Consultez la section ci-dessous pour découvrir comment tirer parti de votre liste dynamique de comptes.

>[!TIP]
>
>Tout comme avec les listes intelligentes standard, vous pouvez utiliser une logique avancée pour affiner davantage vos résultats. Pour ce faire, vous avez besoin d’au moins trois filtres. Dans les listes dynamiques de compte, un conteneur (quel que soit le nombre de filtres qu’il contient lui-même) équivaut à un filtre.

## Actions de la liste intelligente des comptes {#account-smart-list-actions}

Dans l’onglet Aperçu de votre liste dynamique de comptes, vous remarquerez quelques options d’action.

**Export** : Cette opération exporte les résultats de votre liste dynamique de comptes au format CSV.

**Cloner** : Effectue une copie de votre liste dynamique de compte.

**Envoyer au réseau publicitaire** : Envoie la liste à LinkedIn en tant que nouvelle audience mise en correspondance.

Vous pouvez également référencer votre liste dynamique de compte dans une liste/campagne dynamique standard à l’aide du filtre _Personnes membres de la liste dynamique de compte_.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Les résultats de la liste dynamique Personnes membres du compte affichent chaque personne dans le ou les comptes identifiés, et pas seulement les personnes qui se trouvent via les filtres de personne mise en correspondance dans la liste dynamique des comptes.

>[!NOTE]
>
>**Définition**
>
>**Personnes membres de la liste** dynamique de compte : Dans ce cas, le mot &quot;membre&quot; fait référence au compte lui-même, de sorte que &quot;membre du peuple&quot; signifie les personnes réelles (enregistrements Marketo) dans ces comptes.
