---
unique-page-id: 11386358
description: Sandbox Marketo - Documentation de Marketo - Documentation du produit
title: Sandbox Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Sandbox Marketo {#marketo-sandbox}

Un sandbox Marketo Engage est une instance supplémentaire utilisée à des fins de test avant son implémentation dans l’environnement de production.

>[!AVAILABILITY]
>
>Tout le monde n’a pas acheté cette fonctionnalité. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

Un sandbox Marketo ne peut pas être synchronisé avec votre CRM standard s’il est déjà synchronisé avec votre instance de production. Utilisez le sandbox de votre CRM pour la synchronisation, et suivez toutes les mêmes étapes que la synchronisation d’origine.

## Choses à savoir sur les sandbox {#things-to-know-about-sandboxes}

* Si vous souhaitez ajouter des utilisateurs, le processus est identique à [ajout d’utilisateurs en production](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). Là encore, ils doivent utiliser une adresse e-mail différente s’ils disposent déjà d’un identifiant Marketo.
* Votre sandbox Marketo sera initialement vide, mais disposera des mêmes fonctionnalités que votre instance de production.
* Si vous créez un programme dans votre sandbox et souhaitez le déplacer en production, vous pouvez effectuer une [importation de programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Les sandbox sont limités afin que les instances de production ne soient pas affectées négativement par les environnements de test. Vous pouvez envoyer jusqu’à 20 e-mails par exécution de campagne.

>[!CAUTION]
>
>Nous ne prenons pas actuellement en charge l’actualisation du sandbox pour la synchronisation de Marketo Dynamics. Si vous devez actualiser votre sandbox Dynamics CRM, un nouveau sandbox Marketo sera requis. Pour plus d’informations, contactez l’équipe chargée de votre compte Adobe (votre gestionnaire de compte).

## Copie d’instance {#instance-copy}

Vous pouvez envoyer un dossier d’assistance demandant une copie d’instance unique pour remplir votre sandbox. Cependant, la copie d’instance ne transportera pas _tout_. Veuillez consulter le support technique de [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) pour plus d&#39;informations.

>[!NOTE]
>
>Si vous modifiez votre CRM natif, une nouvelle instance Marketo est nécessaire et une copie d’instance vers la nouvelle instance Marketo n’est pas possible. Au lieu de cela, veuillez travailler avec le support Marketo pour explorer la fonctionnalité du programme d’importation.
