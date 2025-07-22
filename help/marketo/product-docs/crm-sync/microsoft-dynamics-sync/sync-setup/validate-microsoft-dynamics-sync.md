---
unique-page-id: 8783322
description: Validate [!DNL Microsoft Dynamics] Sync - Documents Marketo - Documentation Du Produit
title: Valider [!DNL Microsoft Dynamics] Sync
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# Valider [!DNL Microsoft Dynamics] synchronisation {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Si Multi-Factor Authentication (MFA) est activé pour votre synchronisation [!DNL Dynamics], vous devez la désactiver pour que [!DNL Dynamics] puissiez effectuer correctement la synchronisation avec Marketo. Pour plus d’informations, contactez l’assistance Marketo [&#128279;](https://nation.marketo.com/t5/Support/ct-p/Support).

## Exécuter la synchronisation de validation dans Marketo {#run-validate-sync-in-marketo}

Il est très important d’exécuter l’outil Valider la synchronisation pour vous assurer que la synchronisation [!DNL Microsoft Dynamics] avec Marketo est correctement configurée avant d’établir la connexion finale entre eux. Le processus génère une liste de contrôle de sept étapes de configuration qui identifient les problèmes éventuels. Vérifier que tout cela a été fait correctement peut vous faire gagner beaucoup de temps plus tard.

1. Cliquez sur l’onglet **[!UICONTROL Admin]**, puis sur le lien **[!DNL Microsoft Dynamics]** dans la zone Intégration .

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Sélectionnez **[!DNL Microsoft]**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Cliquez sur l’onglet **[!UICONTROL Valider la configuration de la synchronisation]**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Saisissez votre nom d’utilisateur, votre mot de passe et votre URL (l’ID client et le secret client sont facultatifs). Cliquez sur **[!UICONTROL Suivant]** lorsque vous avez terminé.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Si vous avez déjà effectué une synchronisation, la mention **CRM** dans l’arborescence de gauche **[!DNL Microsoft Dynamics]** lira, et les données du formulaire ci-dessus peuvent être préremplies.

1. Si tout va bien, la fonction Valider la synchronisation génère une liste de contrôle remplie de coches vertes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Si vous voyez une ![ — ](assets/delete.png), alors cette étape pose un problème. Voir [Correction [!DNL Dynamics] des problèmes de synchronisation de validation](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) pour identifier et résoudre le problème. Réexécutez ensuite les étapes de validation de la synchronisation jusqu’à ce que le résultat ressemble à l’image ci-dessus.

   >[!CAUTION]
   >
   >Nous ne prenons actuellement pas en charge l’actualisation du sandbox pour la synchronisation [!DNL Marketo Dynamics]. Si vous devez actualiser votre sandbox CRM [!DNL Dynamics], un nouveau sandbox Marketo sera requis. Contactez votre responsable du succès client pour plus d’informations.

>[!MORELIKETHIS]
>
>[Correction [!DNL Dynamics] Problèmes de synchronisation de la validation](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
