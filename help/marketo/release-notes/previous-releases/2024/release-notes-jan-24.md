---
description: Notes de mise à jour - Janvier 2024 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Janvier 2024
feature: Release Information
exl-id: 64e85f6c-b746-46b6-ab51-5ad1817396b2
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 6%

---

# Notes de mise à jour : janvier 2024 {#release-notes-jan-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 janvier. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **12 janvier 2024**, avec un déploiement progressif des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr> 
   <td><strong>Webinaires à la demande pour les webinaires interactifs</strong> : les webinaires à la demande vous permettent de publier l’enregistrement des webinaires et de suivre ses visites/montres. Vous obtiendrez ainsi plus de pistes grâce à des inscrits qui n’ont pas assisté au webinaire (pas d’affichage) mais qui sont toujours intéressés par la recherche de plus amples détails et l’affichage de l’enregistrement.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">Webinaires On-Demand</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Pages d’entrée de conversation</strong> : incorporez un flux de conversation de Dynamic Chat directement dans une page d’entrée de Marketo Engage afin que les visiteurs puissent planifier une réunion par l’intermédiaire d’un Dynamic Chat sans avoir à remplir un formulaire ni à interagir avec un chatterbot.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Filtrage de l’activité des robots de messagerie</strong> : améliore la capture de l’activité des robots pour l’engagement des courriers électroniques en vous permettant de choisir l’agressivité du filtrage de l’identification de l’activité des robots.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">Filtrage de l’activité des robots de messagerie</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
    <tr> 
   <td><strong>Mise à jour de l’API d’importation de pistes en bloc</strong> : un ajustement mineur a été apporté au comportement de l’API d’importation de pistes en bloc lorsque <b>id</b> est spécifié comme <b>lookupField</b> lors de la création de la tâche. Si un enregistrement de personne lié au <b>id</b> fourni est introuvable dans la base de données du Marketo Engage, aucune mise à jour d’enregistrement ne se produit, car l’enregistrement est introuvable. Le comportement mis à jour inclut désormais l’incrémentation du nombre dans la propriété <b>numOfRowsFailed</b> dans la réponse, ce qui indique que l’opération a échoué dans de tels cas.</td> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
  <tr> 
   <td><strong>Co-hosts for Interactive Webinars</strong> : les co-hôtes de la section Équipe de webinaires des webinaires interactifs permettent au créateur de l’événement d’ajouter des utilisateurs internes ou externes au programme de webinaires interactifs afin de partager les responsabilités d’administration et de diffusion.</td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md#adding-a-webinar-team" target="_blank">Ajout d’une équipe de webinaires</a></td>
  </tr>
  <tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Supprimer un utilisateur dans les webinaires interactifs</strong> : un administrateur de Marketo Engage peut désormais supprimer un ou plusieurs utilisateurs spécifiques dans les webinaires interactifs.</td> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
 </tbody> 
</table>
<br/>

## Fonctionnalités de version agile {#agile-release-features}

Toutes les fonctionnalités ci-dessous suivent un format Agile et sont publiées à diverses dates avant ou après la date de publication standard. Vérifiez l’état de chaque fonction en regard de celle-ci.

### Actions Sales Insight {#sales-insight-actions}

![(star)](assets/yellow-star.png)

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:15%">Statut</th>
   <th style="width:20%">Documentation</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Fenêtre de composition extensible</strong> : la fenêtre de composition d’email compresse désormais automatiquement l’espace inutilisé, ce qui permet d’avoir plus d’espace dans l’éditeur. De plus, la fenêtre pourra s’ouvrir et s’étendre davantage, donnant aux utilisateurs autant de place qu’ils le doivent pour apporter des modifications à leurs emails.</td> 
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
   <td><strong>Interface utilisateur de Chatbot pour Conversational Forms</strong> : les visiteurs du site web peuvent désormais demander un clic en direct dans un flux de conversation.</td> 
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
   <td><strong>Options de couleur de la police Chatbot</strong> : personnalisez les couleurs de la police dans une configuration de chatbot.</td> 
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
   <td><strong>Option pour répéter le dialogue</strong> : vous pouvez maintenant redémarrer un dialogue au début une fois qu’un visiteur a atteint la fin.</td> 
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
   <td><strong>Arrêt manuel de conversation en direct</strong> : les visiteurs et les agents peuvent désormais mettre fin manuellement à une session de conversation en direct.</td> 
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
   <td><strong>Activités de Marketo Engage récentes dans la boîte de réception de l’agent</strong> : les activités de Marketo Engage récentes, telles que le courrier électronique ouvert et le formulaire rempli, s’affichent pour les pistes dans la boîte de réception de l’agent.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Embranchement conditionnel</strong> : vous pouvez désormais afficher aux visiteurs différents contenus de conversation en fonction de conditions prédéfinies, telles que l’emplacement du visiteur ou la disponibilité de l’agent en direct.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour Liste-désabonnement en un clic** : Gmail et Yahoo ont mis en oeuvre plusieurs nouvelles exigences d’expéditeur qui ont pris effet le 1er février 2024. Découvrez [ce qu&#39;ils sont et comment ils vous affectent](https://nation.marketo.com/t5/employee-blogs/update-support-for-one-click-list-unsubscribe-for-marketo/ba-p/344514#M352){target="_blank"}.

* **Mise à jour de l’API de piste de synchronisation** : le comportement de l’ [API de piste de synchronisation](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"} a été légèrement ajusté pour les mises à jour du champ `unsubscribed`. Désormais, lorsque vous transmettez `null` comme valeur, cela revient à transmettre une valeur de `false`.

* **Marketo Engage Forms jQuery 1.x** : dans notre version de janvier 2024, nous allons mettre à jour jQuery pour Marketo Engage Forms vers jQuery 3.x. Cela peut avoir un impact sur l’implémentation personnalisée du formulaire basée sur des versions plus anciennes de jQuery. [En savoir plus ici](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}.

* **Vérification des e-mails pour les utilisateurs SSO uniquement** : SSO Seuls les utilisateurs étaient automatiquement vérifiés, ce qui leur permettait d’utiliser un compte de messagerie inaccessible. À compter de la mi-janvier, tous les utilisateurs d’authentification unique existants ne seront plus vérifiés et devront vérifier à nouveau leur adresse électronique via un lien que nous envoyons au compte de messagerie. Tous les nouveaux utilisateurs d’authentification unique devront vérifier à l’avenir leurs adresses électroniques.

* Regardez le [Webinaire de mise à jour du Marketo Engage de janvier 2024](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"}.
