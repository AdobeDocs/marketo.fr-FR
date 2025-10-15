---
description: OP-Scoring-Behaviour - Documents Marketo - Documentation du produit
title: OP-Score-Comportement
feature: Programs
exl-id: c564a301-0054-431a-8f0f-0299cd91b59c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 30%

---

# OP-Score-Comportement {#op-scoring-behavior}

Cet exemple est un programme opérationnel avancé (segmenté en unités lexicales) pour le score de comportement à l’aide d’un programme par défaut de Marketo Engage. Affichez et modifiez les valeurs de notation sous l’onglet « Mes jetons » du programme. Nécessite un champ de score personnalisé appelé « Score de comportement ».

Pour obtenir de l’aide sur la stratégie ou la personnalisation d’un programme, contactez l’équipe du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/fr/customers/consulting-services/main.html){target="_blank"}.

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
   <td>01-Membre</td>
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
   <td>Évaluation comportementale</td>
   <td>BehaviorScore</td>
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
   <td>E-mail - Clics sur le lien dans l’e-mail</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Formulaire - Remplit Le Formulaire De Contact</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Formulaire : remplit le formulaire de contenu</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Formulaire : Remplit Le Formulaire Par Défaut</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Formulaire : remplit le formulaire d’événement</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Web - Télécharge n’importe quel PDF</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Web - Score PPC</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Web - Pages Web Clés Des Visites</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Web - Visite de plusieurs pages Web en 1 jour</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Événement en direct - avec participation</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Salon professionnel - influencé</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Salon professionnel - kiosque visité</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Webinaire - Terminé</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Diminuer le score - Aucune activité</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Diminuer le score - Visites de pages web indésirables</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Interactions</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Modifications du statut du programme</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Atténuation du score</td>
  </tr>
 </tbody>
</table>

![](assets/op-scoring-behavior-1.png)

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
   <td><code>{{my.Decrease Score - No Activity}}</code></td>
   <td>-10</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Decrease Score - Visits Undesirable Web Pages}}</code></td>
   <td>-5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Email - Clicks Link}}</code></td>
   <td>+2</td>
  </tr>
   <tr>
   <td>Score</td>
   <td><code>{{my.Form - Fills Out Contact Form}}</code></td>
   <td>+30</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Form - Fills Out Content Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Form - Fills Out Default Form}}</code></td>
   <td>+10</td>
  </tr>
   <tr>
   <td>Score</td>
   <td><code>{{my.Form - Fills-out Event Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Live Event - Attended}}</code></td>
   <td>+30</td>
  </tr>
   <tr>
   <td>Score</td>
   <td><code>{{my.Tradeshow - Influenced}}</code></td>
   <td>+20</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Tradeshow - Visited Booth}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Web - Downloaded Any PDF}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Web - PPC Scoring}}</code></td>
   <td>+15</td>
  </tr>
   <tr>
   <td>Score</td>
   <td><code>{{my.Web - Visits Key Web Pages}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Web - Visits Multiple Web Pages in 1 Day}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Score</td>
   <td><code>{{my.Webinar - Attended}}</code></td>
   <td>+20</td>
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
