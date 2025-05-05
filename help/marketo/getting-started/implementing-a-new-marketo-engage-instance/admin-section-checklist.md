---
description: Configurez la section Admin pour votre nouvelle instance de Marketo Engage.
title: Bonnes pratiques relatives aux nouvelles instances - Liste de contrôle des sections d’administration
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 6%

---

# Bonnes pratiques relatives aux nouvelles instances : liste de contrôle des sections d’administration {#new-instance-best-practices-admin-section-checklist}

En tant que nouvel administrateur naviguant dans une nouvelle instance de Marketo Engage, appliquez la liste de contrôle ci-dessous pour vous aider à accomplir le processus de mise en oeuvre. Comme avec tous ces guides, vous pouvez également [télécharger les listes de contrôle](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) et suivre votre progression.

## Rôles {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rôles</td>
    <td><li>Vérifiez les rôles prédéfinis et vérifiez les autorisations/accès à chaque rôle.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=fr#create-a-new-role" target="_blank">Créez un nouveau rôle</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=fr#edit-a-role" target="_blank">modifiez les rôles</a> en fonction des besoins de votre entreprise.</li>
    <li><a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Affectez des utilisateurs aux rôles appropriés</a>. Les utilisateurs doivent être ajoutés à l’abonnement dans Adobe Admin Console avant d’accorder leurs rôles dans "Rôles". Reportez-vous à la section Utilisateurs de la <a href="/help/marketo/getting-started/initial-setup/user-setup.md">liste de contrôle Configuration initiale</a>.</li>
    <li>Après avoir affecté les rôles des utilisateurs, passez en revue le nombre d’utilisateurs par rôle.</li>
    <li>Implémentez un rôle unique pour chaque utilisateur de l’API pour faciliter la résolution des problèmes.</li></td>
  </tr>
  <tr>
    <td>Environnement de test (le cas échéant)</td>
    <td><li>Passez en revue les catégories ci-dessus pour votre <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">sandbox</a>.</li></td>
  </tr>
</tbody>
</table>

## Espaces de travail &amp; Divisions {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espaces de travail et partitions (le cas échéant)</td>
    <td><li>Déterminez le nombre d'<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=fr" target="_blank"> espaces de travail</a> et/ou partitions dont votre organisation a besoin et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=fr" target="_blank"> combien d'utilisateurs ont accès à chaque espace de travail.</a></li>
    <li>Définissez l’objectif principal de chaque espace de travail et partition.</li>
    <li>Définissez la relation entre vos espaces de travail et vos partitions.</li></td>
  </tr>
</tbody>
</table>

## Paramètres de la campagne intelligente {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Paramètres de la campagne intelligente</td>
    <td><li>Ajoutez une <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=fr" target="_blank">restriction sur la taille de campagne dynamique</a>, afin d’éviter tout envoi accidentel par courrier électronique de l’ensemble de votre base de données.</li></td>
  </tr>
</tbody>
</table>

## Limites de communication {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limites de communication</td>
    <td><li>Mettez en oeuvre les <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=fr" target="_blank">limites de communication</a>.</li>
    <li>Déterminez si votre entreprise a besoin d’une stratégie sur les limites de communication.</li></td>
  </tr>
</tbody>
</table>

