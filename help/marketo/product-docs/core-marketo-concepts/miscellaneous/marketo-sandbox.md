---
unique-page-id: 11386358
description: Marketo Sandbox - Marketo Docs - Documentation du produit
title: Marketo Sandbox
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Marketo Sandbox {#marketo-sandbox}

Un sandbox Marketo est une instance supplémentaire utilisée à des fins de test avant la mise en oeuvre dans l’environnement de production.

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Pour plus d’informations, contactez votre responsable de succès client.

Un sandbox Marketo ne peut pas être synchronisé avec votre gestion de la relation client standard s’il est déjà synchronisé avec votre instance de production. Utilisez le sandbox de la gestion de la relation client pour la synchronisation et suivez toutes les étapes de la synchronisation d’origine.

## Informations sur les sandbox {#things-to-know-about-sandboxes}

* Une fois que votre sandbox a été configuré pour le Gestionnaire de succès client et que vous avez envoyé l’invitation, vous devez utiliser une adresse électronique différente de celle de votre instance de production Marketo pour vous connecter.
* Si vous souhaitez ajouter des utilisateurs, le processus est le même que l&#39;[ajout d&#39;utilisateurs en production](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). Là encore, ils doivent utiliser une autre adresse électronique s&#39;ils ont déjà une connexion Marketo.
* Votre sandbox Marketo sera début vide, mais les mêmes fonctionnalités seront disponibles que votre instance de production.
* Si vous créez un programme dans votre sandbox et souhaitez le déplacer vers la production, vous pouvez effectuer une [importation de programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Les sandbox sont ralentis afin que les instances de production ne soient pas affectées par les environnements de test. Vous pouvez envoyer jusqu’à 30 courriers électroniques par exécution de campagne.

>[!CAUTION]
>
>Actuellement, nous ne prenons pas en charge l&#39;actualisation de sandbox pour Marketo Dynamics Sync. Si vous devez actualiser votre sandbox Dynamics CRM, un nouveau sandbox Marketo sera nécessaire. Pour plus d’informations, contactez votre responsable de succès client.

## Copie d&#39;instance {#instance-copy}

Vous pouvez envoyer un dossier d&#39;assistance demandant une copie d&#39;instance unique pour remplir votre sandbox. Cependant, la copie d&#39;instance n&#39;apporte pas _tout_. Pour plus de détails, veuillez consulter [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>* La copie d&#39;instance est **non** prise en charge si l&#39;instance source est intégrée à Microsoft Dynamics.
>* Si vous modifiez votre gestion de la relation client native, une nouvelle instance Marketo est nécessaire, et une copie d’instance vers la nouvelle instance Marketo n’est pas possible. Au lieu de cela, demandez à l&#39;assistance Marketo d&#39;explorer la fonctionnalité d&#39;importation de Programme.

