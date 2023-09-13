---
description: Comportement de chatbot - Documents Marketo - Documentation du produit
title: Comportement de chatterbot
feature: Dynamic Chat
source-git-commit: 9a8f6fe57b585ba0eac6a577bf99e0419d8818a1
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Comportement de chatterbot {#chatbot-behavior}

Vous trouverez ci-dessous différents scénarios possibles qui surpassent le comportement attendu du visiteur dans chacun d’eux.

<table>
  <tbody>
    <tr>
      <th>Abréviation</th>
      <th>Détails</th>
    </tr>
    <tr>
      <td>D1, D2, D3, etc.</td>
      <td>Représente plusieurs boîtes de dialogue où D1 est une boîte de dialogue</td>
    </tr>
    <tr>
      <td>P1, P2, P3, etc.</td>
      <td>Représente les priorités de dialogue où P1 est la priorité la plus élevée</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3, etc.</td>
      <td>Représente plusieurs pages web où WP1 est la première page web.</td>
    </tr>
    <tr>
      <td>V1, V2, V3, etc.</td>
      <td>Représente plusieurs visiteurs de page web pour lesquels V1 est le visiteur un</td>
    </tr>
   </tbody>
</table>

## Scénarios {#scenarios}

<table>
  <tr>
      <th>Scénario</th>
      <th>Comportement attendu de Chatbot</th>
      <th>Action du serveur principal</th>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visites WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1</p>
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
        <p>D1 sera résolu sur V1</p>
        <p>Après l’actualisation, D1 sera résolu à nouveau.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Après actualisation, aucune modification n’est apportée au déclencheur D1 ni au nombre d’engagements.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>La V1 clique sur D1 mais n’a pas répondu</p>
      </td>
      <td>D1 sera résolu sur V1</td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Aucune modification du nombre d’engagements D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 clique sur D1 et fournit la première réponse.</p>
      </td>
      <td>D1 sera résolu sur V1</td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Le nombre d’engagements pour D1 sera augmenté de 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 clique sur D1 et fournit la première réponse.</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1</p>
        <p>Après l’actualisation, D1 se poursuit.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs et d’engagements pour D1 seront augmentés de 1.</p>
        <p>Après actualisation, aucune modification n’est apportée au nombre.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 clique sur D1, interagit avec le chatterbot et termine D1.</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1</p>
        <p>Après l’actualisation, aucune boîte de dialogue ni dialogue ne sera résolue pour V1.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs, le nombre d’engagements et le nombre terminé pour D1 seront augmentés de 1.</p>
        <p>Après actualisation, aucun dialogue ni dialogue ne sera résolu.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement, WP2</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>La V1 clique sur D1 mais n’a pas répondu</p>
        <p>V1 visites WP2</p>
      </td>
      <td>
        <p>La visite de page WP1, D1 sera résolue sur V1</p>
        <p>Page visit WP2, D1 sera résolu sur V2.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Dans WP2, aucune modification du nombre de déclencheurs D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement, WP2</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 clique sur D1 et est engagé</p>
        <p>V1 visites WP2</p>
      </td>
      <td>
        <p>La visite de page WP1, D1 sera résolue sur V1</p>
        <p>La visite de page WP2, D1 sera résolue sur V1</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs et d’engagements pour D1 seront augmentés de 1.</p>
        <p>Dans WP2, aucune modification n’est apportée à un décompte.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>D2 ciblé pour uniquement WP2</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 clique sur D1 et fournit la première réponse.</p>
        <p>V1 visites WP2</p>
      </td>
      <td>
        <p>D1 sera résolu sur WP1</p>
        <p>D1 continuera V1 sur WP2</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs et d’engagements pour D1 seront augmentés de 1.</p>
        <p>Aucune modification du déclencheur D2 ou du nombre d’engagements</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>D2 ciblé pour uniquement WP2</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>La V1 clique sur D1 mais n’a pas répondu</p>
        <p>V1 visites WP2</p>
      </td>
      <td>D1 sera résolu sur WP1<br/>
      D2 sera résolu sur WP2</td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Le nombre de déclencheurs pour D2 sera augmenté de 1.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>D2 ciblé pour uniquement WP2</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 clique sur D1 et termine D1</p>
        <p>V1 visites WP2</p>
      </td>
      <td>D1 sera résolu sur WP1 et après la fin<br/>D2 sera résolu sur WP2</td>
      <td>
        <p>Le nombre de déclencheurs, le nombre d’engagements et le nombre terminé pour D1 seront augmentés de 1.</p>
        <p>Le nombre de déclencheurs pour D2 sera augmenté de 1.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>D2 ciblé pour uniquement WP2</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 clique sur D1 et termine D1</p>
        <p>V1 visites WP2</p>
        <p>Les clics V1 sur D2 fournissent la première réponse.</p>
      </td>
      <td>D1 sera résolu sur WP1 et après la fin<br/>D2 sera résolu sur WP2</td>
      <td>
        <p>Le nombre de déclencheurs, le nombre d’engagements et le nombre terminé pour D1 seront augmentés de 1.</p>
        <p>Le nombre de déclencheurs et d’engagements pour D2 sera augmenté de 1.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>La V1 clique sur D1 mais n’a pas répondu</p>
        <p>D1 est dépublié</p>
      </td>
      <td>D1 sera résolu sur V1</td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Aucune modification du nombre d’engagements D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>La V1 clique sur D1 mais n’a pas répondu</p>
        <p>D1 est dépublié</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois.</p>
        <p>Une fois l’actualisation terminée, aucune boîte de dialogue ne sera résolue.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Aucune modification du nombre d’engagements D1</p>
        <p>Après actualisation, aucune modification n’est apportée au déclencheur D1 ni au nombre d’engagements.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 engagé avec D1</p>
        <p>D1 est dépublié</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1</p>
        <p>Après l’actualisation, D1 se poursuit.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Le nombre d’engagements D1 sera augmenté de 1</p>
        <p>Après l’actualisation, la D1 sera conservée sans aucune autre modification pour déclencher ou impliquer le nombre</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>La V1 clique sur D1 mais n’a pas répondu</p>
        <p>D1 est publié avec de nouvelles modifications.</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois.</p>
        <p>Après l’actualisation, la dialogue avec les nouvelles modifications sera résolue.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Après actualisation, comme D1 avec de nouvelles modifications, mais sans autre changement pour déclencher le nombre</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 uniquement</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>Les clics V1 sur D1 fournissent la première réponse.</p>
        <p>D1 est publié avec de nouvelles modifications.</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois.</p>
        <p>Après actualisation, le dialogue avec les anciennes modifications se poursuit.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Le nombre d’engagements pour D1 sera augmenté de 1</p>
        <p>Après actualisation, car l’ancien D1 s’affiche, aucun changement ne déclenche le nombre.</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 ciblé pour WP1 avec une priorité 1</p>
        <p>D2 ciblé pour WP1 avec 2 priorités</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>La V1 clique sur D1 mais n’a pas répondu</p>
        <p>D1 est dépublié</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois.</p>
        <p>Après l’actualisation, D2 est résolu sur V1.</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Après actualisation, le nombre de déclencheurs pour D2 est augmenté de 1.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec une priorité 1</p>
        <p>D2 ciblé pour WP1 avec 2 priorités</p>
        <p>V1 visite pour la première fois WP1</p>
        <p>V1 clique sur D1 et termine D1</p>
        <p>V1 actualise WP1 et voir D2<br/>V1 clique sur D2 et termine D2.</p>
        <p>Le marketeur a apporté des modifications à D1 et les a republiées.</p>
        <p>V1 actualise WP1</p>
      </td>
      <td>
        <p>D1 sera résolu sur V1 pour la première fois.</p>
        <p>Après l’actualisation, D2 est résolu sur V1.</p>
        <p>Après avoir terminé D1 et D2, quelles que soient les modifications ou la republication de D1, D2 ne s’affichera plus à V1</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs, le nombre d’engagements et le nombre terminé pour D1 seront augmentés de 1.</p>
        <p>Actualiser une fois D2 terminé, aucune action à effectuer</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec un déclencheur "Temps passé sur le site" de 30 secondes</p>
        <p>V1 visites WP1</p>
      </td>
      <td>
        <p>D1 sera résolu mais ne sera pas déclenché vers V1</p>
        <p>Au bout de 30 secondes, D1 s’affiche/se déclenche sur V1.</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 ne sera augmenté que de 1 après 30 secondes ou plus passées sur la page web.</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1, WP2 avec un déclencheur "Temps passé sur la page" de 30 secondes</p>
        <p>V1 visite WP1, WP2</p>
      </td>
      <td>
        <p>D1 sera résolu mais ne sera pas déclenché vers V1</p>
        <p>Au bout de 30 secondes, D1 s’affiche/se déclenche sur V1.</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 ne sera augmenté que de 1 après 30 secondes ou plus passées sur la page web.</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec un déclencheur "pourcentage de défilement" de 50</p>
        <p>V1 visites WP1</p>
      </td>
      <td>
        <p>D1 sera résolu mais ne sera pas déclenché vers V1</p>
        <p>Après un défilement de 50 %, D1 s’affiche/se déclenche sur V1.</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 ne sera augmenté que de 1 après 50 % de défilement.</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour WP1 avec une priorité 1 et un déclencheur "Temps passé sur la page" de 30 secondes</p>
        <p>D2 ciblé pour WP1 avec 2 priorités et événement "pourcentage de défilement de page" de 50</p>
        <p>V1 visite WP1, après 10 secondes V1 visite WP2, V1 visite WP1</p>
      </td>
      <td>
        <p>Sur WP1, D1 sera résolu mais ne sera pas déclenché sur V1</p>
        <p>Sur WP2, D2 sera résolu mais ne sera pas déclenché sur V1</p>
        <p>Sur WP1, D1 sera résolu et après 20 secondes D1 sera déclenché sur V1</p>
      </td>
      <td>Le nombre de déclencheurs pour D1 ne sera augmenté que de 1 après 30 secondes.</td>
    </tr>
    <tr>
      <td>
        <p>D1 ciblé pour le WP1 avec le déclencheur "Temps passé sur le site" d’une minute</p>
        <p>V1 visite WP1 pendant 1 minute et affiche D1 mais n’engage pas</p>
        <p>La V1 ferme le WP1 et revient au WP1 2 jours plus tard</p>
      </td>
      <td>
        <p>D1 s’affichera automatiquement à V1, car ils ont déjà rempli les critères de déclenchement au cours de la session précédente.</p>
        <p>La même logique s’applique au "temps passé sur la page" et au "pourcentage de défilement de la page".</p>
      </td>
      <td>
        <p>Le nombre de déclencheurs pour D1 sera augmenté de 1</p>
        <p>Après le retour, aucune action à effectuer</p>
      </td>
    </tr>
  </tbody>
</table>

