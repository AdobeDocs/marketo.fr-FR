---
unique-page-id: 8783322
description: Validation de la synchronisation Microsoft Dynamics - Documents Marketo - Documentation du produit
title: Validation de la synchronisation Microsoft Dynamics
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Validation de la synchronisation Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Si l’authentification à plusieurs facteurs (MFA) est activée pour votre synchronisation Dynamics, vous devez la désactiver pour que Dynamics se synchronise correctement avec Marketo. Pour plus d’informations, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

## Exécuter la validation de la synchronisation dans Marketo {#run-validate-sync-in-marketo}

Il est très important d’exécuter l’outil Valider la synchronisation pour vous assurer que votre synchronisation Microsoft Dynamics avec Marketo est configurée correctement avant d’établir la connexion finale entre elles. Le processus génère une liste de contrôle de sept étapes de configuration qui déterminent où des problèmes existent. La vérification correcte de ces tâches peut vous faire gagner du temps.

1. Cliquez sur l’onglet **[!UICONTROL Admin]** , puis sur le lien **[!DNL Microsoft Dynamics]** dans la zone Intégration.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Sélectionnez **[!DNL Microsoft]**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Cliquez sur l’onglet **[!UICONTROL Valider la configuration de synchronisation]** .

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Saisissez votre nom d’utilisateur, votre mot de passe et votre URL (l’identifiant du client et le secret du client sont facultatifs). Cliquez sur **[!UICONTROL Suivant]** une fois terminé.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Si vous avez déjà synchronisé , **[!UICONTROL CRM]** dans l’arborescence de gauche sera lu **[!DNL Microsoft Dynamics]**, et les données du formulaire ci-dessus peuvent être préremplies.

1. Si tout va bien, la synchronisation de validation génère une liste de contrôle remplie de coches vertes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Si vous voyez un ![—](assets/delete.png), cette étape présente un problème. Voir [Correction des problèmes de synchronisation de validation de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"} pour identifier et résoudre le problème. Exécutez à nouveau les étapes de validation de la synchronisation jusqu’à ce que le résultat ressemble à l’image ci-dessus.

   >[!CAUTION]
   >
   >Actuellement, nous ne prenons pas en charge l’actualisation des environnements de test pour la synchronisation Marketo Dynamics. Si vous devez actualiser votre environnement de test Dynamics CRM, un nouvel environnement de test Marketo est requis. Pour plus d’informations, contactez l’équipe du compte d’Adobe (votre gestionnaire de compte).

>[!MORELIKETHIS]
>
>[Correction des problèmes de synchronisation de validation Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"}
