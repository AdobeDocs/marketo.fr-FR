---
unique-page-id: 11380774
description: Score de compte - Documents Marketo - Documentation du produit
title: Évaluation du compte
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
feature: Target Account Management
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Évaluation du compte {#account-score}

La notation de compte est un élément essentiel de la gestion de compte Target. Cela vous aide à déterminer le niveau d’engagement de vos comptes.

## Qu’est-ce que la notation de compte ? {#what-is-account-scoring}

Il s’agit d’une approche systématique conçue pour aider les équipes de vente et de marketing à identifier et à prioriser les entreprises (y compris les prospects) les plus susceptibles de faire un achat.

Dans le monde complexe des processus d’achat B2B, il est rare qu’une seule personne prenne une décision d’achat. Il y a souvent différents rôles impliqués, chacun ayant ses propres besoins. La notation basée sur les comptes prend cela en compte en agrégeant les scores de piste de plusieurs pistes et en fournissant un score au niveau du compte.

## Exemples courants {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>Score d'engagement</strong></td> 
   <td>Profondeur de l’engagement basée sur les activités comportementales suivies sur différents canaux (par exemple, e-mail, web, publicité) par les personnes dans des comptes cibles spécifiques.</td>
  </tr>
  <tr>
   <td><strong>Score d’intérêt du produit du compte</strong></td>
   <td>Les personnes issues de comptes cibles qui montrent un intérêt pour le contenu d’un produit spécifique (par exemple, le téléchargement d’un livre blanc).</td> 
  </tr>
  <tr>
   <td><strong>Score d’engagement web du compte</strong></td>
   <td>Personnes provenant de comptes cibles visitant le canal web. Un même score peut être créé pour mesurer l’engagement des canaux à partir du courrier électronique, de la publicité ou d’autres canaux.</td> 
  </tr>
 </tbody>
</table>

## Comment configurer la note du compte {#how-to-configure-account-score}

>[!NOTE]
>
>Pour calculer les scores du compte, vous devez d’abord créer des scores de piste. Marketo TAM agrège automatiquement les scores de piste aux scores du compte. À titre d’exemple, nous allons prendre deux des exemples ci-dessus (_Score d’intérêt du produit du compte_ et _Score d’engagement web du compte_).
>
>Créez tout d’abord des champs de score de piste qui capturent les détails pertinents de chaque piste d’un compte cible.\
>Attribuez ensuite ces scores de piste à leurs scores de compte respectifs :\
>Score d’intérêt du produit du compte = SOMME (Score d’intérêt du produit de piste)\
>Score d’engagement Web du compte = SOMME (Score d’engagement Web de piste)

>[!NOTE]
>
>Les utilisateurs peuvent créer plusieurs scores d’engagement de compte et affecter différents scores de personne à différents scores de compte.

Une fois que vous avez configuré le score de piste, procédez comme suit.

1. Cliquez sur **Administration**.

   ![](assets/account-score-1.png)

1. Cliquez sur **Gestion de compte Target**.

   ![](assets/account-score-2.png)

1. Dans les champs de notation, cliquez sur **Modifier**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Vous pouvez choisir jusqu’à **cinq** pour calculer la note du compte.

1. Saisissez le nom du score du compte, puis cliquez sur le bouton **Sélectionner le score de personne** et sélectionnez le score correspondant.

   ![](assets/account-score-4.png)

1. Cliquez sur **+Ajouter** pour ajouter d’autres scores.

   ![](assets/account-score-5.png)

1. Ajoutez tous les scores souhaités. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/account-score-6.png)