## Balises {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canaux</td>
    <td><li>Définissez comment utiliser <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=fr" target="_blank">channels</a>.</li></td>
  </tr>
  <tr>
    <td>Balises</td>
    <td><li>Définissez comment utiliser <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=fr" target="_blank">tags</a>.</li></td>
  </tr>
  <tr>
    <td>Calendrier<br> 
    (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=fr" target="_blank"> Posséder des sièges dans le calendrier marketing</a> à ceux qui doivent y avoir accès.</li>
    <li>Configurez le <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=fr" target="_blank">calendrier</a>.</li></td>
  </tr>
</tbody>
</table>

## Gestion de la base de données {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gestion des champs</td>
    <td><li>Mettez en oeuvre une convention d’affectation des noms pour les <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=fr" target="_blank">champs personnalisés</a> (par exemple, commençant par "MKTO").</li>
    <li>Soyez sélectif au sujet des champs que vous synchronisez. Plus vous synchronisez de champs, plus le cycle de synchronisation sera lent.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=fr" target="_blank">Bloquez les mises à jour des champs</a> que vous souhaitez écrire à une seule fois (par exemple, source de piste d’origine, détails de source de piste d’origine, champs de gestion dynamique des balises Première touche, etc.).</li></td>
  </tr>
  <tr>
    <td>Activités personnalisées</td>
    <td><li>Définissez des <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=fr" target="_blank">activités personnalisées</a> spécifiques à votre entreprise.</li></td>
  </tr>
  <tr>
    <td>Objets personnalisés</td>
    <td><li>Examinez le nombre d’ <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=fr" target="_blank">objets personnalisés</a> dont vous avez besoin.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=fr" target="_blank">Synchronisez ces objets personnalisés</a> avec votre gestion de la relation client.</li></td>
  </tr>
</tbody>
</table>

## Intégrations {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>Identifiez les autorisations dont vous avez besoin pour accéder à votre CRM.</li>
    <li>Identifiez votre administrateur CRM pour le dépannage.</li></td>
  </tr>
  <tr>
    <td>Services Web</td>
    <td><li>Déterminez les utilisateurs/applications pouvant effectuer des <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=fr" target="_blank">appels API</a> dans votre instance.</li>
    <li>Examinez toutes les applications qui effectueront des appels API et déterminez si une augmentation ou une diminution des appels API est nécessaire.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Configurez les services <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=fr" target="_blank">LaunchPoint</a> pour votre entreprise. Chaque point LaunchPoint doit être associé à un utilisateur d’API unique pour faciliter la résolution des problèmes.</li></td>
  </tr>
  <tr>
    <td>Webinaires interactifs (le cas échéant)</td>
    <td><li>Pour créer des webinaires interactifs, la fonction de webinaire intégrée au Marketo Engage, <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank"> ajoutez des utilisateurs à la section "Utilisateur"</a> sur l’onglet Webinaire interactif.</li>
    <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : les webinaires interactifs ne sont configurés que pour les instances de production.</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (le cas échéant)</td>
    <td><li>Affectez des utilisateurs aux rôles <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">'Access Dynamic Chat' </a> dans Marketo Engage &gt; Admin &gt; Utilisateurs et rôles.</li></td>
  </tr>
  <tr>
    <td>Sales Insight (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Configurez l’action Sales Insight</a> dans Sales Insight &gt; Actions Config.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=fr#invite-individual-users-to-msi-actions" target="_blank">Attribuez des sièges</a> aux utilisateurs appropriés.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=fr" target="_blank">Configurez l’API</a>.</li>
    <li>Personnalisez les <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=fr" target="_blank">scores de piste</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect (le cas échéant)</td>
    <td><li>Invitez les administrateurs de Marketo Engage appropriés à l’ <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">instance de Sales Connect</a>.</li>
    <li>Effectuez la <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">configuration d’administration supplémentaire de Sales Connect</a> dans Sales Connect et Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhooks (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=fr" target="_blank">Créez tous les webhooks requis</a> pour votre entreprise.</li>
    </td>
  </tr>
</tbody>
</table>

## Coffre au trésor {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Coffre au trésor </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=fr" target="_blank">Activez Treasure Chest</a> pour tester les fonctionnalités de pilotage.</li>
    <li>Déterminez les fonctionnalités que vous souhaitez activer ou désactiver.</li></td>
  </tr>
  <tr>
    <td>Inspecteur de campagne </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=fr" target="_blank">Activez l’Inspecteur de campagne</a> pour afficher toutes vos campagnes intelligentes à un seul endroit.</li></td>
  </tr>
</tbody>
</table>
