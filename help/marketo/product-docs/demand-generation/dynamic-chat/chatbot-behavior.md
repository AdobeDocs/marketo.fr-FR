---
description: Comportement du bot conversationnel - Documents Marketo - Documentation du produit
title: Comportement du chatbot
feature: Dynamic Chat
exl-id: e91e7981-6617-42fe-8120-a7311a99cdfb
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1680'
ht-degree: 3%

---

# Comportement du chatbot {#chatbot-behavior}

Voici différents scénarios possibles décrivant le comportement attendu du bot conversationnel avec le visiteur dans chacun d’eux.

<table>
  <tbody>
    <tr>
      <th>Abréviation</th>
      <th>Détails</th>
    </tr>
    <tr>
      <td>D1, D2, D3, etc.</td>
      <td>Représente plusieurs boîtes de dialogue où D1 est la première boîte de dialogue</td>
    </tr>
    <tr>
      <td>P1, P2, P3, etc.</td>
      <td>Représente les priorités de dialogue pour lesquelles P1 est la priorité la plus élevée</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3, etc.</td>
      <td>Représente plusieurs pages web où WP1 est la première page web</td>
    </tr>
    <tr>
      <td>V1, V2, V3, etc.</td>
      <td>Représente plusieurs visiteurs de page web où V1 est visiteur un</td>
    </tr>
   </tbody>
</table>

## Scénarios {#scenarios}

