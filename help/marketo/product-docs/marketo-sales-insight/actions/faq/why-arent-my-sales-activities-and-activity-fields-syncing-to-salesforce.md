---
description: Pourquoi mes activités de vente et champs d’activité ne sont-ils pas synchronisés avec Salesforce ? - Documents Marketo - Documentation sur le produit
title: Pourquoi mes activités de vente et mes champs d’activité ne sont-ils pas synchronisés avec Salesforce ?
exl-id: 5da855f2-18c6-456a-9e5d-ef4499596b3c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 7%

---

# Pourquoi mes activités de vente et mes champs d’activité ne sont-ils pas synchronisés avec Salesforce ? {#why-arent-my-sales-activities-and-activity-fields-syncing-to-salesforce}

**Je ne vois pas les activités d’e-mail ou d’appel synchronisées avec Salesforce.**

* Vérifiez que vous êtes connecté à Salesforce. Chaque utilisateur devra disposer d’une connexion pour consigner ses e-mails et appels vers Salesforce.
* Vérifiez que vous avez configuré les [paramètres de synchronisation Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}.
* Les e-mails effectueront une recherche d’enregistrement en fonction de l’identifiant Salesforce comme recherche principale et de l’adresse e-mail comme adresse secondaire. Vous pouvez confirmer qu’un enregistrement de personne possède un Salesforce ID et une adresse e-mail qui lui sont associés dans l’application web [Actions](https://toutapp.com/next#command_center){target="_blank"}.
* Les appels effectueront une recherche d’enregistrement en fonction de l’identifiant Salesforce uniquement. S’il n’existe aucun ID Salesforce dans l’enregistrement de personne dans Actions, l’appel ne se connecte pas. Vous pouvez confirmer qu’un enregistrement de personne est associé à un Salesforce ID dans l’application web [Actions](https://toutapp.com/next#command_center){target="_blank"}.

**Je ne vois pas les champs d’activité dans la mise à jour de Salesforce.**

Si vous ne voyez pas la mise à jour des champs d’attribut d’activité [e-mail](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} dans Salesforce, cela peut être dû à des restrictions sur l’accessibilité des champs de votre équipe. La sécurité au niveau du champ Salesforce permet aux administrateurs Salesforce de définir des restrictions quant aux informations visibles et modifiables par les utilisateurs. Si les utilisateurs d’Actions ne sont pas autorisés à afficher et modifier ces champs, la synchronisation de l’activité Actions ne parvient pas à mettre à jour ces champs.

* Contactez votre administrateur Salesforce pour vous assurer que ces paramètres de sécurité n’interfèrent pas avec les [champs d’activité du Salesforce Actions](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}.
* Si vous êtes un administrateur Salesforce, vous pouvez afficher l’accessibilité des champs sous l’onglet Contrôles de sécurité . Les principaux objets avec lesquels les actions interagiront sont les suivants : leads, contacts, comptes, opportunités et tâche/activités.

>[!NOTE]
>
>Les champs associés aux objets Lead, Contact, Compte et Opportunité seront installés avec le package Salesforce Sales Insight. Les champs associés au type d’enregistrement [Tâche/Activité) devront être créés](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"} par un administrateur Salesforce.
