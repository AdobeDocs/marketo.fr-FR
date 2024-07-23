---
unique-page-id: 11386358
description: Environnement de test Marketo - Documents Marketo - Documentation du produit
title: Marketo Sandbox
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: e6a5b6c84ce12c0bb4d1df013bcd4471d71ce2c2
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Marketo Sandbox {#marketo-sandbox}

Un environnement de test de Marketo Engage est une instance supplémentaire utilisée à des fins de test avant l’implémentation dans l’environnement de production.

>[!AVAILABILITY]
>
>Cette fonctionnalité n’a pas été achetée par tout le monde. Pour plus d’informations, contactez l’équipe de compte d’Adobe (votre gestionnaire de compte).

Un environnement de test Marketo ne peut pas être synchronisé avec votre système de gestion de la relation client classique s’il est déjà synchronisé avec votre instance de production. Utilisez l’environnement de test de votre CRM pour la synchronisation et procédez comme pour la synchronisation d’origine.

## Informations à connaître sur les environnements de test {#things-to-know-about-sandboxes}

* Si vous souhaitez ajouter des utilisateurs, le processus est identique à [l’ajout d’utilisateurs en production](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). Là encore, ils doivent utiliser une autre adresse électronique s’ils disposent déjà d’une connexion Marketo.
* Votre environnement de test Marketo va commencer vide, mais dispose des mêmes fonctionnalités que votre instance de production.
* Si vous créez un programme dans votre environnement de test et souhaitez le déplacer en production, vous pouvez effectuer un [import de programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Les environnements de test sont ralentis afin que les instances de production ne soient pas affectées négativement par les environnements de test. Vous pouvez envoyer jusqu’à 20 emails par exécution de campagne.

>[!CAUTION]
>
>Actuellement, nous ne prenons pas en charge l’actualisation des environnements de test pour la synchronisation Marketo Dynamics. Si vous devez actualiser votre environnement de test Dynamics CRM, un nouvel environnement de test Marketo est requis. Pour plus d’informations, contactez votre équipe de compte d’Adobe (votre gestionnaire de compte).

## Copie de l’instance {#instance-copy}

Vous pouvez soumettre un cas d’assistance demandant une copie d’instance unique pour remplir votre environnement de test. Cependant, la copie d’instance n’apporte pas _tout_. Pour plus d’informations, consultez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) .

>[!NOTE]
>
>Si vous modifiez votre gestion de la relation client native, une nouvelle instance Marketo est nécessaire et une copie d’instance vers la nouvelle instance Marketo n’est pas possible. Au lieu de cela, contactez le support Marketo pour explorer la fonctionnalité d’importation de programme.
