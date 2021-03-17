---
unique-page-id: 11378814
description: Listes intelligentes du compte - Documentation du marketing - Documentation du produit
title: Listes intelligentes du compte
translation-type: tm+mt
source-git-commit: 96d6cc030ecd9d1da844fe27e1c6f62bbd181d62
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Listes intelligentes du compte {#account-smart-lists}

Voici comment identifier rapidement et précisément vos comptes à valeur élevée.

>[!NOTE]
>
>Cette fonctionnalité est disponible dans une version bêta ouverte et est accessible à toute personne qui a activé à la fois la gestion des balises et l’expérience utilisateur de la prochaine génération de Marketo. Veuillez contacter votre responsable si vous souhaitez participer à la version bêta.

## Créer une Liste intelligente de compte {#create-an-account-smart-list}

1. Dans Marketo, accédez à **Activités marketing**.

   ![](assets/account-smart-lists-1.png)

1. Recherchez et sélectionnez le programme de votre choix.

   ![](assets/account-smart-lists-2.png)

1. Cliquez sur la liste déroulante **New** et sélectionnez **New Local Asset**.

   ![](assets/account-smart-lists-3.png)

1. Cliquez sur **Liste intelligente du compte**.

   ![](assets/account-smart-lists-4.png)

1. Saisissez un nom et cliquez sur **Créer** (la description et les étiquettes sont facultatives).

   ![](assets/account-smart-lists-5.png)

Votre Liste Smart Account a été créée ! Voir ci-dessous les étapes de définition de ses règles.

## Règles de Liste intelligente du compte {#account-smart-list-rules}

Les Listes Smart de compte fonctionnent de la même manière que les Listes dynamiques standard, à l’exception notable : conteneurs.

1. Pour définir votre Liste intelligente de compte, cliquez sur l&#39;onglet **Règles de Liste intelligente de compte**.

   ![](assets/account-smart-lists-6.png)

1. Sélectionnez le ou les filtres de compte de votre choix. Dans cet exemple, nous choisissons _L&#39;industrie est la santé_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

1. Sélectionnez votre ou vos filtres de personne(s) à correspondance. Dans cet exemple, nous choisissons _L&#39;état est la Californie_.

   ![](assets/account-smart-lists-9.png)

**Étape** facultative : C&#39;est là que les conteneurs entrent en jeu. Si vous choisissez un autre filtre de personne mise en correspondance, vous pouvez le déposer sous le premier filtre, ou _dans_, ce qui crée un conteneur. Dans cet exemple, nous créons un conteneur en ajoutant _Le titre de la tâche est CFO_.

![](assets/account-smart-lists-10.png)

Voici à quoi ressemblera le conteneur.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>La création d’un conteneur de filtres crée une règle &quot;et&quot;, ce qui signifie qu’elle renvoie uniquement tous les résultats combinés. Dans cet exemple, il s’agit d’un compte auprès d’un secteur de la santé, en plus d’être situé en Californie _et_ avec une personne répertoriée comme directeur financier. Si vous ne souhaitez pas utiliser de conteneurs, il vous suffit de déposer le filtre au-dessous/au-dessus de celui existant.

Et c&#39;est tout ! Consultez la section ci-dessous pour savoir comment tirer parti de votre Liste intelligente de comptes.

>[!TIP]
>
>Tout comme avec les Listes dynamiques standard, vous pouvez utiliser une logique avancée pour affiner davantage vos résultats. Pour ce faire, vous devez disposer d’au moins trois filtres. Dans les Listes dynamiques de compte, un conteneur (quel que soit le nombre de filtres qu’elle contient) correspond à un filtre.

## Actions de Liste intelligente de compte {#account-smart-list-actions}

Dans l’onglet Aperçu de votre Liste intelligente de compte, vous remarquerez quelques options d’action.

**Exporter** : Cette opération exporte les résultats de votre Liste intelligente de compte au format CSV.

**Cloner** : Effectue une copie de votre Liste intelligente de compte.

**Envoyer au réseau** publicitaire : Envoie la liste à LinkedIn en tant que nouvelle Audience mise en correspondance.

Vous pouvez également référencer votre Liste intelligente de compte dans une Liste/Campaign dynamique standard en utilisant le filtre _Personnes membres de la Liste dynamique de compte_.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Les résultats de la Liste intelligente des personnes membres du compte montreront chaque personne dans le ou les comptes identifiés, et pas seulement les personnes qui sont trouvées via des filtres de personne rapprochée dans la liste intelligente du compte.

>[!NOTE]
>
>**Définition**
>
>**Personnes membres de la liste** dynamique du compte : Dans ce cas, le mot &quot;membre&quot; fait référence au compte lui-même, de sorte que &quot;membre du peuple&quot; signifie les personnes réelles (enregistrements de marqueur) dans ces comptes.
