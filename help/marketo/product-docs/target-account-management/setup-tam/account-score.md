---
unique-page-id: 11380774
description: Note de compte - Documentation sur le marketing - Documentation du produit
title: Note de compte
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Note de compte {#account-score}

La notation de compte est un élément essentiel de la gestion des comptes de Cible. Il vous permet de déterminer le niveau d’engagement de vos comptes.

## Qu’est-ce que la notation de compte ? {#what-is-account-scoring}

Il s&#39;agit d&#39;une approche systématique conçue pour aider les équipes de vente et de marketing à identifier et à classer par priorité les sociétés (y compris les prospects) les plus susceptibles de faire un achat.

Dans le monde complexe des processus d&#39;achat B2B, il est rare qu&#39;une seule personne prenne une décision d&#39;achat. Il y a souvent divers rôles en jeu, chacun avec ses propres besoins. La notation basée sur le compte en tient compte en agrégeant les scores de piste de plusieurs pistes et en fournissant un score au niveau du compte.

## Exemples courants {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>Note sur l’engagement du compte</strong></td> 
   <td>Profondeur de l’engagement en fonction des activités comportementales suivies sur différents canaux (par exemple, courriel, web et publicité) par les personnes appartenant à des comptes de cible spécifiques.</td>
  </tr>
  <tr>
   <td><strong>Score d’intérêt du produit du compte</strong></td>
   <td>Les personnes des comptes de cible qui s'intéressent au contenu d'un produit spécifique (par exemple, le téléchargement d'un livre blanc).</td> 
  </tr>
  <tr>
   <td><strong>Note d’engagement Web du compte</strong></td>
   <td>Des personnes de comptes de cible visitant le canal Web. Il est possible de créer le même score pour mesurer l’engagement du canal à partir de la messagerie électronique, de la publicité ou d’autres canaux.</td> 
  </tr>
 </tbody>
</table>

## Comment configurer la note du compte {#how-to-configure-account-score}

>[!NOTE]
>
>Pour calculer des scores de compte, vous devez d’abord créer des scores de piste. Marketo TAM automatiquement les agrégats conduisent les scores aux scores du compte. À titre d’exemple, nous allons prendre deux des exemples ci-dessus (_Note d’intérêt du produit du compte_ et _Note d’engagement Web du compte_).
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

1. Cliquez sur **Gestion du compte de Cible**.

   ![](assets/account-score-2.png)

1. Dans Champs de score, cliquez sur **Modifier**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Vous pouvez sélectionner jusqu’à **cinq champs** pour calculer la note du compte.

1. Saisissez le nom de la note de compte, cliquez sur la liste déroulante **Sélectionner une note de personne** et sélectionnez la note correspondante.

   ![](assets/four.png)

1. Cliquez sur **+Ajouter** pour ajouter d’autres scores.

   ![](assets/five.png)

1. Ajoutez tous les scores souhaités. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/six.png)
