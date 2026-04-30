---
unique-page-id: 11386358
description: Découvrez le sandbox Marketo Engage à des fins de test avant la production. Utilisez une instance sandbox pour effectuer des tests sans affecter la production.
title: Sandbox Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 8bb13497a5173f355563e2badf867a5f847be488
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 3%

---

# Sandbox Marketo {#marketo-sandbox}

Un sandbox Marketo Engage est une instance supplémentaire utilisée à des fins de test avant son implémentation dans l’environnement de production.

>[!AVAILABILITY]
>
>Tout le monde n’a pas acheté cette fonctionnalité. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

Un sandbox Marketo ne peut pas être synchronisé avec votre CRM standard s’il est déjà synchronisé avec votre instance de production. Utilisez le sandbox de votre CRM pour la synchronisation, et suivez toutes les mêmes étapes que la synchronisation d’origine.

## Choses à savoir sur les sandbox {#things-to-know-about-sandboxes}

* Si vous souhaitez ajouter des utilisateurs, le processus est identique à [ajout d’utilisateurs en production](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#add-a-user). Là encore, ils doivent utiliser une adresse e-mail différente s’ils disposent déjà d’un identifiant Marketo.
* Votre sandbox Marketo sera initialement vide, mais disposera des mêmes fonctionnalités que votre instance de production.
* Si vous créez un programme dans votre sandbox et souhaitez le déplacer en production, vous pouvez effectuer une [importation de programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Les sandbox sont limités afin que les instances de production ne soient pas affectées négativement par les environnements de test. Vous pouvez envoyer jusqu’à 20 e-mails par exécution de campagne.

>[!CAUTION]
>
>L’actualisation du sandbox pour la synchronisation de Marketo Dynamics _ou_ Salesforce n’est pas prise en charge pour le moment. Si vous devez actualiser votre sandbox CRM, un nouveau sandbox Marketo est requis. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

## Copie d’instance {#instance-copy}

Vous pouvez envoyer un dossier d’assistance demandant une copie d’instance unique pour remplir votre sandbox. Cependant, la copie d’instance ne transportera pas _tout_. Pour plus d’informations, contactez l’assistance technique de [&#128279;](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>Si vous modifiez votre CRM natif, une nouvelle instance Marketo est nécessaire et une copie d’instance vers la nouvelle instance Marketo n’est pas possible. Au lieu de cela, travaillez avec la prise en charge de Marketo pour explorer la fonctionnalité de programme d’importation.
