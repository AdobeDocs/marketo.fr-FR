---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour de Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 0a7e5cc9-f2a6-4721-bbdc-661249a2e2b6
source-git-commit: d646dbb2eeeb7ec6e1dbeb30d1fa02aa380a794c
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 3%

---

# Notes de mise à jour de Dynamic Chat {#dynamic-chat-release}

Les versions de Adobe Dynamic Chat fonctionnent sur un modèle de diffusion continu, ce qui permet une approche plus évolutive du déploiement des fonctionnalités. Il arrive qu’il y ait plusieurs versions par mois. N’hésitez pas à vérifier régulièrement pour obtenir les informations les plus récentes.

La page Notes de mise à jour standard de Marketo Engage [se trouve ici](/help/marketo/release-notes/current.md){target="_blank"}.

## Version de juin 2025 {#june-2025-release}

### Réorganisation de la logique de routage {#routing-logic-revamp}

Nous avons repensé la logique de routage du chat en direct dans Dynamic Chat pour garantir un comportement d’engagement plus intelligent et plus prévisible pour tous les types de routage (compte, personnalisé, équipe et cycle de rotation). La nouvelle logique simplifie les flux de routage et améliore la gestion de secours lorsque des agents ne sont pas disponibles.

#### Améliorations clés du comportement de routage

* **Jusqu’à deux tentatives d’engagement par session**

   * Le système tente de se connecter à un maximum de deux agents (au plus), mais strictement dans la règle de routage principale.

   * Si un agent est disponible mais ne répond pas (par exemple, refuse ou manque la conversation), le système tentera de se connecter à un agent différent du même pool.

   * La logique de secours (comme la rotation) n’est activée que si aucun agent éligible n’est trouvé lors de la résolution initiale, et non pour réessayer après un échec de l’engagement.

* **Comportement Spécifique Aux Règles De Routage**

_&#x200B;**Routage de compte**&#x200B;_

Si le domaine d’e-mail d’un visiteur est mappé à un compte connu, l’agent mappé est toujours considéré comme prioritaire.

Si l’agent est disponible, le chat leur est directement adressé.

Si l’agent n’est pas disponible, le système :

* Ne tente pas d&#39;utiliser un autre agent, même si Round Robin est activé comme solution de secours.

* Au lieu de cela, il :

   * Affiche le calendrier de réunion de l&#39;agent mappé (si activé),
-ou-
   * Retourne à un message par défaut (au pire des cas).

La règle de routage au niveau de la carte (par exemple, Équipe, Personnalisé) n’est prise en compte que si le routage de compte n’est pas éligible (aucun domaine ou agent correspondant).

_&#x200B;**Routage personnalisé/d’équipe**&#x200B;_

Ces règles peuvent renvoyer plusieurs agents éligibles.

Si le premier agent disponible n&#39;engage pas, le système essaie un autre agent de la même liste.

La solution de secours Round Robin n’est pas déclenchée simplement parce qu’un agent ne répond pas.

Si aucun des agents n’engage :

* Le système affiche le calendrier du premier agent essayé (s&#39;il est activé),
-ou-
* Affiche le message de secours par défaut.

_&#x200B;**Routage circulaire**&#x200B;_

Lorsqu&#39;il est utilisé comme règle de transmission principale, le système :

* Tente d&#39;engager le premier agent disponible à partir du pool circulaire.

* Si le premier agent ne répond pas, il réessaye avec le meilleur agent éligible suivant.

Si la fonction Round Robin est utilisée comme solution de secours, elle s’active uniquement si aucun agent n’est résolu à partir de la règle principale.

_&#x200B;**Flux d’expérience du visiteur**&#x200B;_

Le système vérifie si le routage de compte est applicable.

* Si oui et que l’agent est disponible, il se connecte immédiatement.

* Si l’agent n’est pas éligible ou indisponible, il passe à la règle de routage au niveau de la carte.

La règle de routage au niveau de la carte (personnalisée, d’équipe, à tour de rôle) est évaluée.

* La disponibilité (autorisations, statut) des agents éligibles est vérifiée.

* Le système engage un agent et, si nécessaire, tente un deuxième agent à partir de la même règle.

* Si aucun engagement ne réussit, une logique de secours est appliquée :

   * Calendrier de secours (si activé),
-ou-
   * Message par défaut.

La solution de secours Round Robin n’est prise en compte que lorsqu’aucun agent éligible n’est trouvé dans la règle de routage principale, et non lorsque des agents individuels ne répondent pas.

##### Cas d’utilisation {#use-cases}

_&#x200B;**Routage de compte**&#x200B;_

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

_&#x200B;**Routage personnalisé**&#x200B;_

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>La logique personnalisée résout une liste d’agents ; le premier agent est disponible et accepte la conversation.</td>
    <td>La conversation se connecte au premier agent.</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>La règle personnalisée ne résout aucun agent, la fonction de secours Round Robin est activée.</td>
    <td>Le système sélectionne un agent disponible par rotation et l’engage.</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>Deux agents ont été résolus ; aucun d'eux n'accepte la conversation, la solution de secours définie sur le calendrier de réunion.</td>
    <td>Le calendrier de l’agent qui a été essayé pour la première fois s’affiche ou un message de secours par défaut s’affiche.</td>
  </tr>
</tbody></table>

_&#x200B;**Routage de l&#39;équipe**&#x200B;_

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>L’équipe comprend des agents qui utilisent le chat en direct ; le premier agent disponible accepte le chat.</td>
    <td>La conversation se connecte à cet agent.</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>Aucun agent d'équipe n'est disponible et la solution de secours circulaire est activée.</td>
    <td>Le système sélectionne et se connecte à un agent du pool Round Robin.</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>Deux agents disponibles, mais aucun ne s’engage ; calendrier de secours activé.</td>
    <td>Le calendrier de l’agent qui a été tenté pour la première fois s’affiche ou un message de secours est déclenché.</td>
  </tr>
</tbody></table>

_&#x200B;**Routage circulaire**&#x200B;_

<table><thead>
  <tr>
    <th>Type</th>
    <th>Exemple</th>
    <th>Résultat</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Idéal</td>
    <td>Round Robin pool a plusieurs agents ; le second agent accepte le chat après le premier ne l'accepte pas.</td>
    <td>La conversation se connecte au second agent.</td>
  </tr>
  <tr>
    <td>Secours (à tour de rôle)</td>
    <td>Aucun agent disponible dans le pool Round Robin ; le calendrier des réunions est activé.</td>
    <td>Le calendrier s’affiche pour le premier agent de la liste (s’il est configuré) ou un message de secours s’affiche.</td>
  </tr>
  <tr>
    <td>Aucun agent de secours</td>
    <td>Aucun agent disponible ; la solution de secours est désactivée.</td>
    <td>Un message de secours statique s’affiche pour le visiteur.</td>
  </tr>
</tbody></table>

### Notification Pulse {#pulse-notification}

Chaque fois qu’un visiteur demande à se connecter à un agent, nous lui fournissons une notification in-app via le navigateur. Mais parfois, les agents ratent ces conversations.

Avec cette version, l’agent en direct peut obtenir une notification par e-mail, Slack, in-app et par navigateur lorsqu’un nouveau visiteur souhaite discuter.

1. Sur la page d’accueil de Adobe Experience Cloud, cliquez sur l’icône Compte et sélectionnez **Préférences**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Faites défiler jusqu’à _Notifications_ et effectuez vos sélections Dynamic Chat souhaitées.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Le contenu d’une notification Pulse peut être le même que celui que nous utilisons pour les notifications in-app dans le navigateur.
