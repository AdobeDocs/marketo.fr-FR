---
description: Notes De Mise À Jour - Janvier 2024 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour – Janvier 2024
feature: Release Information
exl-id: 64e85f6c-b746-46b6-ab51-5ad1817396b2
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 18%

---

# Notes de mise à jour : janvier 2024 {#release-notes-jan-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 janvier. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 12 janvier 2024**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr>
   <td><strong>Webinaires à la demande pour les webinaires interactifs</strong> : les webinaires à la demande vous permettent de publier l’enregistrement du webinaire et de suivre ses visites/vidéos. Cela vous aidera à obtenir plus de leads par l’intermédiaire des inscrits qui n’ont pas assisté au webinaire (sans participation), mais qui sont toujours intéressés à obtenir plus de détails et à visionner l’enregistrement.</td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">Webinaires à la demande</a></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Pages de destination de conversation</strong> : incorporez un flux de conversation Dynamic Chat directement dans une page de destination Marketo Engage afin que les visiteurs puissent planifier une réunion via Dynamic Chat sans avoir à remplir un formulaire ou à interagir avec un bot conversationnel.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Filtrer l’activité de robot d’e-mail</strong> : améliore la capture de l’activité de robot pour l’engagement des e-mails en vous permettant de choisir le niveau d’agressivité du filtrage d’identification des activités de robot.</td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">Filtrage de l’activité des robots dans les e-mails</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
   </tr>
    <tr>
   <td><strong>Mise à jour de l’API d’importation de leads en bloc</strong> : un ajustement mineur a été apporté au comportement de l’API d’importation de leads en bloc lorsque <b>id</b> est spécifié comme <b>lookupField</b> lors de la création de la tâche. Si un enregistrement de personne lié à l’<b>id</b> fourni est introuvable dans la base de données Marketo Engage, aucune mise à jour d’enregistrement ne se produit, car l’enregistrement ne peut pas être localisé. Le comportement mis à jour inclut désormais l’incrémentation du nombre dans la propriété <b>numOfRowsFailed</b> au sein de la réponse, ce qui signale l’échec de l’opération dans de tels cas.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
   </tr>
  <tr>
   <td><strong>Co-hôtes pour les webinaires interactifs </strong> : les co-hôtes dans la section Équipe de webinaires des webinaires interactifs permettent au créateur de l’événement d’ajouter des utilisateurs internes ou externes au programme de webinaires interactifs pour partager les responsabilités administratives et de diffusion.</td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md#adding-a-webinar-team" target="_blank">Ajout d’une équipe de webinaires</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Supprimer un utilisateur dans les webinaires interactifs</strong> : un administrateur Marketo Engage peut désormais supprimer un ou plusieurs utilisateurs spécifiques dans les webinaires interactifs.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
 </tbody>
</table>
<br/>

## Fonctionnalités de mise à jour d’Agile {#agile-release-features}

Toutes les fonctionnalités ci-dessous suivent un format Agile et sont publiées à différentes dates avant ou après la date de publication standard. Vérifiez le statut en regard de chaque fonctionnalité.

### Actions Sales Insight {#sales-insight-actions}

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
   <td><strong>Fenêtre de composition extensible</strong> : la fenêtre de composition d’e-mail compresse désormais automatiquement l’espace inutilisé, ce qui permet d’avoir plus d’espace dans l’éditeur. De plus, la fenêtre pourra s’afficher et s’agrandir davantage, donnant aux utilisateurs autant d’espace que nécessaire pour apporter des modifications à leurs e-mails.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
 </tbody>
</table>
<br/>
  </tbody>
</table>

### Dynamic Chat {#dynamic-chat}

<table style="border: 0px">
 <tbody>
  <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:15%">Statut</th>
   <th style="width:20%">Documentation</th>
  </tr>
  </tr>
    <tr>
   <td><strong>Interface utilisateur du bot conversationnel pour le Forms de conversation</strong> : les visiteurs du site Web peuvent désormais demander une conversation en direct dans un flux de conversation.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr>
   <td><strong>Options de couleur de police du bot conversationnel</strong> : personnalisez les couleurs de police dans une configuration de bot conversationnel.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr>
   <td><strong>Option de répétition de la boîte de dialogue</strong> : vous pouvez désormais redémarrer une boîte de dialogue au début une fois qu’un visiteur a atteint la fin.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr>
   <td><strong>Résiliation manuelle du chat en direct</strong> : les visiteurs et les agents peuvent désormais mettre fin manuellement à une session de chat en direct.</td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#end-a-session" target="_blank">Boîte de réception de l’agent ou de l’agente</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr>
   <td><strong>Activités Marketo Engage récentes dans la boîte de réception de l’agent</strong> : les activités Marketo Engage récentes, telles que l’e-mail ouvert et le formulaire rempli, s’affichent pour les prospects dans la boîte de réception de l’agent.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Branchement conditionnel</strong> : vous pouvez désormais montrer aux visiteurs différents contenus de conversation en fonction de conditions prédéfinies, telles que l’emplacement du visiteur ou la disponibilité de l’agent actif.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
 </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Mise à jour en un clic List-Unsubscribe** : Gmail et Yahoo ont mis en œuvre plusieurs nouvelles exigences relatives aux expéditeurs qui sont entrées en vigueur le 1er février 2024. Découvrez [ce qu’elles sont et comment elles vous affectent](https://nation.marketo.com/t5/employee-blogs/update-support-for-one-click-list-unsubscribe-for-marketo/ba-p/344514#M352){target="_blank"}.

* **Mise à jour de l’API de lead de synchronisation** : le comportement de l’[API de lead de synchronisation](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"} a été légèrement modifié concernant les mises à jour du champ `unsubscribed`. Désormais, lorsque vous transmettez `null` comme valeur, cela équivaut à transmettre une valeur de `false`.

* **Marketo Engage Forms jQuery 1.x** : dans notre version de janvier 2024, nous mettrons à jour jQuery pour Marketo Engage Forms vers jQuery 3.x. Cela peut avoir un impact sur l’implémentation des formulaires personnalisés reposant sur des versions plus anciennes de jQuery. [En savoir plus ici](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}.

* **Vérification des e-mails pour les utilisateurs SSO uniquement** : les utilisateurs SSO uniquement étaient automatiquement vérifiés, ce qui leur permettait d’utiliser un compte de messagerie inaccessible. À compter de la mi-janvier, tous les utilisateurs SSO uniquement existants ne seront plus vérifiés et devront vérifier à nouveau leur adresse e-mail via un lien que nous envoyons au compte de messagerie. Tous les nouveaux utilisateurs SSO uniquement devront à l’avenir vérifier leurs adresses e-mail.

* Regardez le [Webinaire de mise à jour de janvier 2024 de Marketo Engage](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"}.
