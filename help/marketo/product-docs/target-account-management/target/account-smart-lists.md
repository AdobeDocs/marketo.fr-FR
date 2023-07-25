---
unique-page-id: 11378814
description: Listes dynamiques de compte - Documents Marketo - Documentation du produit
title: Listes dynamiques de compte
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '508'
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

1. Cliquez sur le bouton **Nouveau** et sélectionnez **Nouvelle ressource locale**.

   ![](assets/account-smart-lists-3.png)

1. Cliquez sur **Liste dynamique de comptes**.

   ![](assets/account-smart-lists-4.png)

1. Saisissez un nom et cliquez sur **Créer** (La description et les étiquettes sont facultatives).

   ![](assets/account-smart-lists-5.png)

Votre liste dynamique de comptes a été créée. Voir ci-dessous les étapes de définition de ses règles.

## Règles de la liste intelligente des comptes {#account-smart-list-rules}

Les listes dynamiques de compte fonctionnent de la même manière que les listes dynamiques standard, à une exception notable : conteneurs.

1. Pour définir votre liste dynamique de comptes, cliquez sur le bouton **Règles de liste intelligente des comptes** .

   ![](assets/account-smart-lists-6.png)

1. Sélectionnez le ou les filtres de compte de votre choix. Dans cet exemple, nous choisissons _L&#39;industrie est la santé_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >Données d’indicateur ICP utilisées dans votre [Classement et réglage des profils de compte](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) s’affichent sous la forme d’attributs de compte personnalisés à utiliser dans votre liste dynamique de comptes. Ces données d’attribut personnalisé sont basées sur le moment où le modèle de profil de compte a été créé/mis à jour.

1. Sélectionnez votre ou vos filtres de personne(s) mappée(s). Dans cet exemple, nous choisissons _État de Californie_.

   ![](assets/account-smart-lists-9.png)

**ÉTAPE FACULTATIVE**: C&#39;est là que les conteneurs entrent. Si vous choisissez un autre filtre de personne mise en correspondance, vous pouvez le déposer sous le premier, ou _in_ créer un conteneur. Dans cet exemple, nous allons créer un conteneur en ajoutant _Titre de la tâche : CFO_.

![](assets/account-smart-lists-10.png)

Voici à quoi ressemblera le conteneur.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>La création d’un conteneur de filtres crée une règle &quot;et&quot;, ce qui signifie qu’elle ne renverra que tous les résultats combinés. Dans cet exemple, tient compte d’un secteur de la santé et se trouve en Californie. _et_ avec quelqu&#39;un qui est listé comme directeur financier. Si vous ne souhaitez pas utiliser de conteneurs, déposez simplement le filtre en dessous/au-dessus de celui existant.

Et voilà ! Consultez la section ci-dessous pour découvrir comment tirer parti de votre liste dynamique de comptes.

>[!TIP]
>
>Tout comme avec les listes intelligentes standard, vous pouvez utiliser une logique avancée pour affiner davantage vos résultats. Pour ce faire, vous avez besoin d’au moins trois filtres. Dans les listes dynamiques de compte, un conteneur (quel que soit le nombre de filtres qu’il contient lui-même) équivaut à un filtre.

## Actions de la liste intelligente des comptes {#account-smart-list-actions}

Dans l’onglet Aperçu de votre liste dynamique de comptes, vous remarquerez quelques options d’action.

**Exporter**: Cette opération exporte les résultats de votre liste dynamique de comptes au format CSV.

**Cloner**: Effectue une copie de votre liste dynamique de compte.

**Envoyer au réseau publicitaire**: Envoie la liste à LinkedIn en tant que nouvelle audience mise en correspondance.

Vous pouvez également référencer votre liste dynamique de compte dans une liste/campagne dynamique standard à l’aide de la variable _Liste dynamique des personnes membres du compte_ filtre.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Les résultats de la liste dynamique Personnes membres du compte affichent chaque personne dans le ou les comptes identifiés, et pas seulement les personnes qui se trouvent via les filtres de personne mise en correspondance dans la liste dynamique des comptes.

>[!NOTE]
>
>**Définition**
>
>**Liste dynamique des personnes membres du compte**: Dans ce cas, le mot &quot;membre&quot; fait référence au compte lui-même, de sorte que &quot;membre du peuple&quot; signifie les personnes réelles (enregistrements Marketo) dans ces comptes.
