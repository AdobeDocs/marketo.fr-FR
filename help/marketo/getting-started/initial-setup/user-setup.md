---
description: Avant de vous plonger dans votre nouvelle instance de Marketo Engage, vous devez suivre quelques étapes fondamentales pour une utilisation continue. Ces étapes incluent la configuration du compte utilisateur, la configuration de l’administrateur et l’abonnement aux mises à jour système en cours.
short-description: Après avoir terminé les étapes de configuration initiales, apprenez à établir des éléments fondamentaux pour garantir une utilisation continue fluide.
title: Liste de contrôle de configuration de l’utilisateur
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 384740fdfc1f6950369116bd77ee49f9e745bdf1
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Liste de contrôle de configuration de l’utilisateur {#user-setup-checklist}

Maintenant que vous avez terminé toutes les [étapes de configuration initiales](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"}, il est temps d’établir quelques éléments fondamentaux pour garantir une utilisation continue fluide. Cela préparera le terrain pour votre parcours avec Marketo Engage et vous aidera à tirer le meilleur parti de ses fonctionnalités. Commençons !

>[!NOTE]
>
>Vous pouvez également télécharger cette liste de contrôle, [ avec une liste des bonnes pratiques](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) pour votre nouvelle instance, et vérifier les étapes au fur et à mesure.

## Marketo Engage sur Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

Vos nouveaux abonnements de Marketo Engage sont intégrés à [Adobe Identity Management System (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html). Passez à la révision de gestion des utilisateurs suivante dans Adobe Admin Console.

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administration des produits d’abonnement et de Marketo Engage</td>
    <td><li>Vérifiez que l’administrateur système de votre organisation d’Adobe vous a accordé un rôle d’administrateur de produit Adobe.</li> 
    <ul>
    <li>Contactez l’équipe Compte d’Adobe (votre gestionnaire de compte) ou envoyez un e-mail à <code>marketocares@marketo.com</code> pour savoir qui, au sein de votre organisation, dispose des privilèges <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html"> d’administrateur système Adobe Admin Console</a>.</li></ul>
    <li>Acceptez l’invitation "Administrateur de produit Marketo Engage" pour activer votre Adobe ID. L’ <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">e-mail de bienvenue</a> est envoyé lorsque le rôle est attribué dans Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Profils de produit</td>
    <td><li>Affectez tous les utilisateurs de votre choix au <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">profil de produit</a> du Marketo Engage dans Adobe Admin Console.</li>
    <ul>
    <li>Vous ne pouvez pas affecter les rôles des utilisateurs dans Marketo Engage &gt; Admin &gt; Utilisateurs et rôles avant de les ajouter à un profil de produit.</li>
    <li>Chaque abonnement sera un profil de produit autonome. Si un utilisateur indésirable est ajouté à plusieurs profils de produit (par exemple, environnement de test et de production), vous devez supprimer l’utilisateur de tous les profils de produit. Sinon, ils auront toujours accès au Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Utilisateurs et utilisatrices</td>
    <td><li>Créez une stratégie indiquant quand <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">créer un utilisateur</a>.</li> <li>Créez une stratégie indiquant à quel moment supprimer des utilisateurs.</li>
    <li>Déterminez qui doit disposer des <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">autorisations d’administrateur système Adobe et d’administrateur produit Marketo Engage.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Ajoutez des utilisateurs</a> au profil de produit souhaité.</li>
    <li>Créez un utilisateur API pour chaque cas d’utilisation d’API.</li></td>
  </tr>
  <tr>
    <td>API User Management (le cas échéant)</td>
    <td><li>Utilisez l’ <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html"> API de gestion des utilisateurs Adobe</a> pour inviter, mettre à jour et supprimer des utilisateurs.</li>
    <li>Utilisez l’ <a href="https://developer.adobe.com/umapi/"> API de gestion des utilisateurs d’Adobe </a> pour ajouter ou supprimer des rôles (par exemple, administrateurs, administrateurs de support, développeurs).</li>
    </td>
  </tr>
  <tr>
    <td>Administrateur de support produit</td>
    <td><li>Pour <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">envoyer un ticket d’assistance dans Adobe Admin Console</a>, vous devez avoir le rôle 'Administrateur du support produit' attribué par un administrateur système aux abonnements que vous gérez. Seul un administrateur système de votre entreprise peut <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">vous affecter à ce rôle</a>.</li>
    <li>Vous avez peut-être reçu un courrier électronique de l’administrateur système vous indiquant que vous êtes l’administrateur du support pour votre abonnement de Marketo Engage. Si tel est le cas, cliquez sur <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">'Commencer'</a> dans le courrier électronique pour rejoindre l’organisation.</li>
    <li>Déterminez les contacts appropriés (avec au moins un contact de sauvegarde) et demandez à l’administrateur système d’attribuer le rôle d’administrateur du support produit en conséquence.</li></td>
  </tr>
</tbody>
</table>

## Dynamic Chat dans la configuration Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Pour utiliser [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html), le canal d’automatisation des conversations natif en Marketo Engage, passez à la configuration des autorisations d’utilisateur en suivant les étapes ci-dessous dans [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}.

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administration des produits d’abonnement et de Dynamic Chat (le cas échéant)</td>
    <td><li>Vérifiez que l’administrateur système de votre organisation d’Adobe vous a accordé un rôle d’administrateur de produit Adobe.</li> 
    <ul><li>Contactez l’équipe Compte d’Adobe (votre gestionnaire de compte) ou envoyez un e-mail à <code>marketocares@marketo.com</code> pour savoir qui, au sein de votre organisation, dispose des privilèges <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html"> d’administrateur système Adobe Admin Console</a>.</li></ul>
    <li>Acceptez l’invitation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">’Dynamic Chat Product Admin'</a>. L’ <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html"> e-mail de bienvenue</a> est envoyé lorsque Dynamic Chat est activé dans votre instance de Marketo Engage et que vous êtes désigné comme administrateur système.</li></td>
  </tr>
  <tr>
    <td>Profils de produit</td>
    <td><li>Affectez tous les utilisateurs souhaités au profil de produit du Dynamic Chat dans Adobe Admin Console.</li> 
    <ul>
    <li>Si un utilisateur indésirable est ajouté à plusieurs profils de produit, vous devez le supprimer de tous les profils de produit. Sinon, ils auront toujours accès au Dynamic Chat.</li>
    <li>Vous pouvez <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">modifier les profils de produit en Dynamic Chat</a> et créer un profil personnalisé avec un ensemble personnalisé d’autorisations <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions"> disponibles dans votre abonnement</a>.</li></td>
  </tr>
  <tr>
    <td>Utilisateurs et utilisatrices</td>
    <td><li>Créez une stratégie indiquant à quel moment ajouter et supprimer un utilisateur de conversation.</li>
    <li>Créez une stratégie pour savoir qui doit disposer des <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">autorisations d’administrateur de produit par Adobe Dynamic Chat.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Ajoutez des utilisateurs au profil de produit souhaité</a>.</li></td>
  </tr>
</tbody>
</table>

## Configuration des mises à jour système et des communications en cours {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Mises à jour de l’état Marketo des Adobes</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Abonnez-vous aux mises à jour de l’état Adobe Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Notifications</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Abonnez-vous aux notifications d’administration</a> pour tout problème critique tel que les erreurs dans vos campagnes dynamiques et les problèmes critiques liés à la synchronisation CRM.</li></td>
  </tr>
</tbody>
</table>

<p>

Maintenant que votre compte de Marketo Engage est prêt, consultez notre section [Bonnes pratiques pour une nouvelle instance de Marketo Engage](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"} pour tirer le meilleur parti de votre investissement et vous préparer à une réussite à long terme.
