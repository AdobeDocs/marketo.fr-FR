---
description: NOUVELLE ZONE - Documents Marketo - Documentation du produit
title: NOUVELLE ZONE
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: d65903d64d068a6f919df78258654414f3b76426
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 6%

---

# NOUVELLE ZONE : Liste de contrôle de l’administrateur {#new-area-admin-checklist}

Texte d’introduction.

## Rôles {#roles}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rôles</td>
    <td><li>Vérifiez les rôles prédéfinis et vérifiez les autorisations/accès à chaque rôle.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Création d’un nouveau rôle</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">modification des rôles</a> selon les besoins de votre entreprise et la fréquence de connexion des utilisateurs.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Affecter des utilisateurs aux rôles appropriés</a>.</li>
    <li>Après avoir affecté les rôles des utilisateurs, passez en revue le nombre d’utilisateurs par rôle.</li>  <li>Implémentez un rôle unique pour chaque utilisateur de l’API pour faciliter la résolution des problèmes.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Documentation</td>
    <td>Définissez les utilisateurs et les rôles de votre organisation. <br>Définissez votre processus d’ajout d’un nouvel utilisateur/administrateur.</td>
    <td></td>
  </tr>
  <tr>
    <td>Environnement de test (le cas échéant)</td>
    <td>Vérifiez les catégories ci-dessus pour votre environnement de test si vous en avez une.</td>
    <td></td>
  </tr>
</tbody>
</table>

