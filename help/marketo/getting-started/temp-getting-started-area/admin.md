---
description: NOUVELLE ZONE - Documents Marketo - Documentation du produit
title: NOUVELLE ZONE
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 7d8cdb2da42769ee0326a3d585ad32a3405dfac1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 8%

---

# NOUVELLE ZONE : Liste de contrôle de l’administrateur {#new-area-admin-checklist}

Texte d’introduction.

## Rôles {#roles}

<table>
<thead>
  <tr>
    <th>Zone </th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rôles </td>
    <td><li>Vérifiez les rôles prédéfinis et vérifiez les autorisations/accès à chaque rôle.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Création d’un nouveau rôle</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">modification des rôles</a> selon les besoins de votre entreprise et la fréquence de connexion des utilisateurs.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Affecter des utilisateurs aux rôles appropriés</a>.</li>
    <li>Après avoir affecté les rôles des utilisateurs, passez en revue le nombre d’utilisateurs par rôle.</li>  <li>Implémentez un rôle unique pour chaque utilisateur de l’API pour faciliter la résolution des problèmes.</li></td>
  </tr>
  <tr>
    <td>Documentation </td>
    <td>Définissez les utilisateurs et les rôles de votre organisation. <br>Définissez votre processus d’ajout d’un nouvel utilisateur/administrateur. </td>
  </tr>
  <tr>
    <td>Environnement de test (le cas échéant) </td>
    <td>Vérifiez les catégories ci-dessus pour votre environnement de test si vous en avez une. </td>
  </tr>
</tbody>
</table>

## Espaces de travail et partitions {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espaces de travail et partitions </td>
    <td><li>Déterminer le nombre de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> espaces de travail</a> et/ou partitions dont votre organisation a besoin et <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">combien d’utilisateurs ont accès à chaque espace de travail.</a></li>
    <li>Définissez l’objectif principal de chaque espace de travail et partition.</li>
    <li>Définissez la relation entre vos espaces de travail et vos partitions.</li></td>
  </tr>
  <tr>
    <td>Documentation </td>
    <td><li>Documentez comment les espaces de travail sont définis et comment cela se rapporte-t-il aux partitions de base de données (c’est-à-dire un espace de travail global qui voit tout le monde, par rapport aux secteurs d’activité).</li>
    <li>Importez de nouveaux enregistrements dans la partition appropriée.</li>
    <li>Définissez la valeur dans le CRM qui place les utilisateurs dans la partition appropriée.</li></td>
  </tr>
</tbody>
</table>

## Paramètres de la campagne intelligente {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Paramètres de la campagne intelligente </td>
    <td><li>Ajouter un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">restriction sur la taille de campagne dynamique</a>, empêchant l’envoi accidentel de l’ensemble de la base de données par courrier électronique.</li>
    <li>Activation des restrictions pour les personnes dans les campagnes dynamiques</li></td>
  </tr>
</tbody>
</table>

## Paramètres d’e-mail {#email-settings}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Valeurs par défaut des emails</td>
    <td><li>Sous Domaine de marque, sélectionnez votre domaine et ajoutez votre CNAME de messagerie. Cette valeur doit être au format suivant : [EmailTrackingCNAME].[CompanyDomain].com.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Configuration de SPF et DKIM</a> pour la délivrabilité des emails.</li></td>
  </tr>
</tbody>
</table>

## Limites de communication {#communication-limits}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limites de communication</td>
    <td><li>Placer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Limites de communication</a>.</li>
    <li>Déterminez si votre entreprise a besoin d’une stratégie sur les limites de communication.</li></td>
  </tr>
</tbody>
</table>

## Balises {#tags}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canaux</td>
    <td><li>Définition de l’utilisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">channels</a>.</li></td>
  </tr>
  <tr>
    <td>Balises </td>
    <td><li>Définition de l’utilisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">tags</a>.</li></td>
  </tr>
  <tr>
    <td>Calendrier (le cas échéant) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Assertions du calendrier marketing des problèmes</a> à ceux qui ont besoin d’accès.</li> 
    <li>Configuration <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Calendrier</a>.</li></td>
  </tr>
</tbody>
</table>

## Gestion de la base de données {#database-management}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gestion des champs</td>
    <td><li>Mettre en oeuvre la convention d’affectation des noms pour <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">champs personnalisés.</a> Par exemple, commencez par "MKTO".</li>
    <li>Soyez sélectif au sujet des champs que vous synchronisez. Plus vous synchronisez de champs, plus le cycle de synchronisation sera lent.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">Bloquer les mises à jour des champs</a> vous souhaitez écrire une seule fois (c’est-à-dire la source de piste d’origine, les détails de la source de piste d’origine, les champs de gestion dynamique des balises Première touche, etc.).</li></td>
  </tr>
  <tr>
    <td>Activités personnalisées </td>
    <td><li>Définir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank" rel="noopener noreferrer">Activités personnalisées</a> qui sont spécifiques à votre entreprise.</li></td>
  </tr>
  <tr>
    <td>Objets personnalisés </td>
    <td><li>Vérifiez combien de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank" rel="noopener noreferrer">Objets personnalisés</a> vous avez besoin.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank" rel="noopener noreferrer">Synchroniser ces objets personnalisés avec votre gestion de la relation client</a>.</li></td>
  </tr>
</tbody>
</table>

## Intégrations {#integrations}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Lancer la synchronisation CRM. Choisissez l’un des éléments suivants, en fonction du CRM utilisé par votre entreprise : <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank" rel="noopener noreferrer">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank" rel="noopener noreferrer">Microsoft Dynamics</a>.</li>
    <li>Identifiez le type d'accès dont vous avez besoin pour accéder à votre CRM.</li>
    <li>Identifiez votre administrateur CRM pour le dépannage.</li></td>
  </tr>
  <tr>
    <td>Sales Insight (le cas échéant)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank" rel="noopener noreferrer">Configurez Sales Insight.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank" rel="noopener noreferrer">Donnez des sièges aux utilisateurs appropriés.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank" rel="noopener noreferrer">Configuration de l’API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank" rel="noopener noreferrer">Personnalisez les scores de piste.</a></li></td>
  </tr>
</tbody>
</table>
