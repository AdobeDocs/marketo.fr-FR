---
unique-page-id: 10095429
description: Correction Des Problèmes De Synchronisation De La Validation De Dynamics - Documents Marketo - Documentation Du Produit
title: Corriger les problèmes de synchronisation de validation Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 9%

---

# Corriger les problèmes de synchronisation de validation Dynamics {#fix-dynamics-validation-sync-issues}

## Valider les résultats de l’outil de synchronisation {#validate-sync-tool-results}

Lorsque vous exécutez la synchronisation de validation de Dynamics, elle génère un rapport. S’il y a un ![x](assets/delete.png) en regard d’une étape, consultez les options ci-dessous pour identifier et résoudre le problème. Réexécutez ensuite les étapes de validation de la synchronisation jusqu’à ce que le résultat n’affiche plus que des coches vertes.

![](assets/image2015-9-22-15-3a58-3a12.png)

## L’URL est valide {#url-is-valid}

Si vous disposez d’une ![x](assets/delete.png) ici, vérifiez que l’URL est valide. Recherchez-le ici dans Ressources pour les développeurs et consultez Service d’organisation. L’URL peut ne pas être valide pour plusieurs raisons.

1. Connectez-vous à Dynamics. Cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur Paramètres et sélectionnez **Personnalisations**.

   ![](assets/two.png)

1. Cliquez sur **Ressources pour les développeurs**.

   ![](assets/three.png)

1. L’URL du service d’organisation se trouve sous Points d’entrée du service.

   ![](assets/four.png)

## L’identifiant et le mot de passe sont valides {#username-and-password-are-valid}

Si vous disposez d’un ![x](assets/delete.png) ici, vérifiez que vos informations d’identification Microsoft Dynamics sont valides. Pour l’authentification S2S de l’API Web, le nom d’utilisateur dans Marketo doit correspondre à l’[adresse e-mail](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) de l’utilisateur de l’application dans le CRM. Pour les autres types, il doit correspondre au nom d’utilisateur de la synchronisation des utilisateurs.

## L’utilisateur de synchronisation est affecté au rôle Utilisateur de synchronisation Marketo . {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Si vous avez un ![x](assets/delete.png) ici, il peut s’agir de l’un des trois problèmes ci-dessous.

**Option 1 - Vérifiez que le rôle Utilisateur de synchronisation Marketo est activé dans Microsoft Dynamics** :

1. Dans Dynamics, cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres** et sélectionnez **Sécurité**.

   ![](assets/six.png)

1. Cliquez sur **Utilisateurs.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Cliquez sur le lien correspondant à l’utilisateur de synchronisation.

   ![](assets/seven.png)

1. Cliquez sur **Gérer les rôles**.

   ![](assets/eight.png)

1. Vérifiez que le rôle Utilisateur de synchronisation Marketo est coché. Si ce n&#39;est pas le cas, cochez-la et cliquez sur **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Option 2 - Confirmer l’octroi du consentement** :

1. Consultez la section [Accorder le consentement pour l’ID client et l’enregistrement de l’application](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) pour confirmer que l’application dispose du consentement administrateur pour appeler les API.

**Option 3 - Synchroniser l’utilisateur** :

1. Vérifiez que l’utilisateur de synchronisation est ajouté à la configuration Marketo.

## La solution Marketo est bien installée {#marketo-solution-is-properly-installed}

Si vous disposez d’un ![x](assets/delete.png) ici, accédez à Microsoft Dynamics pour vérifier que l’installation de Marketo s’y trouve. Voir l’étape 1 de la documentation sur la configuration de Microsoft Dynamics.

1. Dans Dynamics, cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres** et sélectionnez **Solutions.**

   ![](assets/eleven.png)

1. Vérifiez que la solution figure dans la liste.

   ![](assets/twelve.png)

## Toutes les étapes de la solution sont activées {#all-steps-in-the-solution-are-enabled}

Si vous disposez d’un ![x](assets/delete.png) ici, vérifiez qu’aucune des étapes par défaut n’a été désactivée. Toutes les étapes sont automatiquement activées lors de l’installation, mais elles peuvent être désactivées au cours d’une personnalisation.

## L’utilisateur synchronisé est attribué à la solution Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Si vous disposez d’un ![x](assets/delete.png) ici, assurez-vous que l’utilisateur de la synchronisation est affecté à la page par défaut de Marketo dans Microsoft Dynamics.

1. Dans Dynamics, cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres** et sélectionnez **Configuration Marketo**.

   ![](assets/thirteen.png)

1. Vérifiez que l’utilisateur de synchronisation est affecté comme valeur par défaut.

   ![](assets/fourteen.png)

## L’utilisateur synchonisé correspond au nom d’utilisateur et au mot de passe {#sync-user-matches-username-and-password}

Si vous disposez d’un ![x](assets/delete.png) ici, veillez à attribuer l’utilisateur de synchronisation approprié dans le champ Utilisateur Marketo dans l’étape Configuration par défaut de la configuration de Marketo dans Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