## Espaces de travail et partitions {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espaces de travail et partitions </td>
    <td><li>Déterminer le nombre de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> espaces de travail</a> et/ou partitions dont votre organisation a besoin et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">combien d’utilisateurs ont accès à chaque espace de travail.</a></li>
    <li>Définissez l’objectif principal de chaque espace de travail et partition.</li>
    <li>Définissez la relation entre vos espaces de travail et vos partitions.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Documentation</td>
    <td><li>Documentez comment les espaces de travail sont définis et comment cela se rapporte-t-il aux partitions de base de données (c’est-à-dire un espace de travail global qui voit tout le monde, par rapport aux secteurs d’activité).</li>
    <li>Importez de nouveaux enregistrements dans la partition appropriée.</li>
    <li>Définissez la valeur dans le CRM qui place les utilisateurs dans la partition appropriée.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Paramètres de la campagne intelligente {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Paramètres de la campagne intelligente </td>
    <td><li>Ajouter un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">restriction sur la taille de campagne dynamique</a>, empêchant l’envoi accidentel de l’ensemble de la base de données par courrier électronique.</li>
    <li>Activation des restrictions pour les personnes dans les campagnes dynamiques</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Paramètres d’e-mail {#email-settings}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Valeurs par défaut des emails</td>
    <td><li>Sous Domaine de marque, sélectionnez votre domaine et ajoutez votre CNAME de messagerie. Cette valeur doit être au format suivant : [EmailTrackingCNAME].[CompanyDomain].com.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Configuration de SPF et DKIM</a> pour la délivrabilité des emails.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Limites de communication {#communication-limits}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limites de communication</td>
    <td><li>Placer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Limites de communication</a>.</li>
    <li>Déterminez si votre entreprise a besoin d’une stratégie sur les limites de communication.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Balises {#tags}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canaux</td>
    <td><li>Définition de l’utilisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">channels</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Balises </td>
    <td><li>Définition de l’utilisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">tags</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Calendrier (le cas échéant) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Assertions du calendrier marketing des problèmes</a> à ceux qui ont besoin d’accès.</li> 
    <li>Configuration <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Calendrier</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Gestion de la base de données {#database-management}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gestion des champs</td>
    <td><li>Mettre en oeuvre la convention d’affectation des noms pour <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">champs personnalisés.</a> Par exemple, commencez par "MKTO".</li>
    <li>Soyez sélectif au sujet des champs que vous synchronisez. Plus vous synchronisez de champs, plus le cycle de synchronisation sera lent.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Bloquer les mises à jour des champs</a> vous souhaitez écrire une seule fois (c’est-à-dire la source de piste d’origine, les détails de la source de piste d’origine, les champs de gestion dynamique des balises Première touche, etc.).</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Activités personnalisées </td>
    <td><li>Définir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">Activités personnalisées</a> qui sont spécifiques à votre entreprise.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Objets personnalisés </td>
    <td><li>Vérifiez combien de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">Objets personnalisés</a> vous avez besoin.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">Synchroniser ces objets personnalisés avec votre gestion de la relation client</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Intégrations {#integrations}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Lancer la synchronisation CRM. Choisissez l’un des éléments suivants, en fonction du CRM utilisé par votre entreprise : <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>Identifiez le type d'accès dont vous avez besoin pour accéder à votre CRM.</li>
    <li>Identifiez votre administrateur CRM pour le dépannage.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Sales Insight (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank">Configurez Sales Insight.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">Donnez des sièges aux utilisateurs appropriés.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">Configuration de l’API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">Personnalisez les scores de piste.</a></li></td>
    <td></td>
  </tr>
  <tr>
    <td>Pages de destination </td>
    <td>REMARQUE : Êtes-vous un client de Launch Pack ? Vous pouvez ignorer cette étape. Votre consultant vous fournira un document d’instructions de configuration informatique pendant votre appel de lancement. <br>Configurez votre domaine de landing page avec un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">CNAME</a> et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">saisir les informations sur le domaine et la page ;</a>. Cela doit être au format : [LandingPageCNAME].[CompanyDomain].com <br>Sélectionnez un CNAME pour vos landing pages. Quelques exemples : <br>* **go**.[CompanyDomain].com <br>* **www2**.[CompanyDomain].com <br>* **lp**.[CompanyDomain].com <br>CONSEIL : Gardez-le court ! Les URL plus courtes sont plus faciles à mémoriser. Nous suggérons "go" comme domaine. <br>Ajoutez le code de suivi Analytics (par exemple, Google Analytics ou Adobe Analytics) aux modèles de page d’entrée. </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Edit+Landing+Page+Settings">Modifier les paramètres de la page d’entrée</a></td>
  </tr>
  <tr>
    <td rowspan="2">Munchkin </td>
    <td rowspan="2">REMARQUE : Si vous êtes un client du Launch Pack, ignorez cette étape. Votre consultant vous fournira des instructions de code Munchkin dans votre document d’instructions de configuration informatique. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html" target="_blank">Ajout du code de suivi Munchkin</a> à votre site web. Le code Munchkin peut être <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">codé en dur</a> ou déployé via Google Tag Manager.</td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Add+Munchkin+Tracking+Code+to+Your+Website">Ajout du code de suivi Munchkin à votre site web</a> </td>
  </tr>
  <tr>
    <td><a href="https://developers.marketo.com/javascript-api/lead-tracking/">Suivi des pistes</a> </td>
  </tr>
  <tr>
    <td>Services web </td>
    <td>Activer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html" target="_blank">les restrictions IP ;</a> le cas échéant. <br>Déterminer les utilisateurs/applications pouvant effectuer les opérations suivantes : <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">Appels API</a> dans votre instance. <br>Examinez toutes les applications qui effectueront des appels API et déterminez si une augmentation ou une réduction est nécessaire pour les appels API.</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html#product-docs">Création d’une Liste autorisée pour l’accès aux API basées sur l’adresse IP </a> </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (le cas échéant) </td>
    <td>Pour utiliser <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html" target="_blank">Dynamic Chat</a>, le canal d’engagement conversationnel natif en Marketo Engage, vous passerez à la configuration des autorisations utilisateur en suivant les étapes ci-dessous. <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. <br> <br>Confirmez si votre administrateur système d’organisation Adobe vous a accordé un rôle d’administrateur de produit Adobe. Contact <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe de l’assistance clientèle</a><a href="https://helpx.adobe.com/contact.html)." target="_blank">https://helpx.adobe.com/contact.html</a> pour savoir qui, au sein de votre organisation, dispose des privilèges d’administrateur dans la console. <br>Accepter <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">Invitation "Administrateur de produit Dynamic Chat"</a>. La variable <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">courrier électronique de bienvenue</a> est envoyé lorsque Dynamic Chat est activé dans votre instance de Marketo Engage et que vous êtes désigné administrateur système.  <br>Affectez tous les utilisateurs appropriés au profil de produit du Marketo Engage dans Adobe Admin Console. <br>Vous ne pouvez pas affecter les rôles des utilisateurs dans Marketo Engage/Admin/Utilisateurs et rôles avant de les ajouter à un profil de produit.  <br>Si un utilisateur indésirable est ajouté à plusieurs profils de produit, vous devez le supprimer de tous les profils de produit. Sinon, ils auront toujours accès au Dynamic Chat. </td>
    <td> </td>
  </tr>
  <tr>
    <td>Point de lancement (le cas échéant) </td>
    <td>Configurez les <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a> des services pour votre entreprise.  <br>REMARQUE : les webinaires interactifs sont une fonctionnalité de webinaire intégrée avec une intégration native à Adobe Connect. Aucune intégration supplémentaire n’est nécessaire, mais votre instance devra <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">synchronisation avec Adobe Connect as a LaunchPoint Service.</a>  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Additional+Integrations">Intégrations supplémentaires</a> </td>
  </tr>
  <tr>
    <td>Webhooks (le cas échéant)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">Créer tous les webhooks requis</a> pour vos affaires.  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Create+a+Webhook">Création d’un webhook</a> </td>
  </tr>
</tbody>
</table>

## Coffre au trésor {#treasure-chest}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Coffre au trésor</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">Activer le coffre au trésor</a> pour tester les fonctionnalités de pilotage.  <br>Déterminez les fonctionnalités que vous souhaitez activer ou désactiver.</td>
    <td>Texte</td>
  </tr>
  <tr>
    <td>Inspecteur de campagne </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">Activer l’Inspecteur de campagne</a> pour afficher toutes vos campagnes intelligentes en même temps.</td>
    <td>Texte</td>
  </tr>
</tbody>
</table>
