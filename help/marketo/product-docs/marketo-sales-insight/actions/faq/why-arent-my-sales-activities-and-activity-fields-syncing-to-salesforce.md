---
description: Pourquoi mes activités de vente et mes champs d’activité ne sont-ils pas synchronisés avec Salesforce ? - Documents Marketo - Documentation du produit
title: Pourquoi mes activités de vente et mes champs d’activité ne sont-ils pas synchronisés avec Salesforce ?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Pourquoi mes activités de vente et mes champs d’activité ne sont-ils pas synchronisés avec Salesforce ? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Je ne vois pas d&#39;activités d&#39;appel ou de messagerie synchronisées avec Salesforce.**

* Vérifiez que vous êtes connecté à Salesforce. Chaque utilisateur doit disposer d’une connexion pour consigner son email et ses appels à Salesforce.
* Assurez-vous d’avoir configuré les [paramètres de synchronisation Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Les courriers électroniques effectuent une recherche d’enregistrement basée sur l’identifiant Salesforce comme recherche principale et l’adresse électronique comme adresse secondaire. Vous pouvez confirmer qu’un ID Salesforce et une adresse électronique sont associés à un enregistrement de personne dans l’ [application web Actions](https://toutapp.com/next#command_center){target="_blank"}.
* Les appels effectuent une recherche d’enregistrement en fonction de l’identifiant Salesforce uniquement. S’il n’existe aucun identifiant Salesforce sur l’enregistrement de la personne dans les actions, l’appel ne sera pas consigné. Vous pouvez confirmer qu’un identifiant Salesforce est associé à un enregistrement de personne dans l’ [application web Actions](https://toutapp.com/next#command_center){target="_blank"}.

**Je ne vois pas les champs d&#39;activité dans la mise à jour de Salesforce.**

Si vous ne voyez pas la mise à jour des [champs d’attribut d’activité](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} de l’email dans Salesforce, cela peut être dû à des restrictions de l’accessibilité des champs de votre équipe. La sécurité au niveau du champ Salesforce permet aux administrateurs Salesforce de placer des restrictions sur les informations que les utilisateurs peuvent afficher et modifier. Si les utilisateurs d’Actions n’ont pas accès à l’affichage et à la modification de ces champs, la synchronisation de l’activité Actions ne pourra pas mettre à jour ces champs.

* Consultez votre administrateur Salesforce pour vous assurer que ces paramètres de sécurité n’interférent pas avec les [champs d’activité Salesforce d’actions](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Si vous êtes un administrateur Salesforce, vous pouvez voir votre accessibilité des champs sous l’onglet Contrôles de sécurité . Les principaux objets avec lesquels les actions interagiront sont les suivants : pistes, contacts, comptes, opportunités et tâches/activités.

>[!NOTE]
>
>Les champs associés aux objets Lead, Contact, Account et Opportunity seront installés avec le package Sales Insight Salesforce. Les champs associés au type d’enregistrement [Tâche/Activité devront être créés](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} par un administrateur Salesforce.
