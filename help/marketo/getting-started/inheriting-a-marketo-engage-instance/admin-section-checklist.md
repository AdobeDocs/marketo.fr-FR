---
description: Liste de contrôle de l’administrateur d’instance hérité - Documents Marketo - Documentation du produit
title: Liste de contrôle de l’administrateur d’instance hérité
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 3%

---

# Instance héritée : liste de contrôle de section d’administration {#inherited-instance-admin-section-checklist}

Les listes de contrôle ci-dessous (listes de contrôle ultérieures liées au bas de chaque article) ont été mises en place par Adobe Professional Services avec la participation des champions Marketo pour vous aider à vous mettre rapidement au courant. Vous pouvez également [télécharger les listes de contrôle](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) et suivre votre progression.

>[!TIP]
>
>Si vous êtes un nouvel utilisateur Marketo Engage et que vous ne connaissez pas beaucoup des termes, consultez le [Glossaire du Marketo Engage](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Cela s’applique uniquement aux abonnements des Marketo Engage intégrés à [Adobe Identity Management System (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. Si votre abonnement n’est pas encore intégré à Adobe IMS, passez à l’[expérience héritée des rôles utilisateur et des autorisations](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} dans Marketo Engage > Admin > Utilisateurs et rôles.

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th> 
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Administration des produits d’abonnement et de Marketo Engage</td> 
   <td><li>Votre abonnement de Marketo Engage a-t-il déjà été migré vers <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> ? 
<br/>     Si tel est le cas, votre "administrateur système Adobe Admin Console" vous a-t-il attribué un rôle "Administrateur de produit Adobe Admin Console" ? Si vous ne savez pas qui dans votre organisation dispose des privilèges d’administrateur dans la console, contactez l’ <a href="https://helpx.adobe.com/contact.html" target="_blank">assistance clientèle Adobe</a>.</li>
<li>Avez-vous accepté l’invitation "Administrateur de produit Marketo Engage" ? L’e-mail est envoyé lorsque le rôle est attribué dans Adobe Admin Console.
<br/>     Si ce n’est pas le cas, recherchez l’<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">e-mail de bienvenue</a> dans votre boîte de réception et acceptez l’invitation à activer votre Adobe ID.</li></td>
  </tr>
  <tr> 
   <td>Profil produit</td> 
   <td><li>Tous les utilisateurs appropriés sont-ils affectés au profil de produit du Marketo Engage dans Adobe Admin Console ?
<br/>     Si ce n’est pas le cas, veillez à <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">ajouter et/ou supprimer des utilisateurs</a> des profils de produit de Marketo Engage dans Adobe Admin Console. Vous ne pouvez pas affecter les rôles des utilisateurs dans Marketo Engage &gt; Admin &gt; Utilisateurs et rôles s’ils sont ajoutés à un profil de produit.</li>
<p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : Si un utilisateur indésirable est ajouté à plusieurs profils de produit, vous devez le supprimer de tous les profils de produit. Sinon, ils auront toujours accès au Marketo Engage.</td>
  </tr>
  <tr> 
   <td>API User Management</td> 
   <td><li>Votre abonnement utilise-t-il des API de gestion des utilisateurs de Marketo ?
<br/>     Si tel est le cas, vous devrez utiliser les <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">API Adobe IMS</a> pour inviter, mettre à jour et supprimer des utilisateurs à partir de maintenant.</li>
<p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : "Gestion des rôles" reste dans Marketo Engage et les API de gestion des utilisateurs de Marketo peuvent toujours être utilisées pour la gestion des rôles.</td>
  </tr>
 </tbody> 
</table>

## Utilisateurs et rôles {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Utilisateurs et utilisatrices</td> 
   <td><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : Si votre abonnement figure déjà sur Adobe IMS, passez à l’examen suivant de la gestion des utilisateurs dans Adobe Admin Console. Sinon, accédez à Admin &gt; Utilisateurs et rôles &gt; Utilisateurs dans Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Combien d’utilisateurs</a> y a-t-il ?</li>
<li>Y a-t-il des utilisateurs qui doivent être <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">supprimés</a> ?</li>
<li>Votre entreprise a-t-elle des politiques concernant la suppression d’utilisateurs ?</li> 
<li>Combien d’utilisateurs disposent de <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">droits d’administrateur</a> ?</li>
<li>L'un de ces utilisateurs doit-il être remplacé par <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">autres rôles ?</a></li> 
<li>Qui sont les <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">utilisateurs de l’API</a> dans cette instance ?</li></td>
  </tr>
  <tr> 
   <td>Rôles</td> 
   <td><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : Que vous utilisiez Marketo avec ou non l’identité de l’Adobe, passez en revue les autorisations de rôle dans Marketo Engage sous Admin &gt; Utilisateurs et rôles &gt; Rôles.
   <p><li>Combien y a-t-il de rôles ?</li>  
<li>De quels <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">autorisations/accès</a> chaque rôle possède-t-il ? Y a-t-il des ajustements ?</li>
<li>Combien d’utilisateurs y a-t-il par rôle ?</li>
<li>À quelle fréquence les utilisateurs <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">se connectent-ils </a> ?</li>
<li>Chaque utilisateur de l’API a-t-il son <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">propre rôle utilisateur</a> ? Si ce n’est pas le cas, envisagez de mettre en oeuvre cette méthode pour faciliter le dépannage.</li> 
<li>Vos rôles utilisateur et autorisations sont-ils conformes aux politiques de confidentialité des données de votre entreprise en ce qui concerne la conformité aux réglementations (par exemple, <a href="https://gdpr-info.eu/" target="_blank">RGPD</a>) ? Les <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">stratégies de confidentialité</a> des données d’entreprise permettent-elles aux utilisateurs de télécharger et de partager des données utilisateur de Marketo Engage ? Est-il nécessaire d'accorder des autorisations ?</li></td>
  </tr>
  <tr> 
   <td>Utilisateurs de l’assistance</td> 
   <td><li>Avez-vous configuré les <a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">contacts autorisés</a> appropriés dans le portail d’assistance ?</li></td>
  </tr>
  <tr> 
   <td>Documentation interne</td> 
   <td><li>Les utilisateurs et les rôles sont-ils clairement définis dans votre organisation ?</li>
<li>Quel est votre processus pour ajouter un nouvel utilisateur/administrateur ?</li></td>
  </tr>
  <tr> 
   <td>Environnement de test (le cas échéant)</td> 
   <td><li>Avez-vous une <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">instance sandbox</a> ?
   <br/>     Si tel est le cas, passez en revue les catégories ci-dessus pour votre environnement de test.</li>
<li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Import de programme</a> est-il lié à votre environnement de test ?</li></td>
  </tr>
 </tbody> 
</table>

## Piste d&#39;audit {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Piste d'audit</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Qui travaille</a> dans l’instance ?</li></td>
  </tr>
 </tbody> 
</table>

## Espaces de travail &amp; Divisions {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Espaces de travail &amp; Divisions</td> 
   <td><li>Combien d'<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">espaces de travail et/ou de partitions</a> avez-vous ?</li>
<li>Quel est l’objectif principal de chaque Workspace et partition ?</li>
<li>Est-ce que vos <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">espaces de travail</a> ou <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Partitions</a> doivent faire l'objet d'un audit/d'une modification ?</li>
<li>Quelle est la relation entre vos espaces de travail et vos partitions ?</li>
<li>Combien d’utilisateurs <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank"> ont accès </a> à chaque Workspace ?</li></td>
  </tr>
  <tr> 
   <td>Documentation interne</td> 
   <td><li>Comment les espaces de travail et les partitions sont-ils définis ?</li>
<li>Quel est votre processus pour ajouter des espaces de travail à votre instance ou ajouter des utilisateurs à une Workspace ?</li></td>
  </tr>
 </tbody> 
</table>

## Campagnes intelligentes {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Campagnes intelligentes</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Existe-t-il une restriction</a> sur la taille d’une campagne dynamique ? 
   <br/>     Si ce n’est pas le cas, envisagez d’en ajouter une. Nous vous recommandons de limiter les limites de la campagne dynamique à 25 % de votre base de données afin d’éviter toute trop de communication ou de traitement de l’ensemble de votre base de données dans les workflows. Cela protège non seulement votre marque, mais également les performances de votre instance.</li></td>
  </tr>
 </tbody> 
</table>

## Limites de communication {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Limites de communication</td> 
   <td><li>Y a-t-il des <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">limites de communication</a> en place ? Votre entreprise a-t-elle des politiques pour lesquelles des limites de communication peuvent être nécessaires ?</li>
<p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : Nous vous recommandons de limiter votre communication à 1 par jour et 3 par 7 jours, avec des emails <b>non</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">opérationnels</a> bloqués.</td>
  </tr>
 </tbody> 
</table>

## Balises {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Balises</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Combien de balises</a> y a-t-il ? Combien de balises sont utilisées ? Dois-je ajouter des éléments ?</li>
<li>Les balises sont-elles requises dans vos programmes ?</li></td>
  </tr>
  <tr> 
   <td>Canaux</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Combien de canaux</a> y a-t-il ? Combien sont utilisés ?</li>
<li>Tous les <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">états du programme de canal sont-ils appropriés</a> ? Est-ce qu'ils affichent la progression dans le programme ?</li>
<li>Vos canaux sont-ils liés à des types de programmes spécifiques ?</li>
<li>Quels états sont considérés comme une réussite pour chaque canal ? Ces objectifs correspondent-ils à vos objectifs marketing ?</li>
<li>Le canal opérationnel est-il utilisé de manière appropriée ?</li>
<li>Dans le cas d’un Report Builder avancé (l’explorateur de cycle de revenu/le RCE), le comportement de l’analyse des canaux est-il défini de manière à s’aligner sur les pratiques de votre programme incorporant le coût de la période ?</li></td>
  </tr>
  <tr> 
   <td>Calendrier marketing (le cas échéant)</td> 
   <td><li>Combien y a-t-il de <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">types d’entrée de calendrier</a> ? Sont-ils toujours pertinents ?</li></td>
  </tr>
 </tbody> 
</table>

## Gestion de la base de données {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Gestion des champs</td> 
   <td><li>Combien de champs y a-t-il ? 
   <br/>     Cliquez sur <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Exporter les noms de champ</a> pour consulter la liste de vos champs, champs personnalisés et noms d’API.</li>
<li>Combien y a-t-il de <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">champs personnalisés</a> ?</li>
<li>Combien de champs sont utilisés ? 
<br/>     Sélectionnez <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Exporter utilisé par</a> dans la liste déroulante Actions de champ pour passer en revue les ressources associées d’un champ.</li>
<li>Combien de champs sont synchronisés entre Marketo Engage et votre CRM ?</li>
<li>Les champs CRM sont-ils synchronisés avec les objets appropriés ?</li>
<li>Existe-t-il un <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">jeu de vues personnalisé</a> pour les détails de personne ? Devrait-il y en avoir ?</li>
<li>Disposez-vous d’une convention d’affectation des noms pour vos champs en fonction de la source ? 
<br/>     Si ce n’est pas le cas, envisagez d’implémenter cette méthode.</li>
<li>Existe-t-il des champs <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">bloqués</a> ? 
<br/>     Si c'est le cas, veillez à comprendre pourquoi.</li></td>
  </tr>
  <tr> 
   <td>Activités personnalisées</td> 
   <td><li>Existe-t-il des <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">activités personnalisées</a> ?
<br/>     Si tel est le cas, cliquez dessus pour comprendre les activités qui ne sont pas liées à un formulaire Marketo, un email ou une landing page.</li></td>
  </tr>
  <tr> 
   <td>Objets personnalisés</td> 
   <td><li>Combien d'<a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">objets personnalisés</a> y a-t-il ? Comment sont-ils synchronisés avec votre CRM ?</li>
<li>Comment ces objets personnalisés sont-ils utilisés par vos programmes et requêtes de liste ?</li></td>
  </tr>
 </tbody> 
</table>

## E-mail {#email}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Paramètres par défaut des emails</td> 
   <td><li>Dans Admin &gt; Email, tous vos paramètres par défaut sont-ils à jour (par exemple, <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">"à partir de" email/libellé</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">domaine de marque</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">message de désabonnement</a>, etc.) ?</li></td>
  </tr>
 </tbody> 
</table>

## Intégrations {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>À quel CRM synchronisez-vous ? Salesforce ? MS Dynamics ? Veeva ?</li>
<li>Utilisez-vous une <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">synchronisation personnalisée</a> ?</li>
<li>[Salesforce uniquement] Votre instance a-t-elle implémenté des filtres de synchronisation personnalisés ? 
<p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : Contactez le support Marketo pour identifier les filtres de synchronisation personnalisés ou demander qu’une règle de synchronisation personnalisée soit implémentée.</li></td>
  </tr>
  <tr> 
   <td>Pages de destination</td> 
   <td><li>Quel est le <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">domaine défini sur</a> ?</li>
   <li>En quoi consiste la page d’accueil ?</li>
<li>Quel est le <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">jeu de secours en tant que</a> ?</li>
<li>Le préremplissage de formulaire est-il activé ?</li>
<li><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">Les URL personnalisées</a> sont-elles activées ?</li>
<li>Existe-t-il des règles configurées pour les <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">redirections</a> ?</li>
<li>Avez-vous des alias de domaine en place ? Effectuez-vous le suivi de la manière dont vous utilisez vos alias de domaine ?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">Domaines sécurisés pour les pages d’entrée</a> est-il activé ? 
<br/>     Confirmez si les ressources de votre landing page contiennent une URL "http".</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Votre <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">code de suivi Munchkin</a> se trouve-t-il sur votre site web (et non sur une page d’entrée de Marketo Engage) ?</li>
<li>Une requête de navigateur <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Do Not Track</a> est-elle activée ?</li>
<li>Votre <a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/javascriptapi/lead-tracking.html" target="_blank">API Munchkin</a> est-elle configurée ? 
<p><img src="assets/tip-icon.png" alt="icône de bulle">CONSEIL : si vous ne disposez pas de documentation sur l’emplacement du code de la serviette sur votre site web, vous pouvez afficher toutes les URL en créant un <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">rapport d’activité de la page web</a>.</li></td>
  </tr>
  <tr> 
   <td>Services Web</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">Restrictions d’IP</a> sont-elles activées ? Devraient-ils l'être ?</li>
<li>Quels utilisateurs/applications effectuent des appels API dans votre instance ?</li>
<li>Êtes-vous en train d’atteindre ou êtes-vous sur le point d’atteindre votre limite d’API ?
<br/>     Si tel est le cas, envisagez d’augmenter ou de contrôler votre instance pour réduire ces appels d’API.</li></td>
  </tr>
  <tr> 
   <td>Adobe Dynamic Chat (le cas échéant)</td> 
<td>Suivez les étapes ci-dessous pour accéder à <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. Si vous n'avez pas encore configuré Adobe ID, <a href="https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html" target="_blank">apprenez à le faire ici</a>.
<br/>
<li>Avez-vous accepté l’invitation <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Dynamic Chat Product Admin</a> ? L’e-mail est envoyé lorsque Dynamic Chat est activé dans votre instance de Marketo Engage et que vous êtes désigné comme administrateur système.
<br/>     Dans le cas contraire, recherchez l’e-mail de bienvenue dans votre boîte de réception et acceptez l’invitation à configurer votre Adobe ID.</li>   
<li>Avez-vous ajouté les <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">utilisateurs souhaités</a> au profil de produit du Dynamic Chat dans Adobe Admin Console ?
<li>Assurez-vous que le profil de produit du Dynamic Chat est ajouté à l’identité de l’Adobe de vos utilisateurs éligibles. Vous ne pouvez pas affecter de rôles "Dynamic Chat d’accès" dans Marketo Engage &gt; Admin &gt; Utilisateurs et rôles s’ils sont ajoutés à un profil de produit.</li>
<li>Dans l’onglet "Profils de produit", les autorisations de profil par défaut sont-elles alignées sur les besoins de votre entreprise ?<br/> 
Dans le cas contraire, modifiez les autorisations du profil spécifique. </li>
<li>Si vous disposez de plusieurs abonnements, vos utilisateurs sont-ils ajoutés aux bons abonnements ?</li>
<br>
Une fois le contrôle des paramètres Utilisateurs et rôles terminé, connectez-vous à Dynamic Chat pour poursuivre votre audit.  
<li>Avez-vous <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">connecté votre instance de Marketo Engage</a> à Dynamic Chat ?</li>
<li>Les cinq profils par défaut avec des autorisations prédéfinies sont-ils applicables à votre organisation ?<br/> 
     Dans le cas contraire, vous pouvez <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">les modifier en Dynamic Chat</a>. Vous pouvez également <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">créer un profil personnalisé</a> avec un jeu personnalisé d’autorisations.</li>
<li>Pour permettre à vos utilisateurs d’accéder à Dynamic Chat, avez-vous coché "Dynamic Chat d’accès" sur le rôle de Marketo Engage approprié sous Admin &gt; Utilisateurs et rôles &gt; Rôles ?
<br/><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : Les rôles "Admin" et "Utilisateur marketing" doivent avoir accès au Dynamic Chat.</li>
</td>
  </tr>
  <td>Marketo Sales Insight (le cas échéant)</td> 
   <td><li>Le <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">package MSI a-t-il été installé</a> ?</li>
<li>Avez-vous <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">effectué une mise à niveau vers la dernière version de Sales Insight</a> ?</li>
<li>Avez-vous terminé la configuration de Sales Insight ? <br/>     Utilisateurs d'Enterprise/d'Unlimited <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">, cliquez ici</a>, utilisateurs professionnels <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">, cliquez ici</a>.</li>
<li>Avez-vous <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">donné l'accès à vos utilisateurs</a> en fonction du nombre de sièges que vous avez achetés ?</li>
<li><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Étoiles et flammes</a> sont-elles personnalisées ?</li></td>
  </tr>
  <tr> 
   <td>Point de lancement (le cas échéant)</td> 
   <td><li>Quels services avez-vous configuré (par exemple, <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a>, etc.) ? Est-ce qu'il y en a qui approchent de leur expiration ?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Combien d’appels API</a> vos intégrations utilisent-elles ?</li>
<li>Disposez-vous des intégrations appropriées pour vos cas d’utilisation ?</li></td>
  </tr>
  <tr> 
   <td>Webhooks (le cas échéant)</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Quelles connexions</a> avez-vous configurées ?</li>
<li>N’est-il plus utilisé ?</li></td>
  </tr>
  <tr> 
   <td>Applications mobiles (le cas échéant)</td> 
   <td><li>Quelles <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">applications mobiles</a> avez-vous ?</li>
<li>Des <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">appareils de test</a> ont-ils été ajoutés ?</li></td>
  </tr>
 </tbody> 
</table>

## Coffre au trésor {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Coffre au trésor</td> 
   <td><li>Qu'est-ce qui est activé dans la <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">Poitrine au trésor</a> ?</li>
<li>Certaines fonctionnalités doivent-elles être activées ou désactivées ?</li></td>
  </tr>
  <tr> 
   <td>Inspecteur de campagne</td> 
   <td><li><a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Inspecteur de campagne</a> est-il activé ?
<br/>Si ce n'est pas le cas, envisagez de l'activer pour identifier facilement les campagnes : actives, synchronisées avec votre CRM et/ou supprimant des enregistrements.</li></td>
  </tr>
 </tbody> 
</table>

## Alertes et mises à jour {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th>
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Mises à jour de l’état du Marketo Engage</td> 
   <td><li>Votre instance est-elle abonnée aux <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">mises à jour de l’état du Marketo Engage</a> ?</li></td>
  </tr>
  <tr> 
   <td>Alertes</td> 
   <td><li>Y a-t-il des <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">alertes actives</a> envoyées à des équipes internes depuis Marketo Engage ?</li>
<li>Si oui, ces alertes fonctionnent-elles correctement ?</li></td>
  </tr>
  <tr> 
   <td>Notifications</td> 
   <td><li>Êtes-vous abonné à l'administrateur approprié <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">notifications</a> ?</li></td>
  </tr>
 </tbody> 
</table>
