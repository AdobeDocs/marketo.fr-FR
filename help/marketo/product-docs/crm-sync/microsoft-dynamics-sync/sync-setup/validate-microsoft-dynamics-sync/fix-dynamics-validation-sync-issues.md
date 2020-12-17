---
unique-page-id: 10095429
description: Correction des problèmes de synchronisation de la validation de la dynamique - Documents marketing - Documentation du produit
title: Correction des problèmes de synchronisation de validation de Dynamics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


# Correction des problèmes de synchronisation de validation de Dynamics {#fix-dynamics-validation-sync-issues}

## Valider les résultats de l&#39;outil de synchronisation {#validate-sync-tool-results}

Lorsque vous exécutez Dynamics Validate Sync, il génère ce rapport. Si ![delete](assets/delete.png) se trouve en regard d&#39;une étape, reportez-vous à la section ci-dessous pour identifier et résoudre le problème. Réexécutez ensuite les étapes de validation de synchronisation jusqu’à ce que le résultat n’affiche rien d’autre que des coches.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL valide {#url-is-valid}

Si ![delete](assets/delete.png) se trouve ici, vérifiez que l’URL est valide. Reportez-vous à la section Ressources pour les développeurs et consultez la section Service d&#39;organisation. L&#39;URL peut être non valide pour plusieurs raisons.

1. Connexion à Dynamics. Cliquez sur l&#39;icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur Paramètres et sélectionnez **Personnalisations**.

   ![](assets/two.png)

1. Cliquez sur **Ressources du développeur**.

   ![](assets/three.png)

1. L&#39;URL du service d&#39;organisation se trouve sous Points de terminaison du service.

   ![](assets/four.png)

## Le nom d&#39;utilisateur et le mot de passe sont valides {#username-and-password-are-valid}

Si vous avez ![—](assets/delete.png) ici, vérifiez que votre nom d&#39;utilisateur et votre mot de passe Microsoft Dynamics sont valides.

## L&#39;utilisateur de synchronisation est affecté au rôle Utilisateur de synchronisation du marketing {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Si vous avez ![—](assets/delete.png) ici, vous devez vérifier que le rôle Utilisateur de synchronisation de Marketo est coché dans Microsoft Dynamics. Reportez-vous à l&#39;étape 2 de la documentation d&#39;installation de Microsoft Dynamics.

1. Dans Dynamics, cliquez sur l&#39;icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres** et sélectionnez **Sécurité**.

   ![](assets/six.png)

1. Cliquez sur **Utilisateurs.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Cliquez sur le lien correspondant à l’utilisateur de synchronisation.

   ![](assets/seven.png)

1. Cliquez sur **Gérer les rôles**.

   ![](assets/eight.png)

1. Vérifiez que le rôle Utilisateur de synchronisation de marketing est coché. Si ce n’est pas le cas, cochez-le et cliquez sur **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## La solution Marketo est correctement installée {#marketo-solution-is-properly-installed}

Si vous avez ![—](assets/delete.png) ici, accédez à Microsoft Dynamics pour vérifier que l&#39;installation de Marketo est présente. Reportez-vous à l&#39;étape 1 de la documentation de configuration de Microsoft Dynamics.

1. Dans Dynamics, cliquez sur l&#39;icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres **et sélectionnez **Solutions.**

   ![](assets/eleven.png)

1. Vérifiez que la solution est répertoriée.

   ![](assets/twelve.png)

## Toutes les étapes de la solution sont activées {#all-steps-in-the-solution-are-enabled}

Si vous avez ![—](assets/delete.png) ici, vérifiez qu’aucune des étapes par défaut n’a été désactivée. Toutes les étapes sont automatiquement activées lors de l’installation, mais elles peuvent être désactivées lors d’une personnalisation.

## L&#39;utilisateur de synchronisation est affecté à la solution Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Si vous avez ![—](assets/delete.png) ici, assurez-vous que l&#39;utilisateur Sync est affecté sur la page Marketo Default de Microsoft Dynamics.

1. Dans Dynamics, cliquez sur l&#39;icône Paramètres et sélectionnez **Paramètres avancés**.

   ![](assets/one.png)

1. Cliquez sur **Paramètres **et sélectionnez **Marketo Config**.

   ![](assets/thirteen.png)

1. Vérifiez que l’utilisateur de synchronisation est affecté comme utilisateur par défaut.

   ![](assets/fourteen.png)

## Synchroniser l’utilisateur correspond au nom d’utilisateur et au mot de passe {#sync-user-matches-username-and-password}

Si vous avez ![—](assets/delete.png) ici, veillez à affecter l&#39;utilisateur de synchronisation approprié dans le champ Utilisateur de Marketo dans l&#39;étape de configuration par défaut de la configuration de Marketo dans Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Valider Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

