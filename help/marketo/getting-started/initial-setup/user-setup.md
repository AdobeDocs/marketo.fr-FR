---
description: Avant de vous lancer dans la création de votre nouvelle instance Marketo Engage, suivez ces quelques étapes fondamentales qui assureront la continuité de votre utilisation. Ces étapes incluent la configuration du compte d’utilisation, la configuration de l’administration de support et l’abonnement aux mises à jour du système en cours.
short-description: Après avoir terminé les étapes de configuration initiales, vous apprendrez à définir les éléments fondamentaux qui assureront la fluidité et la continuité de votre utilisation.
title: Liste de contrôle de la configuration utilisateur
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 7%

---

# Liste de contrôle de la configuration utilisateur {#user-setup-checklist}

Maintenant que vous avez terminé toutes les [étapes de configuration initiales](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"}, il est temps d’établir certains éléments fondamentaux pour assurer une utilisation continue et fluide. Cela jettera les bases de votre parcours avec Marketo Engage et vous aidera à tirer le meilleur parti de ses fonctionnalités. C’est parti !

>[!NOTE]
>
>Vous pouvez également télécharger cette liste de contrôle, [ainsi qu’une liste des bonnes pratiques](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) pour votre nouvelle instance, et vérifier les étapes au fur et à mesure.

## Marketo Engage sur Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

Vos nouveaux abonnements Marketo Engage ont été intégrés à [Adobe Identity Management System (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html). Passez à la révision suivante de la gestion des utilisateurs dans Adobe Admin Console.

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administrateur de produit d’abonnement et de Marketo Engage</td>
    <td><li>Vérifiez que votre administrateur système d’organisation Adobe vous a accordé le rôle d’administrateur de produit Adobe.</li>
    <ul>
    <li>Contactez l’équipe du compte Adobe (votre gestionnaire de compte) ou envoyez un e-mail à <code>marketocares@marketo.com</code> pour savoir qui, au sein de votre organisation, dispose des privilèges <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Administrateur système Adobe Admin Console</a>.</li></ul>
    <li>Acceptez l’invitation « Marketo Engage Product Admin » pour activer votre Adobe ID. L’<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">e-mail de bienvenue</a> est envoyé lorsque le rôle est attribué dans le Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Profils de produit</td>
    <td><li>Affectez tous les utilisateurs souhaités au Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">profil de produit</a> dans Adobe Admin Console.</li>
    <ul>
    <li>Vous ne pouvez pas affecter les rôles des utilisateurs dans Marketo Engage &gt; Admin &gt; Utilisateurs et rôles avant de les ajouter à un profil de produit.</li>
    <li>Chaque abonnement sera un profil de produit autonome. Si un utilisateur indésirable est ajouté à plusieurs profils de produit (par exemple, sandbox de production et de test), vous devez le supprimer de tous les profils de produit. Sinon, ils auront toujours accès à Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Utilisateurs et utilisatrices</td>
    <td><li>Créez une politique sur le moment <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">créer un utilisateur</a>.</li> <li>Créez une politique sur le moment où supprimer des utilisateurs et utilisatrices.</li>
    <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : vous devez être un administrateur système pour supprimer des utilisateurs.
    <li>Déterminez qui doit disposer des autorisations d’administrateur système Adobe et d’administrateur de produit Marketo Engage <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html"></a>. <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Ajoutez des utilisateurs</a> au profil de produit souhaité.</li>
    <li>Créez un utilisateur d’API pour chaque cas d’utilisation d’API.</li></td>
  </tr>
  <tr>
    <td>API User Management (le cas échéant)</td>
    <td><li>Utilisez l’API <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">Adobe User Management</a> pour inviter, mettre à jour et supprimer des utilisateurs.</li>
    <li>Utilisez l’API <a href="https://developer.adobe.com/umapi/">Adobe User Management</a> pour ajouter ou supprimer des rôles (par exemple, administrateurs, administrateurs de l’assistance, développeurs).</li>
    </td>
  </tr>
  <tr>
    <td>Administrateur du support produit</td>
    <td><li>Pour <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">envoyer un ticket d’assistance dans Adobe Admin Console</a>, le rôle « Administrateur de l’assistance produit » doit être attribué par un administrateur système aux abonnements que vous gérez. Seul un administrateur système de votre entreprise peut <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">vous affecter à ce rôle</a>.</li>
    <li>Il se peut que vous ayez reçu un e-mail de l’administrateur système vous indiquant que vous êtes l’administrateur de l’assistance pour votre abonnement Marketo Engage. Si tel est le cas, cliquez sur <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">'Commencer'</a> dans l'e-mail pour rejoindre l'organisation.</li>
    <li>Déterminez les contacts appropriés (avec au moins un contact de sauvegarde) et demandez à l’administrateur système d’affecter le rôle d’administrateur du support produit en conséquence.</li></td>
  </tr>
</tbody>
</table>

## Configuration de Dynamic Chat sur Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Pour utiliser [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html), le canal d&#39;automatisation de conversation natif dans Marketo Engage, procédez à la configuration des autorisations utilisateur en suivant les étapes ci-dessous dans [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}.

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administrateur du produit Abonnement et Dynamic Chat (le cas échéant)</td>
    <td><li>Vérifiez que votre administrateur système d’organisation Adobe vous a accordé le rôle d’administrateur de produit Adobe.</li>
    <ul><li>Contactez l’équipe du compte Adobe (votre gestionnaire de compte) ou envoyez un e-mail à <code>marketocares@marketo.com</code> pour savoir qui, au sein de votre organisation, dispose des privilèges <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Administrateur système Adobe Admin Console</a>.</li></ul>
    <li>Acceptez l’invitation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">’Administrateur de produit Dynamic Chat’</a>. L’<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">e-mail de bienvenue</a> est envoyé lorsque Dynamic Chat est activé dans votre instance Marketo Engage et que vous êtes désigné comme administrateur système.</li></td>
  </tr>
  <tr>
    <td>Profils de produit</td>
    <td><li>Affectez tous les utilisateurs souhaités au profil de produit du Module de conversation dynamique dans Adobe Admin Console.</li>
    <ul>
    <li>Si un utilisateur indésirable est ajouté à plusieurs profils de produit, vous devez le supprimer de tous les profils de produit. Sinon, ils auront toujours accès à Dynamic Chat.</li>
    <li>Vous pouvez <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">modifier les profils de produit dans Dynamic Chat</a> et créer un profil personnalisé avec un ensemble personnalisé d’autorisations <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">disponibles dans votre abonnement</a>.</li></td>
  </tr>
  <tr>
    <td>Utilisateurs et utilisatrices</td>
    <td><li>Créez une politique sur le moment où ajouter et supprimer un utilisateur de conversation.</li>
    <li>Créez une politique sur les personnes qui doivent disposer des autorisations d’administrateur de produit <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Ajoutez des utilisateurs au profil de produit souhaité</a>.</li></td>
  </tr>
</tbody>
</table>

## Configurer les communications et mises à jour système en cours {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Mises à jour du statut d’Adobe Marketo</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Abonnement aux mises à jour du statut de Adobe Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Notifications</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Abonnez-vous aux notifications des administrateurs</a> en cas de problèmes critiques tels que des erreurs dans vos campagnes intelligentes et des problèmes critiques détectés avec la synchronisation CRM.</li></td>
  </tr>
</tbody>
</table>

<p>

Maintenant que votre compte Marketo Engage est prêt, veuillez consulter notre section [ Bonnes pratiques pour une nouvelle instance Marketo Engage ](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"} pour tirer le meilleur parti de votre investissement et vous configurer pour une réussite à long terme.
