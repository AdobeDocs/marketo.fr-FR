---
description: NOUVELLE ZONE - Documents Marketo - Documentation du produit
title: NOUVELLE ZONE
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 5%

---

# NOUVELLE ZONE : Liste de contrôle de l’administrateur {#new-area-admin-checklist}

Texte d’introduction.

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
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Création d’un nouveau rôle</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">modification des rôles</a> selon les besoins de votre entreprise.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html%22%20/l%20%22assign-roles-to-a-user" target="_blank">Affecter des utilisateurs aux rôles appropriés</a>. Les utilisateurs doivent être ajoutés à l’abonnement dans Adobe Admin Console avant d’accorder leurs rôles dans les rôles. Reportez-vous à la section "Utilisateurs" de la liste de contrôle "Configuration initiale" [LIEN].</li>
    <li>Après avoir affecté les rôles des utilisateurs, passez en revue le nombre d’utilisateurs par rôle.</li>
    <li>Implémentez un rôle unique pour chaque utilisateur de l’API pour faciliter la résolution des problèmes.</li></td>
  </tr>
  <tr>
    <td>Documentation</td>
    <td><li>Définissez les utilisateurs et les rôles de votre organisation.</li>
    <li>Définissez votre processus d’ajout d’un nouvel utilisateur/administrateur.</li></td>
  </tr>
  <tr>
    <td>Environnement de test (le cas échéant)</td>
    <td><li>Vérifiez les catégories ci-dessus pour votre <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md">sandbox</a>.</li></td>
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
    <td><li>Déterminer le nombre de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> espaces de travail</a> et/ou partitions dont votre organisation a besoin et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">combien d’utilisateurs ont accès à chaque espace de travail.</a></li>
    <li>Définissez l’objectif principal de chaque espace de travail et partition.</li>
    <li>Définissez la relation entre vos espaces de travail et vos partitions.</li></td>
  </tr>
  <tr>
    <td>Documentation</td>
    <td><li>Documentez comment les espaces de travail sont définis et comment cela se rapporte aux partitions de base de données (par exemple, un espace de travail global qui montre tout le monde par rapport aux secteurs d’activité).</li>
    <li>Importez de nouveaux enregistrements dans la partition appropriée.</li>
    <li>Définissez la valeur dans votre CRM qui place les utilisateurs dans la partition appropriée.</li></td>
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
    <td><li>Ajouter un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">restriction sur la taille de campagne dynamique</a>, empêchant tout envoi accidentel par courrier électronique de l’ensemble de votre base de données.</li></td>
  </tr>
</tbody>
</table>

