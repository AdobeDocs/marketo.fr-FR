---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour de Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: ce7142e471271dfb33b265e226b67bcc3b35594b
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 4%

---

# Notes de mise à jour de Dynamic Chat {#dynamic-chat-release}

Les versions de Adobe Dynamic Chat fonctionnent sur un modèle de diffusion continu, ce qui permet une approche plus évolutive du déploiement des fonctionnalités. Il arrive qu’il y ait plusieurs versions par mois. N’hésitez pas à vérifier régulièrement pour obtenir les informations les plus récentes.

La page Notes de mise à jour standard de Marketo Engage [se trouve ici](/help/marketo/release-notes/current.md){target="_blank"}.

## Version de juin 2025 {#june-25-release}

### Réorganisation de la logique de routage {#routing-logic-revamp}

Nous avons repensé la logique de routage du chat en direct dans Dynamic Chat pour garantir un comportement d’engagement plus intelligent et plus prévisible pour tous les types de routage (compte, personnalisé, équipe et cycle de rotation). La nouvelle logique simplifie les flux de routage et améliore la gestion de secours lorsque des agents ne sont pas disponibles.

#### Améliorations clés du comportement de routage

* **Jusqu’à deux tentatives d’engagement par session**

   * Le système tente de se connecter à au plus deux agents, mais strictement dans la règle de routage principale.

   * Si un agent est disponible mais ne répond pas (par exemple, il est refusé ou manquant), le système tente d&#39;obtenir un second agent du même pool.

   * La logique de secours (comme la rotation) n’est activée que si aucun agent éligible n’est trouvé lors de la résolution initiale, et non pour réessayer après un échec de l’engagement.

* **Comportement Spécifique Aux Règles De Routage**

_**Routage de compte**_

Si le domaine d’e-mail d’un visiteur est mappé à un compte connu, l’agent mappé est toujours considéré comme prioritaire.

Si l’agent est disponible, le chat leur est directement adressé.

Si l’agent n’est pas disponible, le système :

Ne tente pas d&#39;utiliser un autre agent, même si Round Robin est activé comme solution de secours.

Au lieu de cela, il :

Affiche le calendrier de réunion de l&#39;agent mappé (si activé), ou

Retourne à un message par défaut (au pire des cas).

La règle de routage au niveau de la carte (par exemple, Équipe, Personnalisé) n’est prise en compte que si le routage de compte n’est pas éligible (aucun domaine ou agent correspondant).

_**Routage personnalisé/d’équipe**_

Ces règles peuvent renvoyer plusieurs agents éligibles.

Si le premier agent disponible n&#39;engage pas, le système essaie un autre agent de la même liste.

La solution de secours Round Robin n’est pas déclenchée simplement parce qu’un agent n’a pas répondu.

Si aucun des agents n’engage :

Le système affiche le calendrier du premier agent essayé (s&#39;il est activé), ou

Affiche le message de secours par défaut.

_**Routage circulaire**_

Lorsqu&#39;il est utilisé comme règle de transmission principale, le système :

Tente d&#39;engager le premier agent disponible à partir du pool circulaire.

Si le premier ne répond pas, il réessaye avec le meilleur agent éligible suivant.

Si la fonction Round Robin est utilisée comme solution de secours, elle s’active uniquement si aucun agent n’est résolu à partir de la règle principale.

**Flux d’expérience du visiteur**

Le système vérifie si le routage de compte est applicable.

Si oui, et l’agent est disponible, → se connecte immédiatement.

Si non éligible ou agent indisponible, → passe à la règle de routage au niveau de la carte.

La règle de routage au niveau de la carte (personnalisée, d’équipe, à tour de rôle) est évaluée.

La disponibilité (autorisations, statut) des agents éligibles est vérifiée.

Le système engage un agent et, si nécessaire, tente un deuxième agent à partir de la même règle.

Si aucun engagement ne réussit, → logique de secours est appliquée :

Calendrier de secours (si activé), ou

Message par défaut.

La solution de secours Round Robin n’est prise en compte que lorsqu’aucun agent éligible n’est trouvé dans la règle de routage principale, et non lorsque des agents individuels ne répondent pas.

**Cas d’utilisation**

Routage de compte

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>Le domaine du visiteur est mappé à un compte ; le chat en direct est activé pour l’agent mappé et il est disponible</td>
    <td>La conversation se connecte directement à l’agent mappé</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>L’agent mappé n’est pas disponible, la solution de secours arrondie est activée</td>
    <td>Le système sélectionne un agent disponible par rotation et l’engage </td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>L'agent mappé n'est pas disponible, pas de solution de secours Round Robin ; la réservation de réunion est activée</td>
    <td>Le système affiche le calendrier de l’agent mappé ou affiche un message de secours par défaut</td>
  </tr>
</tbody></table>

Routage personnalisé

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
</tbody></table>

Routage d&#39;équipe

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
</tbody></table>

Routage circulaire

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>TEXTE</td>
    <td>TEXTE</td>
  </tr>
</tbody></table>

### Notification Pulse {#pulse-notification}

Chaque fois qu’un visiteur demande à se connecter à un agent, nous lui fournissons aujourd’hui une notification de navigateur in-app, mais les agents ne participent souvent pas à ces conversations.

* Désormais, l’agent en direct recevra un e-mail, un Slack, une inapp et une notification du navigateur lorsqu’un nouveau visiteur souhaite discuter

* Le contenu des notifications Pulse peut être identique à celui que nous utilisons aujourd’hui pour les notifications in-app dans le navigateur

Le comportement doit être le même que celui actuel pour que l’agent accepte lorsque plusieurs agents acceptent.
