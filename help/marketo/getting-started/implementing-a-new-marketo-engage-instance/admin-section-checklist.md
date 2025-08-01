---
description: Configurez la section Admin de votre nouvelle instance Marketo Engage.
title: Bonnes Pratiques Relatives Aux Nouvelles Instances - Liste De Contrôle De La Section Admin
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 6%

---

# Bonnes Pratiques Relatives Aux Nouvelles Instances : Liste De Contrôle De La Section Admin {#new-instance-best-practices-admin-section-checklist}

En tant que nouveau responsable administratif naviguant dans une nouvelle instance de Marketo Engage, appliquez la liste de contrôle ci-dessous pour vous guider tout au long du processus d’implémentation. Comme pour tous ces guides, vous pouvez également [télécharger les listes de contrôle](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) et suivre votre progression.

## Rôles {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rôles</td>
    <td><li>Passez en revue les rôles préconfigurés et vérifiez les autorisations/accès dont dispose chaque rôle.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=fr#create-a-new-role" target="_blank">Créez un nouveau rôle</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=fr#edit-a-role" target="_blank">modifiez les rôles</a> en fonction des besoins de votre organisation.</li>
    <li><a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Affectez des utilisateurs aux rôles appropriés</a>. Les utilisateurs doivent être ajoutés à l’abonnement dans Adobe Admin Console avant d’accorder leurs rôles dans « Rôles ». Reportez-vous à la section Utilisateurs de la liste de contrôle <a href="/help/marketo/getting-started/initial-setup/user-setup.md">Configuration initiale</a>.</li>
    <li>Après avoir affecté les rôles aux utilisateurs, vérifiez le nombre d’utilisateurs par rôle.</li>
    <li>Mettez en œuvre un rôle unique pour chaque utilisateur de l’API afin de faciliter la résolution des problèmes.</li></td>
  </tr>
  <tr>
    <td>Sandbox (le cas échéant)</td>
    <td><li>Consultez les catégories ci-dessus pour votre <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">sandbox</a>.</li></td>
  </tr>
</tbody>
</table>

## Espaces de travail &amp; Divisions {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espaces de travail et partitions (le cas échéant)</td>
    <td><li>Déterminez le nombre d<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=fr" target="_blank">espaces de travail</a> et/ou de partitions dont votre entreprise a besoin et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=fr" target="_blank"> combien d’utilisateurs ont accès à chaque espace de travail</a>.</li>
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
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Paramètres de la campagne intelligente</td>
    <td><li>Ajoutez une <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=fr" target="_blank">restriction sur la taille de la campagne intelligente</a> pour éviter d’envoyer accidentellement par e-mail l’ensemble de la base de données.</li></td>
  </tr>
</tbody>
</table>

## Limites de communication {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limites de communication</td>
    <td><li>Implémentez des <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=fr" target="_blank">limites de communication</a>.</li>
    <li>Déterminez si votre entreprise a besoin d’une politique sur les limites de communication.</li></td>
  </tr>
</tbody>
</table>

## Balises {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canaux</td>
    <td><li>Définissez comment utiliser les <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=fr" target="_blank">canaux</a>.</li></td>
  </tr>
  <tr>
    <td>Balises</td>
    <td><li>Définissez comment utiliser les <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=fr" target="_blank">balises</a>.</li></td>
  </tr>
  <tr>
    <td>Calendrier <br>
    (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=fr" target="_blank">Envoyez des places dans le calendrier marketing</a> aux personnes qui ont besoin d’y accéder.</li>
    <li>Configurez le <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=fr" target="_blank">Calendrier</a>.</li></td>
  </tr>
</tbody>
</table>

## Gestion de la base de données {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gestion des champs</td>
    <td><li>Implémentez une convention de nommage pour les <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=fr" target="_blank"> champs personnalisés </a> (par exemple, en commençant par « MKTO »).</li>
    <li>Soyez sélectif quant aux champs que vous synchronisez. Plus vous synchronisez de champs, plus le cycle de synchronisation est lent.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=fr" target="_blank">Bloquez les mises à jour apportées aux champs</a> vous souhaitez qu’elles soient écrites une seule fois (par exemple, la source de lead d’origine, les détails de la source de lead d’origine, les champs UTM de première touche, etc.).</li></td>
  </tr>
  <tr>
    <td>Activités personnalisées</td>
    <td><li>Définissez des <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=fr" target="_blank">activités personnalisées</a> qui sont spécifiques à votre entreprise.</li></td>
  </tr>
  <tr>
    <td>Objets personnalisés</td>
    <td><li>Vérifiez le nombre <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=fr" target="_blank">d’objets personnalisés</a> dont vous avez besoin.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=fr" target="_blank">Synchronisez ces objets personnalisés</a> avec votre CRM.</li></td>
  </tr>
</tbody>
</table>

## Intégrations {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
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
    <td><li>Déterminez les utilisateurs/applications qui peuvent effectuer des appels <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=fr" target="_blank">API</a> dans votre instance.</li>
    <li>Passez en revue toutes les applications qui effectueront des appels API et déterminez si une augmentation ou une diminution des appels API est nécessaire.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Configurez les services <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=fr" target="_blank">LaunchPoint</a> pour votre entreprise. Chaque point de lancement doit être associé à un utilisateur d’API unique pour faciliter la résolution des problèmes.</li></td>
  </tr>
  <tr>
    <td>Webinaires interactifs (le cas échéant)</td>
    <td><li>Pour créer des webinaires interactifs, la fonctionnalité de webinaire intégrée de Marketo Engage, <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">ajoutez des utilisateurs à la section « Utilisateur »</a> dans l’onglet Webinaire interactif .</li>
    <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : les webinaires interactifs ne sont configurés que pour les instances de production.</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (le cas échéant)</td>
    <td><li>Affectez des utilisateurs aux rôles <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">'Accéder à Dynamic Chat'</a> dans Marketo Engage &gt; Admin &gt; Utilisateurs et rôles.</li></td>
  </tr>
  <tr>
    <td>Insight de vente (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Configurer l’action Sales Insight</a> dans Sales Insight &gt; Configuration des actions.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=fr#invite-individual-users-to-msi-actions" target="_blank">Attribuer des places</a> aux utilisateurs appropriés.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=fr" target="_blank">Configurez l’API</a>.</li>
    <li>Personnalisez les <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=fr" target="_blank">scores de prospect</a>.</li></td>
  </tr>
  <tr>
    <td>Connexion Ventes (le cas échéant)</td>
    <td><li>Invitez les administrateurs Marketo Engage appropriés dans l’instance <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">Sales Connect</a>.</li>
    <li>Effectuez la <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank"> configuration supplémentaire d’administration de Sales Connect </a> dans Sales Connect et Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhooks (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=fr" target="_blank">Créez tous les Webhooks requis</a> pour votre entreprise.</li>
    </td>
  </tr>
</tbody>
</table>

## Coffre au trésor {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=fr" target="_blank">Activez l’Inspecteur de campagne</a> pour afficher toutes vos campagnes intelligentes en un seul endroit.</li></td>
  </tr>
</tbody>
</table>
