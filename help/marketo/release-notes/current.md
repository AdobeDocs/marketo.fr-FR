---
description: Notes de mise à jour actuelles - Documentation de Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 33c67217b57c4dced059488edec9f78d0759e72b
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 7%

---

# Notes de mise à jour : janvier 2024 {#release-notes-jan-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 janvier. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **12 janvier 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr> 
   <td><strong>Webinaires à la demande pour les webinaires interactifs</strong>: les webinaires à la demande vous permettent de publier l’enregistrement du webinaire et de suivre ses visites/montres. Vous obtiendrez ainsi plus de pistes grâce à des inscrits qui n’ont pas assisté au webinaire (pas d’affichage) mais qui sont toujours intéressés par la recherche de plus amples détails et l’affichage de l’enregistrement.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">Webinaires On-Demand</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Pages d’entrée de conversation</strong>: Incorporez un flux de conversation de Dynamic Chat directement dans une page d’entrée de Marketo Engage afin que les visiteurs puissent planifier une réunion par l’intermédiaire d’un Dynamic Chat sans avoir à remplir un formulaire ou interagir avec un chatterbot.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Filtrage de l’activité des robots de messagerie</strong>: améliore la capture de l’activité de robot pour l’engagement email en vous permettant de choisir l’agressivité du filtrage de l’identification de l’activité de robot.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">Filtrage de l’activité des robots de messagerie</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
    <tr> 
   <td><strong>Mise à jour de l’API d’importation de pistes en bloc</strong>: un léger ajustement a été apporté au comportement de l’API Bulk Lead Import lors de la <b>id</b> est spécifié comme <b>lookupField</b> lors de la création de la tâche. Si un enregistrement de personne est lié au <b>id</b> est introuvable dans la base de données du Marketo Engage, aucune mise à jour d’enregistrement ne se produit, car l’enregistrement est introuvable. Le comportement mis à jour inclut désormais l’augmentation du nombre dans la variable <b>numOfRowsFailed</b> dans la réponse, indiquant que l’opération a échoué dans de tels cas.</td> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
  <tr> 
   <td><strong>Co-hôtes pour les webinaires interactifs</strong>: les co-hôtes de la section Équipe de webinaires des webinaires interactifs permettent au créateur d’événements d’ajouter des utilisateurs internes ou externes au programme de webinaires interactifs afin de partager les responsabilités d’administration et de livraison.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md#adding-a-webinar-team" target="_blank">Ajout d’une équipe de webinaires</a></td>
  </tr>
  <tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Suppression d’un utilisateur dans les webinaires interactifs</strong>: un administrateur de Marketo Engage peut désormais supprimer un ou plusieurs utilisateurs spécifiques dans les webinaires interactifs.</td> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
 </tbody> 
</table>
<br/>

## Fonctionnalités de version agile {#agile-release-features}

Toutes les fonctionnalités ci-dessous suivent un format Agile et sont publiées à diverses dates avant ou après la date de publication standard. Vérifiez l’état de chaque fonction en regard de celle-ci.

### Actions d’aperçu commercial {#sales-insight-actions}

![(étoile)](assets/yellow-star.png)

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:15%">Statut</th>
   <th style="width:20%">Documentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Fenêtre de composition extensible</strong>: la fenêtre composer un email compresse désormais automatiquement l’espace inutilisé, ce qui permet d’avoir plus d’espace dans l’éditeur. De plus, la fenêtre pourra s’ouvrir et s’étendre davantage, donnant aux utilisateurs autant de place qu’ils le doivent pour apporter des modifications à leurs emails.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>
  </tbody> 
</table>

### Dynamic Chat {#dynamic-chat}

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:15%">Statut</th>
   <th style="width:20%">Documentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Interface utilisateur de Chatbot pour Conversation Forms</strong>: les visiteurs du site web peuvent désormais demander une conversation en direct dans un flux de conversation.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Options de couleur de police du robot de messagerie</strong>: personnalisez les couleurs de police dans une configuration de chatbot.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Option pour répéter le dialogue</strong>: vous pouvez maintenant redémarrer une Dialogue au début une fois qu’un visiteur a atteint la fin.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Arrêt manuel d’une conversation en direct</strong>: les visiteurs et les agents peuvent désormais mettre fin manuellement à une session de chat en direct.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#end-a-session" target="_blank">Boîte de réception de l’agent(e)</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Activités Marketo Engage récentes dans la boîte de réception de l’agent</strong>: les activités de Marketo Engage récentes, telles que Courrier électronique ouvert et Formulaire rempli, s’affichent pour les pistes dans la boîte de réception de l’agent.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Embranchement conditionnel</strong>: vous pouvez désormais afficher aux visiteurs différents contenus de conversation en fonction de conditions prédéfinies, telles que l’emplacement du visiteur ou la disponibilité de l’agent en direct.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour List-Unsubscribe en un clic**: Gmail et Yahoo ont mis en place plusieurs nouvelles exigences d’expéditeur qui sont entrées en vigueur le 1er février 2024. Formation [ce qu&#39;ils sont et comment ils vous affectent](https://nation.marketo.com/t5/employee-blogs/update-support-for-one-click-list-unsubscribe-for-marketo/ba-p/344514#M352){target="_blank"}.

* **Mise à jour de l’API de piste de synchronisation**: la variable [API de piste de synchronisation](https://developers.marketo.com/rest-api/lead-database/leads/#create_and_update){target="_blank"}Le comportement de a a été légèrement ajusté en ce qui concerne les mises à jour apportées à la variable `unsubscribed` champ . Maintenant, quand vous passez `null` comme valeur, c’est égal à transmettre une valeur de `false`.

* **Marketo Engage Forms jQuery 1.x**: dans notre version de janvier 2024, nous allons mettre à jour jQuery pour Marketo Engage Forms vers jQuery 3.x. Cela peut avoir un impact sur l’implémentation personnalisée du formulaire basée sur des versions plus anciennes de jQuery. [En savoir plus ici](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}.

* **Vérification par e-mail pour les utilisateurs SSO uniquement**: SSO Seuls les utilisateurs étaient automatiquement vérifiés, ce qui leur permettait d’utiliser un compte de messagerie inaccessible. À compter de la mi-janvier, tous les utilisateurs d’authentification unique existants ne seront plus vérifiés et devront vérifier à nouveau leur adresse électronique via un lien que nous envoyons au compte de messagerie. Tous les nouveaux utilisateurs d’authentification unique devront vérifier à l’avenir leurs adresses électroniques.

* Regardez la [Webinaire de mise à jour de janvier 2024 pour les Marketo Engage](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"}.
