---
description: Liste de contrôle d’administration d’instance héritée - Documents Marketo - Documentation du produit
title: Liste de contrôle d’administration d’instance héritée
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 3%

---

# Instance héritée : liste de contrôle de la section Admin {#inherited-instance-admin-section-checklist}

Les listes de contrôle ci-dessous (les listes de contrôle suivantes mentionnées au bas de chaque article) ont été créées par Adobe Professional Services avec la contribution de Marketo Champions pour vous aider à vous mettre rapidement à niveau. Vous pouvez également [télécharger les listes de contrôle](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) et suivre votre progression.

>[!TIP]
>
>Si vous êtes un nouvel utilisateur ou une nouvelle utilisatrice de Marketo Engage et ne connaissez pas la plupart des termes, consultez le [Glossaire Marketo Engage](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Cela s’applique uniquement aux abonnements Marketo Engage intégrés à [Adobe Identity Management System (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. Si votre abonnement n’a pas encore intégré Adobe IMS, poursuivez avec l’expérience [rôles utilisateur et autorisations hérités](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} dans Marketo Engage > Admin > Utilisateurs et rôles.

<table>
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Administrateur de produit d’abonnement et de Marketo Engage</td>
   <td><li>Votre abonnement Marketo Engage a-t-il déjà été migré vers <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> ?
<br/>     Adobe Admin Console Si tel est le cas, votre rôle d’« administrateur système de Adobe Admin Console » vous a-t-il été attribué ? Si vous ne savez pas qui, dans votre organisation, dispose de privilèges d’administrateur dans la console, contactez l’<a href="https://helpx.adobe.com/contact.html" target="_blank">Assistance clientèle Adobe</a>.</li>
<li>Avez-vous accepté l’invitation « Marketo Engage Product Admin » ? L’e-mail est envoyé lorsque le rôle est attribué dans le Adobe Admin Console.
<br/>     Dans le cas contraire, recherchez l’e-mail de bienvenue <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank"> dans votre boîte de réception et acceptez l’invitation à activer votre Adobe ID</a></li></td>
  </tr>
  <tr>
   <td>Profil produit</td>
   <td><li>Tous les utilisateurs appropriés sont-ils affectés au profil de produit Marketo Engage dans Adobe Admin Console ?
<br/>     Dans le cas contraire, veillez à <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">ajouter et/ou supprimer des utilisateurs</a> des profils de produit Marketo Engage dans le Adobe Admin Console. Vous ne pouvez pas affecter les rôles des utilisateurs dans Marketo Engage &gt; Admin &gt; Utilisateurs et rôles s’ils sont ajoutés à un profil de produit.</li>
<p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : si un utilisateur indésirable est ajouté à plusieurs profils de produit, vous devez le supprimer de tous les profils de produit. Sinon, ils auront toujours accès à Marketo Engage.</td>
  </tr>
  <tr>
   <td>API User Management</td>
   <td><li>Votre abonnement utilise-t-il des API User Management de Marketo ?
<br/>     Si tel est le cas, vous devrez utiliser les <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">API Adobe IMS</a> pour inviter, mettre à jour et supprimer des utilisateurs à l’avenir.</li>
<p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : la « gestion des rôles » reste dans Marketo Engage et les API User Management de Marketo peuvent toujours être utilisées pour la gestion des rôles.</td>
  </tr>
 </tbody>
</table>

## Utilisateurs et rôles {#users-and-roles}

<table>
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Utilisateurs et utilisatrices</td>
   <td><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : si votre abonnement se trouve déjà dans Adobe IMS, passez à la révision de la gestion des utilisateurs dans Adobe Admin Console. Sinon, accédez à Admin &gt; Utilisateurs et rôles &gt; Utilisateurs dans Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Combien d’utilisateurs </a>-vous ?</li>
<li>Y a-t-il des utilisateurs qui doivent être <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">supprimés</a> ?</li>
<li>Votre entreprise applique-t-elle des politiques concernant la suppression d’utilisateurs ?</li>
<li>Combien d’utilisateurs disposent des <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">autorisations d’administrateur</a> ?</li>
<li>L’un de ces utilisateurs doit-il être remplacé par <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">d’autres rôles ?</a></li>
<li>Qui sont les <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">utilisateurs d’API</a> dans cette instance ?</li></td>
  </tr>
  <tr>
   <td>Rôles</td>
   <td><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : que vous utilisiez Marketo avec Adobe Identity ou non, passez en revue les autorisations des rôles dans Marketo Engage sous Admin &gt; Utilisateurs et rôles &gt; Rôles.
   <p><li>Combien y a-t-il de rôles ?</li>
<li>De quelles <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">autorisations/accès</a> dispose chaque rôle ? Devrait-on en ajuster?</li>
<li>Combien d’utilisateurs y a-t-il par rôle ?</li>
<li>À quelle fréquence les utilisateurs <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">se connectent-ils</a> ?</li>
<li>Chaque utilisateur de l’API dispose-t-il de son <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">rôle d’utilisateur</a> ? Si ce n’est pas le cas, envisagez de mettre en œuvre ceci pour faciliter le dépannage.</li>
<li>Vos rôles utilisateur et vos autorisations s’alignent-ils sur vos politiques de confidentialité des données d’entreprise pour assurer la conformité à la réglementation (par exemple, <a href="https://gdpr-info.eu/" target="_blank">RGPD</a>) ? Les données d’entreprise <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">politiques de confidentialité</a> permettent-elles aux utilisateurs de télécharger et de partager des données utilisateur Marketo Engage ? L’activité d’autorisation est-elle nécessaire ?</li></td>
  </tr>
  <tr>
   <td>Utilisateurs du support technique</td>
   <td><li>Avez-vous configuré les <a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">contacts autorisés</a> appropriés dans le portail d’assistance ?</li></td>
  </tr>
  <tr>
   <td>Documentation interne</td>
   <td><li>Les utilisateurs et les rôles sont-ils clairement définis dans votre organisation ?</li>
<li>Quel est votre processus d’ajout d’un nouvel utilisateur/administrateur ?</li></td>
  </tr>
  <tr>
   <td>Sandbox (le cas échéant)</td>
   <td><li>Avez-vous une <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">instance sandbox</a> ?
   <br/>     Si tel est le cas, passez en revue les catégories ci-dessus pour votre sandbox.</li>
<li>L’<a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">importation de programme</a> est-elle liée à votre sandbox ?</li></td>
  </tr>
 </tbody>
</table>

## Journal d’audit {#audit-trail}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Journal d’audit</td>
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Qui travaille</a> dans cette instance ?</li></td>
  </tr>
 </tbody>
</table>

## Espaces de travail &amp; Divisions {#workspaces-and-partitions}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Espaces de travail &amp; Divisions</td>
   <td><li>Combien d’espaces de travail et/ou de partitions <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank"></a> avez-vous ?</li>
<li>Quel est l’objectif principal de chaque Workspace et partition ?</li>
<li>Vos <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">espaces de travail</a> ou <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">partitions</a> doivent-ils être audités/modifiés ?</li>
<li>Quelle est la relation entre vos espaces de travail et vos partitions ?</li>
<li>Combien d’utilisateurs <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">ont accès</a> à chaque Workspace ?</li></td>
  </tr>
  <tr>
   <td>Documentation interne</td>
   <td><li>Comment les espaces de travail et les partitions sont-ils définis ?</li>
<li>Quel est votre processus pour ajouter des espaces de travail à votre instance ou ajouter des utilisateurs à un Workspace ?</li></td>
  </tr>
 </tbody>
</table>

## Campagnes intelligentes {#smart-campaigns}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Campagnes intelligentes</td>
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Avez-vous une restriction </a> sur la taille des campagnes intelligentes ?
   <br/>     Si ce n’est pas le cas, envisagez d’en ajouter un. Nous vous recommandons de limiter les limites de Smart Campaign à 25 % de votre base de données afin d’éviter toute surcommunication ou traitement de l’ensemble de votre base de données dans les workflows. Cela permet non seulement de protéger votre marque, mais également de protéger les performances de votre instance.</li></td>
  </tr>
 </tbody>
</table>

## Limites de communication {#communication-limits}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Limites de communication</td>
   <td><li>Existe-t-il des <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">limites de communication</a> ? Votre entreprise dispose-t-elle de politiques dans lesquelles des limites de communication peuvent être nécessaires ?</li>
<p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : nous vous recommandons de limiter votre communication à 1 par jour et 3 par 7 jours, avec les e-mails <b>non</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">opérationnels</a> bloqués.</td>
  </tr>
 </tbody>
</table>

## Balises {#tags}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Balises</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Combien y a-t-il de balises </a> ? Combien de balises sont utilisées ? Faut-il en ajouter ?</li>
<li>Les balises sont-elles requises dans vos programmes ?</li></td>
  </tr>
  <tr>
   <td>Canaux</td>
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Combien de canaux </a>-vous ? Combien sont en cours d'utilisation ?</li>
<li>Tous les <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">statuts de programme de canal</a> sont-ils appropriés ? Est-ce qu'il y a une progression dans le programme?</li>
<li>Vos canaux sont-ils liés à des types de programmes spécifiques ?</li>
<li>Quels états sont considérés comme une réussite pour chaque canal ? Est-ce que cela correspond à vos objectifs de marketing?</li>
<li>Le canal opérationnel est-il utilisé de manière appropriée ?</li>
<li>Pour Advanced Report Builder (Revenue Cycle Explorer/RCE), le comportement d’analyse des canaux est-il défini pour s’aligner sur les pratiques de votre programme en incorporant le coût de la période ?</li></td>
  </tr>
  <tr>
   <td>Calendrier marketing (le cas échéant)</td>
   <td><li>Combien y a-t-il de <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">types d’entrées de calendrier</a> ? Sont-elles toutes toujours pertinentes ?</li></td>
  </tr>
 </tbody>
</table>

## Gestion de la base de données {#database-management}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Gestion des champs</td>
   <td><li>Combien y a-t-il de champs ?
   <br/>     Cliquez sur <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Exporter les noms de champ</a> pour consulter une liste de vos champs, champs personnalisés et leurs noms d’API.</li>
<li>Combien y a-t-il <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank"> champs personnalisés </a> ?</li>
<li>Combien de champs sont utilisés ?
<br/>     Sélectionnez <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank"> Exportation utilisée par </a> dans la liste déroulante Actions de champ pour passer en revue les ressources associées d’un champ.</li>
<li>Combien de champs sont synchronisés entre Marketo Engage et votre CRM ?</li>
<li>Les champs du CRM sont-ils synchronisés avec les objets appropriés ?</li>
<li>Existe-t-il un <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">affichage personnalisé</a> pour les détails de la personne ? Devrait-il y en avoir ?</li>
<li>Avez-vous une convention de nommage pour vos champs basée sur la source ?
<br/>     Sinon, envisagez d’implémenter cette .</li>
<li>Y a-t-il des champs <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">bloqués</a> ?
<br/>     Si oui, assurez-vous de comprendre pourquoi ils le sont.</li></td>
  </tr>
  <tr>
   <td>Activités personnalisées</td>
   <td><li>Existe-t-il des <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">activités personnalisées</a> ?
<br/>     Si tel est le cas, cliquez dessus pour identifier les activités qui ne sont pas liées à un formulaire Marketo, un e-mail ou une page de destination.</li></td>
  </tr>
  <tr>
   <td>Objets personnalisés</td>
   <td><li>Combien y'a-t-il d'<a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">objets personnalisés</a> ? Comment sont-ils synchronisés avec votre CRM ?</li>
<li>Comment ces objets personnalisés sont-ils utilisés par vos programmes et requêtes de liste ?</li></td>
  </tr>
 </tbody>
</table>

## E-mail {#email}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Paramètres par défaut des e-mails</td>
   <td><li>Dans Admin &gt; E-mail, tous vos paramètres par défaut sont-ils à jour (par exemple, e-mail/libellé <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank"> « de »</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">domaine de branding</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">message de désabonnement</a>, etc.) ?</li></td>
  </tr>
 </tbody>
</table>

## Intégrations {#integrations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>CRM</td>
   <td><li>À quel CRM effectuez-vous une synchronisation ? SALESFORCE ? MS Dynamics ? Veeva ?</li>
<li>Utilisez-vous une <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">synchronisation personnalisée</a> ?</li>
<li>[Salesforce uniquement] Votre instance dispose-t-elle de filtres de synchronisation personnalisés implémentés ?
<p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : contactez l’assistance Marketo pour identifier les filtres de synchronisation personnalisés ou demander l’implémentation d’une règle de synchronisation personnalisée.</li></td>
  </tr>
  <tr>
   <td>Pages de destination</td>
   <td><li>En quoi le <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">domaine est-il défini</a> ?</li>
   <li>En quoi la page d’accueil est-elle définie ?</li>
<li>En quoi consiste le <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">jeu de secours</a> ?</li>
<li>Le préremplissage de formulaire est-il activé ?</li>
<li>Les <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">URL personnalisées</a> sont-elles activées ?</li>
<li>Existe-t-il des règles configurées pour les <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">redirections</a> ?</li>
<li>Avez-vous des alias de domaine en place ? Effectuez-vous un suivi de la manière dont vous utilisez les alias de domaine ?</li>
<li>L’option <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">Domaines sécurisés pour les pages de destination</a> est-elle activée ?
<br/>     Vérifiez si les ressources de votre page de destination contiennent une URL « http ».</li></td>
  </tr>
  <tr>
   <td>Munchkin</td>
   <td><li>Votre <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">code de suivi Munchkin se trouve-t-il sur votre site web </a> (il ne s’agit pas d’une page de destination Marketo Engage) ?</li>
<li>Une requête de navigateur <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Ne pas suivre</a> est-elle activée ?</li>
<li>Votre <a href="https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking" target="_blank">API Munchkin</a> est-elle configurée ?
<p><img src="assets/tip-icon.png" alt="icône d’astuce">CONSEIL : si vous ne disposez pas de documentation sur l’emplacement du code munchkin sur votre site web, vous pouvez afficher toutes les URL en créant un <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">rapport d’activité de page web</a>.</li></td>
  </tr>
  <tr>
   <td>Services Web</td>
   <td><li>Les <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">restrictions IP</a> sont-elles activées ? Devraient-ils l'être ?</li>
<li>Quels utilisateurs/applications effectuent des appels API dans votre instance ?</li>
<li>Atteignez-vous ou êtes-vous sur le point d’atteindre votre limite d’API ?
<br/>     Si tel est le cas, envisagez de l’augmenter ou d’auditer votre instance pour réduire ces appels API.</li></td>
  </tr>
  <tr>
   <td>Adobe Dynamic Chat (le cas échéant)</td>
<td>Vous devrez accéder à <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a> en suivant les étapes ci-dessous. Si vous n’avez pas encore configuré d’Adobe ID, <a href="https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html" target="_blank">découvrez comment faire ici</a>.
<br/>
<li>Avez-vous accepté l’invitation <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Administrateur de produit Dynamic Chat</a> ? L’e-mail est envoyé lorsque Dynamic Chat est activé dans votre instance Marketo Engage et que vous êtes désigné comme administrateur système.
<br/>     Dans le cas contraire, recherchez l’e-mail de bienvenue dans votre boîte de réception et acceptez l’invitation à configurer votre Adobe ID.</li>
<li>Avez-vous ajouté les <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">utilisateurs souhaités</a> au profil de produit Dynamic Chat dans Adobe Admin Console ?
<li>Assurez-vous que les utilisateurs éligibles disposent du profil de produit Dynamic Chat ajouté à leur identité Adobe. Vous ne pouvez pas affecter de rôles « Accéder à Dynamic Chat » dans Marketo Engage &gt; Admin &gt; Utilisateurs et rôles s’ils sont ajoutés à un profil de produit.</li>
<li>Dans l’onglet « Profils de produit », les autorisations de profil par défaut sont-elles alignées avec les besoins de votre organisation ?<br/>
Dans le cas contraire, modifiez les autorisations pour le profil spécifique. </li>
<li>Si vous disposez de plusieurs abonnements, vos utilisateurs sont-ils ajoutés aux bons abonnements ?</li>
<br>
Une fois l’audit des paramètres Utilisateurs et rôles terminé, connectez-vous à Dynamic Chat pour poursuivre l’audit.
<li>Avez-vous <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">connecté votre instance Marketo Engage</a> à Dynamic Chat ?</li>
<li>Les cinq profils par défaut avec des autorisations prédéfinies s’appliquent-ils à votre organisation ?<br/>
     Dans le cas contraire, vous pouvez <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">les modifier dans Dynamic Chat</a>. Vous pouvez également <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">créer un profil personnalisé</a> avec un ensemble personnalisé d’autorisations.</li>
<li>Pour fournir à vos utilisateurs l’accès à Dynamic Chat, avez-vous coché « Accéder à Dynamic Chat » pour le rôle Marketo Engage applicable sous Admin &gt; Utilisateurs et rôles &gt; Rôles ?
<br/><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : les rôles « Admin » et « Utilisateur marketing » doivent avoir accès à Dynamic Chat.</li>
</td>
  </tr>
  <td>Marketo Sales Insight (le cas échéant)</td>
   <td><li>Le package <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI a-t-il été installé</a> ?</li>
<li>Avez-vous <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">mis à niveau vers la dernière version de Sales Insight</a> ?</li>
<li>Avez-vous terminé la configuration de Sales Insight ? <br/>     Utilisateurs d’entreprise/illimités <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">cliquez ici</a>, utilisateurs professionnels <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">cliquez ici</a>.</li>
<li>Avez-vous <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">donné l’accès à vos utilisateurs</a> en fonction du nombre de places achetées ?</li>
<li>Est-ce que <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Stars and Flames</a> est personnalisé ?</li></td>
  </tr>
  <tr>
   <td>Point de lancement (le cas échéant)</td>
   <td><li>Quels services avez-vous configurés (par exemple, <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a>, etc.) ? Y en a-t-il qui arrivent à expiration ?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Combien d’appels d’API </a> vos intégrations utilisent-elles ?</li>
<li>Avez-vous mis en place les intégrations appropriées pour vos cas d’utilisation ?</li></td>
  </tr>
  <tr>
   <td>Webhooks (le cas échéant)</td>
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Quelles connexions </a> avez-vous configurées ?</li>
<li>Les modèles ne sont-ils plus utilisés ?</li></td>
  </tr>
  <tr>
   <td>Applications mobiles (le cas échéant)</td>
   <td><li>De quelles <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">applications mobiles</a> disposez-vous ?</li>
<li>Des <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">appareils de test</a> ont-ils été ajoutés ?</li></td>
  </tr>
 </tbody>
</table>

## Coffre au trésor {#treasure-chest}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Coffre au trésor</td>
   <td><li>Qu'est-ce qui se passe dans le <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">coffre au trésor</a> ?</li>
<li>Certaines fonctionnalités doivent-elles être activées ou désactivées ?</li></td>
  </tr>
  <tr>
   <td>Inspecteur de campagne</td>
   <td><li>L’option <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Inspecteur de campagne</a> est-elle activée ?
<br/>Si ce n’est pas le cas, envisagez de l’activer pour identifier facilement les campagnes actives, celles qui se synchronisent avec votre CRM et/ou celles qui suppriment des enregistrements.</li></td>
  </tr>
 </tbody>
</table>

## alertes et mises à jour ; {#alerts-and-updates}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Mises à jour du statut de Marketo Engage</td>
   <td><li>Votre instance est-elle abonnée aux <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">mises à jour de statut de Marketo Engage </a> ?</li></td>
  </tr>
  <tr>
   <td>Alertes</td>
   <td><li>Des <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">alertes actives</a> sont-elles envoyées à des équipes internes depuis Marketo Engage ?</li>
<li>Si oui, ces alertes fonctionnent-elles correctement ?</li></td>
  </tr>
  <tr>
   <td>Notifications</td>
   <td><li>Êtes-vous abonné aux <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">notifications</a> d’administration appropriées ?</li></td>
  </tr>
 </tbody>
</table>
