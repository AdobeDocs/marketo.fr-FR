---
unique-page-id: 8783322
description: Valider Microsoft Dynamics Sync - Marketo Docs - Documentation du produit
title: Valider Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# Valider Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Si l&#39;authentification multifacteur (MFA) est activée pour Dynamics Sync, vous devez la désactiver pour que Dynamics se synchronise correctement avec Marketo. Pour de plus amples informations, veuillez contacter l&#39;assistance [](http://nation.marketo.com/community/support_solutions)marketing.

## Exécuter la validation de la synchronisation dans Marketo {#run-validate-sync-in-marketo}

Il est très important d&#39;exécuter l&#39;outil Valider la synchronisation pour s&#39;assurer que Microsoft Dynamics Sync avec Marketo est configuré correctement avant d&#39;établir la connexion finale entre eux. Le processus génère une liste de contrôle de sept étapes de configuration qui identifie les problèmes existants. La vérification de ces informations correctement effectuée peut vous faire gagner beaucoup de temps par la suite.

1. Cliquez sur l&#39;onglet **Admin** , puis sur le lien **Microsoft Dynamics** dans la zone Intégration.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Sélectionnez **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Cliquez sur l’onglet **Valider la configuration** de synchronisation.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Saisissez votre nom d’utilisateur, votre mot de passe et votre URL (l’ID de client et la clé secrète client sont facultatifs). Lorsque vous avez terminé, cliquez sur **Suivant** .

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Si vous avez déjà effectué la synchronisation, **CRM** dans l&#39;arborescence de gauche lit **Microsoft Dynamics** et les données du formulaire ci-dessus peuvent être préremplies.

1. Si tout va bien, la fonction Valider la synchronisation génère une liste de contrôle pleine de coches vertes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Si vous voyez un ![—](assets/delete.png), alors cette étape a un problème. Voir [Correction des problèmes](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) de synchronisation de validation de Dynamics pour identifier et résoudre le problème. Ensuite, réexécutez les étapes de validation de synchronisation jusqu’à ce que le résultat ressemble à l’image ci-dessus.

   >[!CAUTION]
   >
   >Actuellement, nous ne prenons pas en charge l&#39;actualisation de sandbox pour Marketing Dynamics Sync. Si vous devez actualiser votre sandbox Dynamics CRM, un nouveau sandbox Marketo sera nécessaire. Pour plus d’informations, contactez votre responsable de succès client.

>[!NOTE]
>
>**Articles connexes**
>
>[Correction des problèmes de synchronisation de validation de Dynamics](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

