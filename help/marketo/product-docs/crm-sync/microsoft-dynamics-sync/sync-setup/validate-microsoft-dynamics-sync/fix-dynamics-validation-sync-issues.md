---
unique-page-id: 10095429
description: Correction des problèmes de synchronisation de validation Dynamics - Documents Marketo - Documentation du produit
title: Correction des problèmes de synchronisation de validation de Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 6%

---

# Correction des problèmes de synchronisation de validation de Dynamics {#fix-dynamics-validation-sync-issues}

## Validation des résultats de l’outil de synchronisation {#validate-sync-tool-results}

Lorsque vous exécutez la synchronisation de validation Dynamics, elle génère un rapport. Si une ![x](assets/delete.png) se trouve en regard d’une étape, reportez-vous aux options ci-dessous pour identifier et résoudre le problème. Ensuite, relancez les étapes de validation de synchronisation jusqu’à ce que le résultat n’affiche que des coches vertes.

![](assets/image2015-9-22-15-3a58-3a12.png)

## L’URL est valide {#url-is-valid}

Si vous avez ici un ![x](assets/delete.png), vérifiez que l’URL est valide. Trouvez-le ici dans Ressources pour les développeurs et consultez le service d’organisation. L’URL peut être invalide pour plusieurs raisons.

1. Connectez-vous à Dynamics. Cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur Paramètres et sélectionnez **Personnalisations**.

   ![](assets/two.png)

1. Cliquez sur **Ressources du développeur**.

   ![](assets/three.png)

1. L’URL du service d’organisation se trouve sous Points de terminaison du service.

   ![](assets/four.png)

## L’identifiant et le mot de passe sont valides {#username-and-password-are-valid}

Si vous avez ici un ![x](assets/delete.png), vérifiez que vos informations d’identification Microsoft Dynamics sont valides. Pour l’authentification Web API S2S, le nom d’utilisateur dans Marketo doit correspondre à l’ [adresse électronique](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) de l’utilisateur de l’application dans le CRM. Pour les autres types, il doit correspondre au nom d’utilisateur de l’utilisateur de synchronisation.

## L’utilisateur de synchronisation est affecté au rôle Utilisateur de synchronisation Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Si vous avez un ![x](assets/delete.png) ici, il peut s’agir de l’un des trois problèmes ci-dessous.

**Option 1 - Vérifiez que le rôle d’utilisateur de synchronisation Marketo est coché dans Microsoft Dynamics** :

1. Dans Dynamics, cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres** et sélectionnez **Sécurité**.

   ![](assets/six.png)

1. Cliquez sur **Users.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Cliquez sur le lien correspondant à l’utilisateur de synchronisation.

   ![](assets/seven.png)

1. Cliquez sur **Gérer les rôles**.

   ![](assets/eight.png)

1. Vérifiez que le rôle Utilisateur de synchronisation Marketo est coché. Si ce n&#39;est pas le cas, cochez-le et cliquez sur **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Option 2 - Confirmer l’octroi du consentement** :

1. Passez en revue l’ [octroi du consentement pour l’ID de client et l’enregistrement d’application](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) pour confirmer que l’application a le consentement de l’administrateur pour appeler des API.

**Option 3 - Utilisateur de synchronisation** :

1. Vérifiez que l’utilisateur de synchronisation est ajouté à la configuration Marketo.

## La solution Marketo est bien installée {#marketo-solution-is-properly-installed}

Si vous avez ici un ![x](assets/delete.png), accédez à Microsoft Dynamics pour vérifier que l’installation de Marketo est bien là. Voir l’étape 1 de la documentation de configuration de Microsoft Dynamics.

1. Dans Dynamics, cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Settings** et sélectionnez **Solutions.**

   ![](assets/eleven.png)

1. Vérifiez que la solution est répertoriée.

   ![](assets/twelve.png)

## Toutes les étapes de la solution sont activées {#all-steps-in-the-solution-are-enabled}

Si vous avez ici un ![x](assets/delete.png), vérifiez qu’aucune des étapes par défaut n’a été désactivée. Toutes les étapes sont automatiquement activées lors de l’installation, mais elles peuvent être désactivées lors d’une personnalisation.

## L’utilisateur synchronisé est attribué à la solution Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Si vous avez ici un ![x](assets/delete.png), assurez-vous que l’utilisateur de synchronisation est affecté sur la page Marketo par défaut dans Microsoft Dynamics.

1. Dans Dynamics, cliquez sur l’icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres** et sélectionnez **Configuration Marketo**.

   ![](assets/thirteen.png)

1. Vérifiez que l’utilisateur de synchronisation est désigné comme valeur par défaut.

   ![](assets/fourteen.png)

## L’utilisateur synchonisé correspond au nom d’utilisateur et au mot de passe {#sync-user-matches-username-and-password}

Si vous avez ici un ![x](assets/delete.png), veillez à affecter l’utilisateur de synchronisation approprié dans le champ Utilisateur Marketo dans l’étape de configuration par défaut de la configuration Marketo dans Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Valider la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
