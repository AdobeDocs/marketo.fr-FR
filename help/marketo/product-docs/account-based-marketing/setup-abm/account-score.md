---
unique-page-id: 11380774
description: Note de compte - Documentation sur le marketing - Documentation du produit
title: Note de compte
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Note de compte {#account-score}

La notation de compte est un élément essentiel du marketing basé sur le compte. Il vous permet de déterminer le niveau d’engagement de vos comptes.

## Qu’est-ce que la notation de compte ? {#what-is-account-scoring}

Il s&#39;agit d&#39;une approche systématique conçue pour aider les équipes de vente et de marketing à identifier et à classer par priorité les sociétés (y compris les prospects) les plus susceptibles de faire un achat.

Dans le monde complexe des processus d&#39;achat B2B, il est rare qu&#39;une seule personne prenne une décision d&#39;achat. Il y a souvent divers rôles en jeu, chacun avec ses propres besoins. La notation basée sur le compte en tient compte en agrégeant les scores de piste de plusieurs pistes et en fournissant un score au niveau du compte.

## Exemples courants {#common-examples}

| **Note sur l’engagement du compte** | Profondeur de l’engagement en fonction des activités comportementales suivies sur différents canaux (par exemple, courriel, web et publicité) par les personnes appartenant à des comptes de cible spécifiques. |
|---|---|
| **Score d’intérêt du produit du compte** | Les personnes des comptes de cible qui s&#39;intéressent au contenu d&#39;un produit spécifique (par exemple, le téléchargement d&#39;un livre blanc). |
| **Note d’engagement Web du compte** | Des personnes de comptes de cible visitant le canal Web. Il est possible de créer le même score pour mesurer l’engagement du canal à partir de la messagerie électronique, de la publicité ou d’autres canaux. |

## Comment configurer la note du compte {#how-to-configure-account-score}

>[!NOTE]
>
>**Explication**
>
>Pour calculer des scores de compte, vous devez d’abord créer des scores de piste. Marketo ABM : les agrégats dirigent automatiquement les scores vers les scores du compte. À titre d’exemple, nous prendrons deux des exemples ci-dessus (*Compte **Score d’intérêt du produit* et *Score d’engagement Web du compte*).
>
>Tout d&#39;abord, créez des champs de score de piste qui capturent les détails pertinents de chaque piste d&#39;un compte de cible.\
>Attribuez ensuite ces scores de piste à leurs scores de compte respectifs :\
>Score d’intérêt du produit du compte = SOMME (Score d’intérêt du produit du prospect)\
>Note d&#39;engagement Web du compte = SOMME (note d&#39;engagement Web de piste)

>[!NOTE]
>
>Les utilisateurs peuvent créer plusieurs scores d’engagement de compte et affecter différents scores de personne à différents scores de compte.

Une fois que vous avez configuré le score de piste, procédez comme suit.

1. Cliquez sur **Admin**.

   ![](assets/one-1.png)

1. Cliquez sur **ABM**.

   ![](assets/two-1.png)

1. Dans Champs de score, cliquez sur **Modifier**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Vous pouvez choisir jusqu’à **cinq **champs pour calculer la note du compte.

1. Saisissez le nom de la note de compte, cliquez sur la liste déroulante **Sélectionner une note de personne** et sélectionnez la note correspondante.

   ![](assets/four.png)

1. Cliquez sur **+Ajouter **pour ajouter d&#39;autres scores.

   ![](assets/five.png)

1. Ajoutez tous les scores souhaités. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/six.png)

