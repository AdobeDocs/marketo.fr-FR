---
description: NOUVELLE ZONE - Documents Marketo - Documentation du produit
title: NOUVELLE ZONE
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '1113'
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
    <td><li>Vérifiez les rôles prédéfinis et vérifiez les autorisations/accès à chaque rôle.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Création d’un nouveau rôle</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">modification des rôles</a> selon les besoins de votre entreprise et la fréquence de connexion des utilisateurs.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html%22%20/l%20%22assign-roles-to-a-user" target="_blank">Affecter des utilisateurs aux rôles appropriés</a>. Les utilisateurs doivent être ajoutés à l’abonnement dans Adobe Admin Console avant d’accorder leurs rôles dans les rôles. Reportez-vous à la section "Utilisateurs" de la liste de contrôle "Configuration initiale" [LIEN]. <br>Après avoir affecté les rôles des utilisateurs, passez en revue le nombre d’utilisateurs par rôle.<br>Implémentez un rôle unique pour chaque utilisateur de l’API pour faciliter la résolution des problèmes.</td>
  </tr>
  <tr>
    <td>Documentation</td>
    <td>Définissez les utilisateurs et les rôles de votre organisation.<br>Définissez votre processus d’ajout d’un nouvel utilisateur/administrateur.</td>
  </tr>
  <tr>
    <td>Environnement de test (le cas échéant)</td>
    <td>Vérifiez les catégories ci-dessus pour votre environnement de test si vous en avez une.</td>
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
    <td>Déterminer le nombre de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> espaces de travail</a> et/ou partitions dont votre organisation a besoin et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">combien d’utilisateurs ont accès à chaque espace de travail.</a><br>Définissez l’objectif principal de chaque espace de travail et partition.<br>Définissez la relation entre vos espaces de travail et vos partitions.</td>
  </tr>
  <tr>
    <td>Documentation</td>
    <td>Documentez comment les espaces de travail sont définis et comment cela se rapporte-t-il aux partitions de base de données (c’est-à-dire un espace de travail global qui voit tout le monde, par rapport aux secteurs d’activité). <br>Importez de nouveaux enregistrements dans la partition appropriée.<br>Définissez la valeur dans le CRM qui place les utilisateurs dans la partition appropriée.</td>
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
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Paramètres de la campagne intelligente</td>
    <td>Ajouter un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">restriction sur la taille de campagne dynamique</a>, empêchant l’envoi accidentel de l’ensemble de la base de données par courrier électronique.</td>
  </tr>
  <tr>
    <td>Documentation</td>
    <td>Documentez comment les espaces de travail sont définis et comment cela se rapporte-t-il aux partitions de base de données (c’est-à-dire un espace de travail global qui voit tout le monde, par rapport aux secteurs d’activité).  <br>Importez de nouveaux enregistrements dans la partition appropriée.<br>Définissez la valeur dans le CRM qui place les utilisateurs dans la partition appropriée.</td>
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
    <td>Sous Domaine de marque, sélectionnez votre domaine et ajoutez votre CNAME de messagerie. Cette valeur doit être au format suivant : [EmailTrackingCNAME].[CompanyDomain].com.  <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Contacter le support Marketo</a> pour la sécuriser avec une configuration de certificat SSL. Ce processus peut prendre jusqu’à 3 jours ouvrables.</td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">Configuration de SPF et DKIM</a> pour la délivrabilité des emails.</td>
  </tr>
  <tr>
  </tr>
  <tr>
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
    <td>Placer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank" rel="noopener noreferrer">Limites de communication</a>.<br>Déterminer si votre entreprise a besoin d’une stratégie sur les limites de communication </td>
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
    <td>Définition de l’utilisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank" rel="noopener noreferrer">channels</a>.</td>
  </tr>
  <tr>
    <td>Balises</td>
    <td>Définition de l’utilisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank" rel="noopener noreferrer">tags</a>.</td>
  </tr>
  <tr>
    <td>Calendrier (le cas échéant)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank" rel="noopener noreferrer">Assertions du calendrier marketing des problèmes</a> à ceux qui ont besoin d’accès. <br>Configuration <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank" rel="noopener noreferrer">Calendrier.</a></td>
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
    <td>Mettre en oeuvre la convention d’affectation des noms pour <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">champs personnalisés.</a> Par exemple, commencez par "MKTO".<br>Soyez sélectif au sujet des champs que vous synchronisez. Plus vous synchronisez de champs, plus le cycle de synchronisation sera lent.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">Bloquer les mises à jour des champs</a> vous souhaitez écrire une seule fois (c’est-à-dire la source de piste d’origine, les détails de la source de piste d’origine, les champs de gestion dynamique des balises Première touche, etc.)</td>
  </tr>
  <tr>
  </tr>
  <tr>
    <td>Activités personnalisées</td>
    <td>Définir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">Activités personnalisées</a> qui sont spécifiques à votre entreprise.  </td>
  </tr>
  <tr>
    <td>Objets personnalisés</td>
    <td>Vérifiez combien de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">Objets personnalisés</a> vous avez besoin. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">Synchroniser ces objets personnalisés avec votre gestion de la relation client</a>. </td>
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
    <td>Lancer la synchronisation CRM. Choisissez l’un des éléments suivants, en fonction du CRM utilisé par votre entreprise : <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>. <br>Identifiez le type d'accès dont vous avez besoin pour accéder à votre CRM. <br>Identifiez votre administrateur CRM pour le dépannage. </td>
  </tr>
  <tr>
    <td>Pages de destination</td>
    <td>REMARQUE : Êtes-vous un client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d’instructions de configuration informatique pendant votre appel de lancement. <br>Configurez votre domaine de landing page avec un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">CNAME</a> et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">saisir les informations sur le domaine et la page ;</a>. Cela doit être au format : [LandingPageCNAME].[CompanyDomain].com <br>Sélectionnez un CNAME pour vos landing pages. Quelques exemples : <br>* **go**.[CompanyDomain].com <br>* **www2**.[CompanyDomain].com <br>* **lp**.[CompanyDomain].com <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console">Contacter le support Marketo</a> pour lancer le processus de configuration d’un certificat SSL. Ce processus peut prendre jusqu’à 3 jours ouvrables. <br>CONSEIL : Gardez-le court ! Les URL plus courtes sont plus faciles à mémoriser. Nous suggérons "go" comme domaine. <br>Ajoutez le code de suivi Analytics (par exemple, Google Analytics ou Adobe Analytics) aux modèles de page d’entrée. </td>
  </tr>
  <tr>
    <td>Munchkin</td>
    <td>REMARQUE : Si vous êtes un client du Launch Pack, ignorez cette étape. Votre consultant vous fournira des instructions de code Munchkin dans votre document d’instructions de configuration informatique. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html">Ajout du code de suivi Munchkin</a> à votre site web. Le code Munchkin peut être <a href="https://developers.marketo.com/javascript-api/lead-tracking/">codé en dur</a> ou déployé via Google Tag Manager.  </td>
  </tr>
  <tr>
    <td>Services Web</td>
    <td>Activer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html">les restrictions IP ;</a> le cas échéant. <br>Déterminer les utilisateurs/applications pouvant effectuer les opérations suivantes : <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">Appels API</a> dans votre instance. <br>Examinez toutes les applications qui effectueront des appels API et déterminez si une augmentation ou une réduction est nécessaire pour les appels API.  </td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td>Configuration requise <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">LaunchPoint</a> des services pour votre entreprise. Chaque point LaunchPoint doit être associé à un utilisateur d’API unique pour faciliter la résolution des problèmes.  </td>
  </tr>
  <tr>
    <td>Webinaires interactifs (le cas échéant)</td>
    <td>REMARQUE : les webinaires interactifs ne sont configurés que pour les instances de production. <br>Pour créer des webinaires interactifs, la fonction de webinaire intégrée, <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">ajouter des utilisateurs à la section "Utilisateur" ;</a> dans l’onglet Webinaire interactif . </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (le cas échéant)</td>
    <td>Pour utiliser <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html">Dynamic Chat</a>, le canal d’automatisation des conversations natif en Marketo Engage, vous passerez à la configuration des autorisations utilisateur en suivant les étapes ci-dessous. <a href="https://adminconsole.adobe.com/">Adobe Admin Console</a>. <br>Confirmez si votre administrateur système d’organisation Adobe vous a accordé un rôle d’administrateur de produit Adobe. Contact <a href="https://helpx.adobe.com/contact.html">Adobe de l’assistance clientèle</a> pour savoir qui, au sein de votre organisation, dispose des privilèges d’administrateur dans la console. <br>Accepter <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">Invitation "Administrateur de produit Dynamic Chat"</a>. La variable <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">courrier électronique de bienvenue</a> est envoyé lorsque Dynamic Chat est activé dans votre instance de Marketo Engage et que vous êtes désigné administrateur système.  <br>Affectez tous les utilisateurs appropriés au profil de produit du Dynamic Chat dans Adobe Admin Console. <br>Si un utilisateur indésirable est ajouté à plusieurs profils de produit, vous devez le supprimer de tous les profils de produit. Sinon, ils auront toujours accès au Dynamic Chat. <br>Vous pouvez <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">modification des profils de produit dans Dynamic Chat</a> et créer un profil personnalisé avec un ensemble personnalisé de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">autorisations disponibles dans votre abonnement</a>. <br>Affecter des utilisateurs à <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">Rôles 'Access Dynamic Chat'</a> dans Marketo Engage/Admin/Utilisateurs et rôles. </td>
  </tr>
  <tr>
    <td>Sales Insight (le cas échéant)</td>
    <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">Configuration de l’action Sales Insight</a> dans Sales Insight &gt; Actions Config.  <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">Donnez des sièges aux utilisateurs appropriés.</a>  <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">Configuration de l’API</a>. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">Personnalisez les scores de piste.</a> </td>
  </tr>
  <tr>
    <td>Sales Connect (le cas échéant)</td>
    <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Invitez les administrateurs de Marketo Engage appropriés à l’instance Sales Connect</a>. <br>Procédez comme suit : <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">configuration supplémentaire de l’administrateur de Sales Connect</a> dans Sales Connect et Salesforce. </td>
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
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">Activer le coffre au trésor</a> pour tester les fonctionnalités de pilotage.  <br>Déterminez les fonctionnalités que vous souhaitez activer ou désactiver. </td>
  </tr>
  <tr>
    <td>Inspecteur de campagne </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">Activer l’Inspecteur de campagne</a> pour afficher toutes vos campagnes intelligentes en même temps. </td>
  </tr>
</tbody>
</table>