## Paramètres d’e-mail {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Valeurs par défaut des emails</td>
    <td><li>Sous Domaine de marque, sélectionnez votre domaine et ajoutez votre CNAME de messagerie. Cette valeur doit être au format suivant : [EmailTrackingCNAME].[CompanyDomain].com.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Contacter le support Marketo</a> pour la sécuriser avec une configuration de certificat SSL. Ce processus peut prendre jusqu’à 3 jours ouvrables.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">Configuration de SPF et DKIM</a> pour la délivrabilité des emails.</li></td>
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
    <td><li>Lancer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">limites de communication</a>.</li>
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
    <td><li>Définition de l’utilisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank">channels</a>.</li></td>
  </tr>
  <tr>
    <td>Balises</td>
    <td><li>Définition de l’utilisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank">tags</a>.</li></td>
  </tr>
  <tr>
    <td>Calendrier (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank">Assertions du calendrier marketing des problèmes</a> à ceux qui ont besoin d’accès.</li>
    <li>Configurez la variable <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank">Calendrier</a>.</li></td>
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
    <td><li>Mise en oeuvre d’une convention d’affectation des noms pour <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">champs personnalisés</a> (par exemple, en commençant par "MKTO").</li>
    <li>Soyez sélectif au sujet des champs que vous synchronisez. Plus vous synchronisez de champs, plus le cycle de synchronisation sera lent.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Bloquer les mises à jour des champs</a> vous souhaitez écrire une seule fois (par exemple, source de piste d’origine, détails de source de piste d’origine, champs UTM Première touche, etc.).</li></td>
  </tr>
  <tr>
    <td>Activités personnalisées</td>
    <td><li>Définir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">Activités personnalisées</a> qui sont spécifiques à votre entreprise.</li></td>
  </tr>
  <tr>
    <td>Objets personnalisés</td>
    <td><li>Vérifiez combien de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">Objets personnalisés</a> vous avez besoin.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">Synchroniser ces objets personnalisés avec votre gestion de la relation client</a>.</li></td>
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
    <td><li>Lancer la synchronisation CRM. Choisissez l’un des éléments suivants, en fonction du CRM utilisé par votre entreprise : <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>.</li>
    <li>Identifiez le type d'accès dont vous avez besoin pour accéder à votre CRM.</li>
    <li>Identifiez votre administrateur CRM pour le dépannage.</li></td>
  </tr>
  <tr>
    <td>Pages de destination</td>
    <td>REMARQUE : Êtes-vous un client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d’instructions de configuration informatique pendant votre appel de lancement. <br>Configurez votre domaine de landing page avec un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">CNAME</a> et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">saisir les informations sur le domaine et la page ;</a>. Cela doit être au format : [LandingPageCNAME].[CompanyDomain].com <br>Sélectionnez un CNAME pour vos landing pages. Quelques exemples : <br>* **go**.[CompanyDomain].com <br>* **www2**.[CompanyDomain].com <br>* **lp**.[CompanyDomain].com <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console">Contacter le support Marketo</a> pour lancer le processus de configuration d’un certificat SSL. Ce processus peut prendre jusqu’à 3 jours ouvrables. <br>CONSEIL : Gardez-le court ! Les URL plus courtes sont plus faciles à mémoriser. Nous suggérons "go" comme domaine. <br>Ajoutez le code de suivi Analytics (par exemple, Google Analytics ou Adobe Analytics) aux modèles de page d’entrée. </td>
  </tr>
  <tr>
    <td>Munchkin</td>
    <td>REMARQUE : Si vous êtes client du Launch Pack, ignorez cette étape. Votre consultant vous fournira des instructions de code Munchkin dans votre document d’instructions de configuration informatique.
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html">Ajout du code de suivi Munchkin</a> à votre site web. Le code Munchkin peut être <a href="https://developers.marketo.com/javascript-api/lead-tracking/">codé en dur</a> ou déployé via Google Tag Manager.</li></td>
  </tr>
  <tr>
    <td>Services Web</td>
    <td><li>Déterminer les utilisateurs/applications pouvant effectuer les opérations suivantes : <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">Appels API</a> dans votre instance.</li>
    <li>Examinez toutes les applications qui effectueront des appels API et déterminez si une augmentation ou une diminution des appels API est nécessaire.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Configuration <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">LaunchPoint</a> des services pour votre entreprise. Chaque point LaunchPoint doit être associé à un utilisateur d’API unique pour faciliter la résolution des problèmes.</li></td>
  </tr>
  <tr>
    <td>Webinaires interactifs (le cas échéant)</td>
    <td>REMARQUE : les webinaires interactifs ne sont configurés que pour les instances de production.
    <li>Pour créer des webinaires interactifs, la fonction de webinaire intégrée, <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">ajouter des utilisateurs à la section "Utilisateur" ;</a> dans l’onglet Webinaire interactif .</li></td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (le cas échéant)</td>
    <td>Pour utiliser <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html">Dynamic Chat</a>, canal d’automatisation de la conversation natif en Marketo Engage, passez à la configuration des autorisations utilisateur en suivant les étapes ci-dessous sur la page <a href="https://adminconsole.adobe.com/">Adobe Admin Console</a>. <br>Confirmez si votre administrateur système d’organisation Adobe vous a accordé un rôle d’administrateur de produit Adobe. Contact <a href="https://helpx.adobe.com/contact.html">Adobe de l’assistance clientèle</a> pour savoir qui, au sein de votre organisation, dispose des privilèges d’administrateur dans la console. <br>Accepter <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">Invitation "Administrateur de produit Dynamic Chat"</a>. La variable <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">courrier électronique de bienvenue</a> est envoyé lorsque Dynamic Chat est activé dans votre instance de Marketo Engage et que vous êtes désigné administrateur système.  <br>Affectez tous les utilisateurs appropriés au profil de produit du Dynamic Chat dans Adobe Admin Console. <br>Si un utilisateur indésirable est ajouté à plusieurs profils de produit, vous devez le supprimer de tous les profils de produit. Sinon, ils auront toujours accès au Dynamic Chat. <br>Vous pouvez <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">modification des profils de produit dans Dynamic Chat</a> et créer un profil personnalisé avec un ensemble personnalisé de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">autorisations disponibles dans votre abonnement</a>. <br>Affecter des utilisateurs à <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">Rôles 'Access Dynamic Chat'</a> dans Marketo Engage/Admin/Utilisateurs et rôles. </td>
  </tr>
  <tr>
    <td>Sales Insight (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">Configuration de l’action Sales Insight</a> dans Sales Insight &gt; Actions Config.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">Attribuer des sièges aux utilisateurs appropriés</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">Configuration de l’API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">Personnalisation des scores de piste</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Invitez les administrateurs de Marketo Engage appropriés à l’instance Sales Connect</a>.</li>
    <li>Procédez comme suit : <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">configuration supplémentaire de l’administrateur de Sales Connect</a> dans Sales Connect et Salesforce.</li></td>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">Activer le coffre au trésor</a> pour tester les fonctionnalités de pilotage.</li>
    <li>Déterminez les fonctionnalités que vous souhaitez activer ou désactiver.</li></td>
  </tr>
  <tr>
    <td>Inspecteur de campagne </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">Activer l’Inspecteur de campagne</a> pour afficher toutes vos campagnes intelligentes en même temps.</li></td>
  </tr>
</tbody>
</table>