<table>
  <tr>
      <th>Scénario</th>
      <th>Comportement attendu du bot conversationnel</th>
      <th>Action du serveur principal</th>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visites WP1</p>
      </td>
      <td>
        <p>D1 sera résolu en V1</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 sera augmenté de 1</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visites WP1</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu en V1</p>
        <p>Après actualisation, D1 sera résolu à nouveau</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Après l’actualisation, aucune modification du déclencheur D1 ou du nombre d’engagements</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 mais n'a pas répondu</p>
      </td>
      <td>D1 sera résolu en V1</td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Aucune modification du nombre d’engagements D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 et fournit la première réponse</p>
      </td>
      <td>D1 sera résolu en V1</td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Le nombre d’engagements pour D1 sera augmenté de 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 et fournit la première réponse</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu en V1</p>
        <p>Après actualisation, D1 se poursuit</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs et le nombre d’engagements pour D1 seront augmentés de 1</p>
        <p>Après actualisation, aucun changement n’est apporté au nombre</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1, interagit avec le chatbot et termine D1</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu en V1</p>
        <p>Après l’actualisation, aucune boîte de dialogue ou boîte de dialogue suivante ne sera résolue pour la version 1</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs, le nombre d’engagements et le nombre terminé pour D1 seront augmentés de 1</p>
        <p>Après l’actualisation, aucune boîte de dialogue ou boîte de dialogue suivante ne sera résolue</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement, WP2</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 mais n'a pas répondu</p>
        <p>V1 visites WP2</p>
      </td>
      <td>
        <p>La visite de page WP1, D1 sera résolue en V1</p>
        <p>La visite de page WP2, D1 sera résolue en V2</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Dans WP2, pas de modification du nombre de déclencheurs D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement, WP2</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 et est engagée</p>
        <p>V1 visites WP2</p>
      </td>
      <td>
        <p>La visite de page WP1, D1 sera résolue en V1</p>
        <p>La visite de page WP2, D1 sera résolue en V1</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs et le nombre d’engagements pour D1 seront augmentés de 1</p>
        <p>Dans WP2, aucune modification n'est apportée à un comptage</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>D2 ciblé pour WP2 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 et fournit la première réponse</p>
        <p>V1 visites WP2</p>
      </td>
      <td>
        <p>D1 sera résolu sur WP1</p>
        <p>D1 continuera à V1 sur WP2</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs et le nombre d’engagements pour D1 seront augmentés de 1</p>
        <p>Aucune modification du déclencheur D2 ou du nombre d’engagements</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>D2 ciblé pour WP2 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 mais n'a pas répondu</p>
        <p>V1 visites WP2</p>
      </td>
      <td>D1 sera résolu sur WP1<br/>
      D2 sera résolu sur WP2</td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Le nombre de déclencheurs pour D2 sera augmenté de 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>D2 ciblé pour WP2 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 et termine D1</p>
        <p>V1 visites WP2</p>
      </td>
      <td>D1 sera résolu sur WP1 et après achèvement<br/>D2 sera résolu sur WP2</td>
      <td>
        <p>Le nombre de déclencheurs, le nombre d’engagements et le nombre terminé pour D1 seront augmentés de 1</p>
        <p>Le nombre de déclencheurs pour D2 sera augmenté de 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>D2 ciblé pour WP2 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 et termine D1</p>
        <p>V1 visites WP2</p>
        <p>Les clics V1 sur D2 fournissent la première réponse</p>
      </td>
      <td>D1 sera résolu sur WP1 et après achèvement<br/>D2 sera résolu sur WP2</td>
      <td>
        <p>Le nombre de déclencheurs, le nombre d’engagements et le nombre terminé pour D1 seront augmentés de 1</p>
        <p>Le nombre de déclencheurs et d’engagements pour D2 sera augmenté de 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 mais n'a pas répondu</p>
        <p>D1 est dépublié</p>
      </td>
      <td>D1 sera résolu en V1</td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Aucune modification du nombre d’engagements D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 mais n'a pas répondu</p>
        <p>D1 est dépublié</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois</p>
        <p>Après actualisation, aucune boîte de dialogue ne sera résolue</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Aucune modification du nombre d’engagements D1</p>
        <p>Après l’actualisation, aucune modification du déclencheur D1 ou du nombre d’engagements</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 engagée avec D1</p>
        <p>D1 est dépublié</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu en V1</p>
        <p>Après actualisation, D1 se poursuit</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Le nombre d’engagements D1 sera augmenté de 1</p>
        <p>Après l’actualisation, comme D1 se poursuit, aucune autre modification n’est apportée au déclencheur ou au nombre d’engagements</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 mais n'a pas répondu</p>
        <p>D1 est publié avec de nouvelles modifications.</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois</p>
        <p>Après l’actualisation, la boîte de dialogue contenant les nouvelles modifications sera résolue</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Après actualisation, utilisez D1 avec de nouvelles modifications, mais aucune autre modification pour déclencher le comptage.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>Les clics V1 sur D1 fournissent la première réponse</p>
        <p>D1 est publié avec de nouvelles modifications.</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois</p>
        <p>Après l’actualisation, la boîte de dialogue avec les anciennes modifications se poursuit</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Le nombre d’engagements pour D1 sera augmenté de 1</p>
        <p>Après l’actualisation, comme l’ancien D1 s’affiche, ne modifiez pas le nombre de déclencheurs</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 ciblé pour WP1 avec 1 priorité</p>
        <p>D2 ciblé pour WP1 avec 2 priorités</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 mais n'a pas répondu</p>
        <p>D1 est dépublié</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois</p>
        <p>Après actualisation, D2 sera résolu en V1</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Après actualisation, le nombre de déclencheurs pour D2 est augmenté de 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec 1 priorité</p>
        <p>D2 ciblé pour WP1 avec 2 priorités</p>
        <p>V1 visite WP1 pour la première fois</p>
        <p>V1 clique sur D1 et termine D1</p>
        <p>V1 actualise WP1 et voit D2<br/>V1 clics sur D2 et termine D2</p>
        <p>Le marketeur a apporté des modifications à D1 et a été republié.</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois</p>
        <p>Après actualisation, D2 sera résolu en V1</p>
        <p>Après avoir terminé D1 et D2, quelles que soient les modifications ou la republication D1, D2 ne sera pas affiché à nouveau à V1</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs, le nombre d’engagements et le nombre terminé pour D1 seront augmentés de 1</p>
        <p>Actualiser une fois D2 terminé, aucune action à effectuer</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec un déclencheur « Time on Site » de 30 secondes</p>
        <p>V1 visites WP1</p>
      </td>
      <td>
        <p>D1 sera résolu mais ne sera pas déclenché vers V1</p>
        <p>Après 30 secondes, D1 s’affiche/est déclenché sur V1</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 sera augmenté de 1 uniquement après plus de 30 secondes passées sur la page web</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1, WP2 avec un déclencheur « Time on page » de 30 secondes</p>
        <p>V1 visites WP1, WP2</p>
      </td>
      <td>
        <p>D1 sera résolu mais ne sera pas déclenché vers V1</p>
        <p>Après 30 secondes, D1 s’affiche/est déclenché sur V1</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 sera augmenté de 1 uniquement après plus de 30 secondes passées sur la page web</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec un déclencheur de « pourcentage de défilement » de 50</p>
        <p>V1 visites WP1</p>
      </td>
      <td>
        <p>D1 sera résolu mais ne sera pas déclenché vers V1</p>
        <p>Après un défilement de 50 %, D1 est affiché/déclenché sur V1</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 sera augmenté de 1 uniquement après un défilement de 50 %</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec 1 priorité et un déclencheur d'événement « Time on page » de 30 secondes</p>
        <p>D2 ciblé pour WP1 avec 2 priorités et événement « pourcentage de défilement de page » de 50</p>
        <p>V1 visite WP1, après 10 secondes V1 visite WP2, V1 visite WP1</p>
      </td>
      <td>
        <p>Sur WP1, D1 sera résolu mais ne sera pas déclenché sur V1</p>
        <p>Sur WP2, D2 sera résolu mais ne sera pas déclenché sur V1</p>
        <p>Sur WP1, D1 sera résolu et après 20 secondes, D1 sera déclenché sur V1</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 sera augmenté de 1 uniquement après 30 secondes</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec un déclencheur « Temps passé sur le site » de 1 minute</p>
        <p>V1 visite WP1 pendant 1 minute et est affiché D1 mais n'engage pas</p>
        <p>V1 ferme WP1 et revient à WP1 2 jours plus tard</p>
      </td>
      <td>
        <p>D1 s’affiche automatiquement dans la version V1, car il répond déjà aux critères de déclenchement lors de la session précédente</p>
        <p>La même logique s’applique à « Temps passé sur la page » et « pourcentage de défilement de la page »</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Après le retour, aucune action à entreprendre</p>
      </td>
    </tr>
  </tbody>
</table>

## Résolution des leads en temps réel {#real-time-lead-resolution}

Lors d’une conversation avec un lead anonyme et avec un ID d’e-mail fourni, nous déterminons si un enregistrement de lead connu existe avec cet ID d’e-mail et utilisons cet enregistrement pour la personnalisation en temps réel. Si nous trouvons plusieurs enregistrements, nous les fusionnons en temps réel. Ce comportement est implémenté pour les boîtes de dialogue et les flux conversationnels.
