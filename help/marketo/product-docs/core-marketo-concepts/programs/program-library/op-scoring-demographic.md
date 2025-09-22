---
description: OP-Scoring-Demographic - Documents Marketo - Documentation du produit
title: OP-Score-Démographique
feature: Programs
exl-id: ed11616e-b587-4d03-b293-9cc9fa3c1699
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 35%

---

# OP-Score-Démographique {#op-scoring-demographic}

Il s’agit d’un exemple de programme opérationnel avancé (segmenté en unités lexicales) utilisant un programme par défaut de Marketo Engage pour la notation démographique. Affichez et modifiez les valeurs de notation sous l’onglet « Mes jetons » du programme. Nécessite un champ de score personnalisé appelé « Score démographique ».

Pour obtenir de l’aide sur la stratégie ou la personnalisation d’un programme, contactez l’équipe du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

## Résumé du canal {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Canal</th>
   <th>Statut d’abonnement</th>
   <th>Comportement d'analyse</th>
   <th>Type de programme</th>
  </tr>
  <tr>
   <td>Opérationnel</td>
   <td>01 - Membre</td>
   <td>Opérationnel</td>
   <td>Par défaut</td>
  </tr>
 </tbody>
</table>

## Champs prérequis {#prerequisite-fields}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Type</th>
   <th>Nom convivial</th>
   <th>Nom de l'API</th>
  </tr>
  <tr>
   <td>Score</td>
   <td>Évaluation démographique</td>
   <td>Score démographique</td>
  </tr>
 </tbody>
</table>

## Le programme contient les Assets suivantes {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Type</th>
   <th>Nom du modèle</th>
   <th>Nom de la ressource</th>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Domaine d’e-mail générique</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Prénom non valide</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Prénom non valide mis à jour</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nom non valide</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nom non valide mis à jour</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Revenus annuels</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Secteur industriel</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Intitulé du poste</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nombre d’employés</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Source</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Domaine d’e-mail générique</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Prénom non valide</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Nom non valide</td>
  </tr>
 </tbody>
</table>

![](assets/op-scoring-demographic-1.png)

## Mes jetons inclus {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Type de jeton</th>
   <th>Nom du jeton</th>
   <th>Valeur</th>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Annual Revenue - High}}</code></td>
   <td>+15</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Annual Revenue - Low}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Annual Revenue - Mid}}</code></td>
   <td>+10</td>
  </tr>
   <tr>
   <td>Score</td>
   <td><code>{{my.Generic Email Domain}}</code></td>
   <td>-2</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Industry - High}}</code></td>
   <td>+10</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Industry - Low}}</code></td>
   <td>+6</td>
  </tr>
   <tr>
   <td>Score</td>
   <td><code>{{my.Industry - Mid}}</code></td>
   <td>+8</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Invalid First Name}}</code></td>
   <td>-5</td>
  </tr>
   <tr>
   <td>Score</td>
   <td><code>{{my.Invalid First Name Updated}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Invalid Last Name}}</code></td>
   <td>-5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Invalid Last Name Updated}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Job Title - High}}</code></td>
   <td>+15</td>
  </tr>
   <tr>
   <td>Score</td>
   <td><code>{{my.Job Title - Low}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Job Title - Mid}}</code></td>
   <td>+10</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Lead Source - High}}</code></td>
   <td>+20</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Lead Source - Low}}</code></td>
   <td>+8</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Lead Source - Mid}}</code></td>
   <td>+10</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Number of Employees}}</code></td>
   <td>+5</td>
  </tr>
 </tbody>
</table>

## Règles de conflit {#conflict-rules}

* **Balises de programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page de destination portant le même nom**
   * Copier le modèle d’origine - _Recommandé_
   * Utiliser le modèle de destination

* **Images du même nom**
   * Conserver les deux fichiers - _Recommandé_
   * Remplacer l&#39;élément de cet abonnement

* **Modèles d’e-mail portant le même nom**
   * Conserver les deux modèles - _Recommandé_
   * Remplacer le modèle existant

## Meilleures pratiques {#best-practices}

* Chaque version de campagne est destinée à être un exemple de la version des bonnes pratiques et n’est pas spécifique à vos cas d’utilisation. N’oubliez pas de mettre à jour les campagnes intelligentes pour résoudre vos problèmes spécifiques et résoudre les problèmes liés aux données.

* Envisagez de mettre à jour la convention de nommage de cet exemple de programme pour l’aligner sur votre convention de nommage.
