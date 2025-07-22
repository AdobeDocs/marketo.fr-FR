---
description: FAQ sur la synchronisation des données d’actions - Documents Marketo - Documentation du produit
title: FAQ sur la synchronisation des données d’actions
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 3%

---

# FAQ sur la synchronisation des données d’actions {#actions-data-sync-faq}

La synchronisation des champs d’unification des données pour [!DNL Sales Insight Actions] permet au système d’extraire des informations sur la personne de votre base de données Marketo Engage vers votre base de données [!DNL Sales Insight Actions].

Cela fournit des données de personne à jour dans l’application web [!DNL Sales Insight Actions] et permet au système de collecter des identifiants uniques pour les enregistrements de personne correspondants dans Marketo et les enregistrements de prospect/contact/compte/opportunité dans [!DNL Salesforce], de sorte que les enregistrements puissent être correctement référencés pour les données de journalisation.

Cette synchronisation peut être activée à partir de l’onglet Configuration [!DNL Sales Insight Actions] dans la section Admin de Marketo Engage. Pour plus d’informations, consultez la section [ Lancement de la synchronisation des données ](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Le diagramme ci-dessus montre comment les données d&#39;activité et de tâche des personnes peuvent se synchroniser entre les systèmes. Quelques points à noter :

* Les enregistrements des personnes sont synchronisés à [!DNL Sales Insight Actions] de Marketo Engage, ce qui fait de Marketo Engage la source de vérité pour [!DNL Sales Insight Actions] données des personnes
* Marketo Engage et [!DNL Sales Insight Actions] [disposent tous deux d’un mécanisme](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) permettant de collecter et de synchroniser le statut de désabonnement avec [!DNL Salesforce]
* Le statut de désabonnement ne se synchronise pas entre les actions de vente et Marketo Engage, mais [!DNL Sales Insight Actions] pouvez être configuré pour vérifier le statut de désabonnement Marketo des personnes avant de permettre aux vendeurs d&#39;envoyer un e-mail avec la vérification de désabonnement [Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Vous trouverez ci-dessous quelques questions fréquentes relatives au fonctionnement de la synchronisation d’unification des données.

## Quels leads/contacts sont synchronisés avec [!DNL Sales Insight Actions] ? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

Les leads et les contacts auxquels un commercial est affecté seront synchronisés dans les actions de vente.

Vous pouvez voir si un prospect/contact a un commercial en [!DNL Salesforce] en examinant le champ standard du propriétaire qui existe.

Le propriétaire des ventes n’a pas besoin d’être l’utilisateur de synchronisation Marketo ou un [!DNL Salesforce] ou un utilisateur de ventes spécifique. Tout ce dont nous avons besoin, c’est d’un utilisateur répertorié dans le champ Propriétaire du prospect et Propriétaire du contact répertorié dans [!DNL Salesforce], afin que nous puissions l’identifier en tant que prospect commercial et le synchroniser dans [!DNL Sales Insight Actions]. Toutes les mises à jour des champs avec lesquels nous effectuons la synchronisation seront également détectées et mises à jour en [!DNL Sales Insight Actions].

## D’où proviennent les données d’activité affichées dans la grille intelligente de Sales Insight ? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

Les données d’activité telles que l’e-mail, l’appel, le moment intéressant et le web, proviennent toutes de la base de données Marketo Engage. La grille dynamique Sales Insight effectue une requête à l’instance Marketo Engage pour récupérer cette information chaque fois qu’un commercial charge le panneau Sales Insight.

![](assets/actions-data-sync-faq-4.png)

Pour que toutes les données d’activité puissent être sourcées à partir de Marketo Engage, [!DNL Sales Insight Actions] synchronise toutes les données d’activité avec Marketo Engage.

## Quels champs liés à la synchronisation des enregistrements des personnes de Marketo Engage vers [!DNL Sales Insight Actions] ? {#what-fields-sync}

Onze champs se synchronisent de Marketo Engage à [!DNL Sales Insight Actions] :

* Prénom
* Nom
* ID de contact [!DNL Salesforce]
* ID de lead [!DNL Salesforce]
* ID de compte [!DNL Salesforce]
* ID de l’opportunité [!DNL Salesforce]
* ID de Marketo
* Société
* Titre
* E-mail
* Numéro de téléphone
* [!DNL Linkedin] URL
* Source

## Les champs qui se synchronisent entre Marketo Engage et [!DNL Sales Insight Actions] sont-ils configurables ? {#are-the-fields-that-sync-configurable}

La configuration de la synchronisation des champs Marketo Engage avec [!DNL Sales Insight Actions] n’est pas disponible, pas plus que la possibilité de mapper les champs. La synchronisation à partir de Marketo mappe automatiquement les champs Marketo standard aux champs standard de votre instance de vente.

## Pourquoi [!DNL Sales Insight Actions] a-t-il sa propre base de données ? {#why-does-actions-have-its-own-database}

[!DNL Sales Insight Actions] dispose de sa propre application web avec une base de données de personnes et d’activités dédiée afin de fournir un espace de travail optimisé conçu pour les équipes commerciales. Cela permet aux responsables des ventes et aux vendeurs de disposer d’un espace pour élaborer et gérer leur stratégie d’engagement   sans accorder d’accès ou de privilèges à l’espace de travail Marketo Engage principal, optimisé pour les spécialistes des opérations marketing.

## Comment les doublons sont-ils gérés ? {#how-are-duplicates-handled}

Votre base de données Actions de vente sera une copie des personnes qualifiées (leads/contacts avec un commercial) qui existent dans votre base de données Marketo Engage. Cela signifie que si deux enregistrements ont la même adresse e-mail et sont créés dans Marketo, un enregistrement en double sera créé dans les actions vente.

## Combien de temps faut-il pour que la synchronisation initiale se termine ? {#how-long-initial-sync}

Le processus initial de synchronisation de toutes vos données de prospect de vente dans une nouvelle instance [!DNL Sales Insight Actions] traite généralement les personnes à environ 1 000 toutes les 1 à 2 minutes. Il s’agit simplement d’une estimation qui peut varier.

Une fois la synchronisation initiale effectuée et toutes vos pistes de vente renseignées dans votre instance d’application web [!DNL Sales Insight Actions], une synchronisation incrémentielle s’exécute chaque fois qu’une mise à jour de l’un des champs pris en charge est synchronisée.

## Les utilisateurs [!DNL Sales Insight Actions] peuvent-ils modifier les données des personnes à partir de l’application web Actions ? {#can-actions-users-edit-people-data}

Non, la possibilité de créer et de modifier des enregistrements de personnes dans Actions n’est pas disponible à la fois pour les utilisateurs et les administrateurs de l’application web Actions. La création et la modification des personnes doivent être effectuées dans [!DNL Salesforce] ou Marketo Engage. [!DNL Sales Insight Actions] utilise Marketo comme source de vérité pour les données des personnes en synchronisant en permanence les nouvelles données. Ainsi, si une personne est mise à jour ou créée dans Marketo à partir d’un workflow dans Marketo ou synchronisée à partir d’[!DNL Salesforce], ces mises à jour sont transmises à la base de données d’applications web [!DNL Sales Insight Actions].

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

## Les activités de vente se connectent-elles à [!DNL Salesforce] ? {#do-sales-activities-log-to-salesforce}

Oui, les activités d’engagement commercial seront enregistrées sur [!DNL Salesforce] en tant que tâches natives. Ces tâches peuvent ensuite être utilisées dans des rapports [!DNL Salesforce] pour alimenter les tableaux de bord de l’équipe qui effectuent le suivi des activités de vente.

[!DNL Sales Insight Actions] permet aux administrateurs de configurer les activités de vente consignées dans le [!DNL Salesforce]. Ces activités comprennent les e-mails, les appels et les tâches de rappel ouvertes.

![](assets/actions-data-sync-faq-6.png)

Le diagramme ci-dessus montre les informations consignées dans le [!DNL Salesforce]. Les activités telles que les e-mails et les appels sont consignées pour [!DNL Salesforce] dans une [synchronisation unidirectionnelle](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). Les [Désabonnements](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) et [Tâches de rappel](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) sont tenus à jour grâce à une synchronisation bidirectionnelle. Chacune de ces synchronisations de données peut être configurée à partir de [!DNL Sales Insight Actions]’interface de l’application web.

>[!MORELIKETHIS]
>
>* [Synchronisation des désabonnements avec [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Vérification du désabonnement de Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [[!DNL Salesforce] Paramètres de synchronisation](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Synchronisation de la tâche de rappel avec [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Lancer la synchronisation des données](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

