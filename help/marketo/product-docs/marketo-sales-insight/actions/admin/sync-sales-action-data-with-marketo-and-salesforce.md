---
description: Synchroniser les données de ventes avec Marketo et Salesforce - Documentation de Marketo - Documentation du produit
title: Synchroniser les données d’action des ventes avec Marketo et Salesforce
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 4%

---

# Synchroniser les données d’action des ventes avec Marketo et Salesforce {#sync-sales-action-data-with-marketo-and-salesforce}

La synchronisation des champs d’unification des données pour les actions de Sales Insight permet au système d’extraire des informations sur la personne de votre base de données Marketo Engage vers votre base de données d’actions de Sales Insight.

Cela fournit des données de personne à jour dans l’application web Actions de Sales Insight et permet au système de collecter des identifiants uniques pour les enregistrements de personne correspondants dans Marketo et les enregistrements de prospect/contact/compte/opportunité dans Salesforce, de sorte que les enregistrements puissent être correctement référencés pour les données de journalisation.

Cette synchronisation peut être activée à partir de l’onglet Configuration des actions Sales Insight dans la section Admin de Marketo Engage. Pour plus d’informations, consultez la section [ Lancement de la synchronisation des données ](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Le diagramme ci-dessus montre comment les données d&#39;activité et de tâche des personnes peuvent se synchroniser entre les systèmes. Quelques points à noter :

* Les enregistrements de personnes sont synchronisés avec les actions Sales Insight à partir de Marketo Engage, ce qui fait de Marketo Engage la source de vérité pour les données de personnes Sales Insight Actions
* Les actions Marketo Engage et Sales Insight [disposent toutes deux d’un mécanisme](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) permettant de collecter et de synchroniser le statut de désabonnement avec Salesforce
* Le statut de désabonnement n&#39;est pas synchronisé des actions de vente vers Marketo Engage, mais les actions de vente Insight peuvent être configurées pour vérifier le statut de désabonnement Marketo des personnes avant de permettre aux vendeurs d&#39;envoyer un e-mail avec la vérification de désabonnement de [Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Vous trouverez ci-dessous quelques questions fréquentes relatives au fonctionnement de la synchronisation d’unification des données.

## Quels leads/contacts sont synchronisés avec les actions de Sales Insight ? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Les leads et les contacts auxquels un commercial est affecté seront synchronisés dans les actions de vente.

Vous pouvez déterminer si un prospect/contact a un commercial dans Salesforce en examinant le champ standard du propriétaire qui existe.

Le propriétaire des ventes n’a pas besoin d’être l’utilisateur de synchronisation Marketo ou un utilisateur Salesforce ou commercial spécifique. Tout ce dont nous avons besoin, c’est d’un utilisateur répertorié dans le champ Propriétaire du prospect et Propriétaire du contact répertorié dans Salesforce, afin que nous puissions l’identifier en tant que prospect commercial et le synchroniser dans les actions Sales Insight. Toutes les mises à jour des champs avec lesquels nous effectuons la synchronisation seront également détectées et mises à jour dans les actions Sales Insight.

## D’où proviennent les données d’activité affichées dans la grille intelligente de Sales Insight ? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Les données d’activité telles que l’e-mail, l’appel, le moment intéressant et le web, proviennent toutes de la base de données Marketo Engage. La grille dynamique Sales Insight effectue une requête à l’instance Marketo Engage pour récupérer cette information chaque fois qu’un commercial charge le panneau Sales Insight.

![](assets/actions-data-sync-faq-4.png)

Pour que toutes les données d’activité puissent provenir de Marketo Engage, les actions Sales Insight synchronisent toutes les données d’activité avec Marketo Engage.

## Quels champs liés à la synchronisation des enregistrements des personnes de Marketo Engage vers les actions de Sales Insight ? {#what-fields-sync}

Onze champs se synchronisent entre Marketo Engage et les actions Sales Insight :

* Prénom
* Nom
* ID de contact Salesforce
* ID de lead Salesforce
* ID de compte Salesforce
* ID d’opportunité Salesforce
* ID de Marketo
* Société
* Titre
* E-mail
* Numéro de téléphone
* URL LinkedIn
* Source

## Les champs qui se synchronisent entre Marketo Engage et les actions Sales Insight sont-ils configurables ? {#are-the-fields-that-sync-configurable}

La configuration de la synchronisation des champs Marketo Engage avec les actions Sales Insight n’est pas disponible, pas plus que la possibilité de mapper les champs. La synchronisation à partir de Marketo mappe automatiquement les champs Marketo standard aux champs standard de votre instance de vente.

## Pourquoi les actions Sales Insight possèdent-elles leur propre base de données ? {#why-does-actions-have-its-own-database}

Sales Insight Actions possède sa propre application web avec une base de données de personnes et d’activités dédiée afin de fournir un espace de travail optimisé conçu pour les équipes commerciales. Cela permet aux responsables des ventes et aux vendeurs de disposer d’un espace pour élaborer et gérer leur stratégie d’engagement   sans accorder d’accès ou de privilèges à l’espace de travail Marketo Engage principal, optimisé pour les spécialistes des opérations marketing.

## Comment les doublons sont-ils gérés ? {#how-are-duplicates-handled}

Votre base de données Actions de vente sera une copie des personnes qualifiées (leads/contacts avec un commercial) qui existent dans votre base de données Marketo Engage. Cela signifie que si deux enregistrements ont la même adresse e-mail et sont créés dans Marketo, un enregistrement en double sera créé dans les actions vente.

## Combien de temps faut-il pour que la synchronisation initiale se termine ? {#how-long-initial-sync}

Le processus initial de synchronisation de toutes vos données de prospect commercial dans une nouvelle instance Sales Insight Actions traite généralement les personnes à environ 1 000 toutes les 1 à 2 minutes. Il s’agit simplement d’une estimation qui peut varier.

Une fois que la synchronisation initiale a eu lieu et que tous vos prospects ont été renseignés dans votre instance d’application web Sales Insight Actions, une synchronisation incrémentielle s’exécute chaque fois qu’une mise à jour d’un des champs pris en charge est synchronisée.

## Les utilisateurs des actions de Sales Insight peuvent-ils modifier les données des personnes à partir de l’application web Actions ? {#can-actions-users-edit-people-data}

Non, la possibilité de créer et de modifier des enregistrements de personnes dans Actions n’est pas disponible à la fois pour les utilisateurs et les administrateurs de l’application web Actions. La création et la modification des personnes doivent être effectuées dans Salesforce ou Marketo Engage. Les actions Sales Insight utilisent Marketo comme source de vérité pour les données des personnes en synchronisant en permanence les nouvelles données. Ainsi, si une personne est mise à jour ou créée dans Marketo à partir d’un workflow dans Marketo ou synchronisée à partir de Salesforce, ces mises à jour sont transmises à la base de données d’applications web Sales Insight Actions.

## Les activités de vente se connectent-elles à Marketo ? {#do-sales-activities-log-to-marketo}

Oui, les activités d’engagement commercial seront enregistrées dans Marketo en tant qu’activités natives. Ces activités incluent également des filtres natifs qui peuvent être utilisés avec des contraintes pour cibler les prospects en fonction des attributs de l’activité de vente.

![](assets/actions-data-sync-faq-5.png)

Vous trouverez ci-dessous une liste des activités qui se connectent à Marketo :

* Envoyer un e-mail de vente
* Ouvrir l’e-mail commercial
* Cliquer sur l’e-mail commercial
* A répondu à l&#39;e-mail commercial
* E-mail de vente renvoyé
* Appel de vente reçu
* Ajouter à la campagne de ventes
* Supprimé de la campagne SFDC

## Les activités de vente se connectent-elles à Salesforce ? {#do-sales-activities-log-to-salesforce}

Oui, les activités d’engagement commercial seront enregistrées dans Salesforce en tant que tâches natives. Ces tâches peuvent ensuite être utilisées dans les rapports Salesforce pour alimenter les tableaux de bord de l’équipe qui effectuent le suivi des activités de vente.

Les actions Sales Insight permettent aux administrateurs de configurer les activités de vente consignées dans Salesforce. Ces activités comprennent les e-mails, les appels et les tâches de rappel ouvertes.

![](assets/actions-data-sync-faq-6.png)

Le diagramme ci-dessus montre les informations consignées dans Salesforce. Les activités telles que les e-mails et les appels sont consignées dans Salesforce dans une [synchronisation unidirectionnelle](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md). Les [Désabonnements](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) et [Tâches de rappel](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) sont tenus à jour grâce à une synchronisation bidirectionnelle. Chacune de ces synchronisations de données peut être configurée à partir de l’interface de l’application web des actions Sales Insight.

>[!MORELIKETHIS]
>
>* [Synchronisation des désabonnements avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Vérification du désabonnement de Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Synchroniser les activités de vente avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Synchronisation de la tâche de rappel avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Lancer la synchronisation des données](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)
