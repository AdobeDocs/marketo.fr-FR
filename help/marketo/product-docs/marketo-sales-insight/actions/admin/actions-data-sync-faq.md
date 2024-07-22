---
description: FAQ sur la synchronisation des données d’actions - Documents Marketo - Documentation du produit
title: FAQ sur la synchronisation des données d’actions
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 26173379c89393596b3ece18c7f7e945a79588d9
workflow-type: tm+mt
source-wordcount: '1054'
ht-degree: 3%

---

# FAQ sur la synchronisation des données d’actions {#actions-data-sync-faq}

La synchronisation des champs d’unification des données pour les actions Sales Insight permet au système d’extraire des informations sur les personnes de votre base de données de Marketo Engage dans votre base de données Sales Insight Actions.

Cela fournit des données de personnes à jour dans l’application web Actions d’aperçu des ventes et permet au système de collecter des identifiants uniques pour les enregistrements de personne correspondants dans Marketo et les enregistrements de prospect/contact/compte/opportunité dans Salesforce, de sorte que les enregistrements puissent être référencés correctement pour la journalisation des données.

Cette synchronisation peut être activée à partir de l’onglet Configuration des actions d’aperçu des ventes de la section Admin de Marketo Engage. Pour plus d’informations, consultez [Lancer la synchronisation des données](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Le diagramme ci-dessus montre comment l’activité des personnes et les données de tâche peuvent se synchroniser entre les systèmes. Quelques éléments à noter :

* Les enregistrements de personnes sont synchronisés avec les actions d’aperçu des ventes du Marketo Engage, ce qui rend Marketo Engage la source de vérité pour les données des personnes dans les actions d’aperçu des ventes
* Les actions Marketo Engage et Sales Insight [ ont un mécanisme](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) pour collecter et synchroniser l’état de désabonnement à Salesforce
* L’état de désabonnement ne se synchronise pas des actions de vente avec le Marketo Engage, mais les actions de statistiques de vente peuvent être configurées pour vérifier l’état de désabonnement Marketo des personnes avant de permettre aux vendeurs d’envoyer un email avec la [vérification de désabonnement Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Vous trouverez ci-dessous quelques questions fréquentes relatives au fonctionnement de la synchronisation de l’unification des données.

## Quels prospects/contacts sont synchronisés avec les actions Sales Insight ? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Les prospects et les contacts auxquels un propriétaire de vente est affecté seront synchronisés dans les actions de vente.

Vous pouvez voir si un prospect/contact a un propriétaire de vente dans Salesforce en consultant le champ propriétaire standard qui existe.

Le propriétaire des ventes ne doit pas nécessairement être l’utilisateur de synchronisation Marketo ou un utilisateur Salesforce ou commercial spécifique. Tout ce dont nous avons besoin, c’est qu’un utilisateur figure dans le champ Propriétaire du prospect et Propriétaire du contact répertorié dans Salesforce, de sorte que nous puissions l’identifier comme un prospect et le synchroniser dans les actions d’aperçu des ventes. Toutes les mises à jour apportées aux champs avec lesquels nous synchronisons seront également détectées et mises à jour dans les actions Sales Insight.

## D’où proviennent les données d’activité affichées dans la grille dynamique d’aperçu des ventes ? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Les données d’activité telles que l’email, l’appel, le moment intéressant et le web, proviennent toutes de la base de données du Marketo Engage. La grille dynamique d’aperçu des ventes envoie une requête à l’instance du Marketo Engage pour récupérer cette information chaque fois qu’un utilisateur commercial charge le panneau d’aperçu des ventes.

![](assets/actions-data-sync-faq-4.png)

Pour garantir que toutes les données d’activité peuvent être obtenues à partir de Marketo Engage, les actions Sales Insight synchronisent toutes les données d’activité vers Marketo Engage.

## Quels champs liés aux enregistrements de personnes sont synchronisés de Marketo Engage vers les actions Sales Insight ? {#what-fields-sync}

11 champs sont synchronisés de Marketo Engage vers les actions Sales Insight :

* Prénom
* Nom
* Identifiant de contact Salesforce
* Identifiant de prospect Salesforce
* Identifiant de compte Salesforce
* Identifiant d’opportunité Salesforce
* ID de Marketo
* Société
* Titre
* E-mail
* Numéro de téléphone
* URL Linkedin
* Source

## Les champs qui se synchronisent entre les actions Marketo Engage et Sales Insight sont-ils configurables ? {#are-the-fields-that-sync-configurable}

La configuration des champs de Marketo Engage synchronisés avec les actions d’aperçu des ventes n’est pas disponible, pas plus que la possibilité de mapper des champs. La synchronisation à partir de Marketo mappe automatiquement les champs Marketo standard aux champs standard de votre instance d’action commerciale.

## Pourquoi les actions d’aperçu des ventes ont-elles leur propre base de données ? {#why-does-actions-have-its-own-database}

Les actions Sales Insight possèdent leur propre application web avec une base de données dédiée de personnes et d’activités afin de fournir un espace de travail optimisé conçu et conçu pour les équipes commerciales. Cela permet aux responsables commerciaux et aux vendeurs de disposer d’un espace pour élaborer et gérer leur stratégie d’engagement.   sans accorder d’accès ou de privilèges à l’espace de travail principal du Marketo Engage, qui est optimisé pour les spécialistes des opérations marketing.

## Comment les doublons sont-ils traités ? {#how-are-duplicates-handled}

Votre base de données des actions de vente est une copie de ces personnes qualifiées (prospects/contacts avec un propriétaire commercial) qui existent dans votre base de données de Marketo Engage. En d’autres termes, s’il existe deux enregistrements avec la même adresse électronique créée dans Marketo, un enregistrement dupliqué sera créé dans les actions de vente.

## Combien de temps faut-il pour que la synchronisation initiale soit terminée ? {#how-long-initial-sync}

Le processus initial de synchronisation de toutes vos données de piste de vente dans une nouvelle instance d’actions Sales Insight traite généralement les personnes à environ 1 000 toutes les 1 à 2 minutes. Il s’agit simplement d’une estimation qui peut varier.

Une fois la synchronisation initiale effectuée et tous les prospects commerciaux renseignés dans l’instance de l’application web Actions d’aperçu des ventes, il y aura une synchronisation incrémentielle qui s’exécutera chaque fois qu’une mise à jour est effectuée sur l’un des champs pris en charge synchronisés.

## Les utilisateurs des actions Sales Insight peuvent-ils modifier les données des personnes à partir de l’application web Actions ? {#can-actions-users-edit-people-data}

Non, la possibilité de créer et de modifier des enregistrements de personnes dans Actions n’est pas disponible à la fois pour les utilisateurs et les administrateurs de l’application web Actions. La création et la modification de personnes doivent être effectuées dans Salesforce ou dans Marketo Engage. Les actions d’aperçu des ventes utilisent Marketo comme source de vérité pour les données personnelles en synchronisant en permanence de nouvelles données. Ainsi, si une personne est mise à jour ou créée dans Marketo à partir d’un workflow dans Marketo ou synchronisée à partir de Salesforce, ces mises à jour seront transmises à la base de données de l’application web Actions d’aperçu des ventes .

## Les activités de vente se connectent-elles à Marketo ? {#do-sales-activities-log-to-marketo}

Oui, les activités d’engagement commercial se connectent à Marketo en tant qu’activités natives. Ces activités incluent également des filtres natifs qui peuvent être utilisés avec des contraintes pour cibler des pistes en fonction des attributs d’activité de vente.

![](assets/actions-data-sync-faq-5.png)

Vous trouverez ci-dessous la liste des activités qui se connectent à Marketo :

* Envoyer un e-mail de vente
* Ouvrir l&#39;e-mail de vente
* Cliquer sur l&#39;e-mail de vente
* A répondu à l&#39;e-mail commercial
* E-mail de vente renvoyé
* Appel de vente reçu
* Ajouter à la campagne de ventes
* Supprimé de la campagne SFDC

## Les activités de vente se connectent-elles à Salesforce ? {#do-sales-activities-log-to-salesforce}

Oui, les activités d’engagement commercial se connecteront à Salesforce en tant que tâches natives. Ces tâches peuvent ensuite être utilisées dans les rapports Salesforce pour alimenter les tableaux de bord des équipes qui effectuent le suivi des activités de vente.

Les actions Sales Insight permettent aux administrateurs de configurer les activités de vente consignées dans Salesforce. Ces activités comprennent des emails, des appels et des tâches de rappel ouvertes.

![](assets/actions-data-sync-faq-6.png)

Le diagramme ci-dessus montre les informations consignées à Salesforce. Les activités telles que les emails et les appels sont consignées dans Salesforce dans une [synchronisation unidirectionnelle](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Se désabonne](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) et [Tâches de rappel](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) sont mises à jour avec une synchronisation bidirectionnelle. Chacune de ces synchronisations de données peut être configurée à partir de l’interface de l’application web Actions d’aperçu commercial.

>[!MORELIKETHIS]
>
>* [Synchronisation des désabonnements avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Vérification de désabonnement Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Paramètres de synchronisation Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Synchronisation de la tâche de rappel avec Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Lancer la synchronisation des données](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

